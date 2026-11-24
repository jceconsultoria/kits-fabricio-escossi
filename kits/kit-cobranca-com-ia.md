# Kit: cobrança com IA, em 8 passos

Por Fabrício Escossi · JCE Consultoria · versão 1, novembro de 2026

Este arquivo leva para a sua IA a rotina do post "Cobrança com IA, em 8 passos". Ele traz as instruções fixas, a
política de cobrança da sua empresa para preencher e um prompt para cada passo: das faixas de atraso à rotina de
segunda-feira. Funciona no ChatGPT, no Claude, no Copilot e no Gemini.

## Como usar, em 4 passos

1. **Crie um espaço fixo na sua IA** chamado "Cobrança":
   - ChatGPT ou Claude: um Projeto;
   - Gemini: um Gem;
   - Copilot: um Notebook, ou anexe este arquivo no início de cada conversa.
2. **Cole o bloco "Instruções para a IA"** nas instruções fixas desse espaço.
3. **Preencha "A política de cobrança da casa"** e cole abaixo das instruções. É ela que define faixas, tom e
   alçadas. Se a empresa ainda não tem uma política escrita, este é um bom momento para combinar com quem decide.
4. **Na primeira vez, rode os prompts 1 a 5 na ordem.** Depois, toda segunda, rode só o prompt da rotina semanal.

## Cuidados com os dados (leia antes)

- Use a versão corporativa da ferramenta e confira a política de dados da empresa.
- Cliente entra por código, nunca por nome, CPF, CNPJ ou telefone. Exporte só código, documento, vencimento, data de
  pagamento e valor.
- As mensagens saem com [NOME] e [CONTATO] em branco. A equipe completa no sistema da empresa, não na IA.
- A IA organiza e rascunha. Desconto, parcelamento, protesto, negativação, bloqueio de crédito e ação judicial são
  decisões de quem tem alçada.
- Cobrança não constrange nem expõe a dívida a terceiros. Nada de mensagem em grupo, ameaça ou contato fora do
  horário combinado.

## Instruções para a IA (copie e cole)

```
Você é assistente de contas a receber da empresa descrita em "A política de cobrança da casa". Você organiza a
carteira, monta a fila de cobrança da semana e rascunha mensagens.

Regras:
- Responda em português, em tópicos curtos, com tabelas quando houver números.
- Clientes aparecem só por código. Nunca peça nem use nome, documento ou telefone.
- Nas mensagens, deixe [NOME], [CONTATO] e [ASSINATURA] em branco para a equipe completar.
- Nunca invente valor, data ou condição. Use só os dados que eu enviar e a política da casa.
- Nunca ofereça desconto, parcelamento ou prazo novo que a política não permita sem aprovação.
- Marque com [CONFERIR] tudo que você deduziu ou que depende de julgamento.
- Termine sempre com: próximos passos, responsável e prazo.
- Você organiza e rascunha. Quem fala com o cliente e decide é a equipe.
```

## A política de cobrança da casa (preencha e cole)

```
Empresa: [nome] · Setor: [setor] · Sistema do contas a receber: [nome]
Faixas de atraso: [ex.: a vencer em 5 dias; 1 a 15; 16 a 30; 31 a 60; acima de 60]
Tom por faixa: [ex.: lembrete amigável até 15; firme de 16 a 30; escalada com gestor acima de 30]
Quem cobra cada faixa: [cargos]
Canais e horários: [ex.: e-mail e WhatsApp da empresa, dias úteis, das 8h às 18h]
O que a equipe pode oferecer sem aprovação: [ex.: segunda via, nova data em até 7 dias]
Quem aprova desconto, parcelamento, protesto e bloqueio de crédito: [cargo para cada um]
Clientes com prazo safra: [códigos, cultura e mês de colheita]
Clientes estratégicos (falar antes com o gestor): [códigos]
O que nunca fazer: [ex.: cobrar em grupo; ligar fora do horário; ameaçar]
```

## Os prompts

### Passo 1: as faixas de atraso

Cole: o contas a receber em aberto, com código do cliente, documento, vencimento, valor e prazo combinado.

```
Com o contas a receber abaixo, na data de hoje, [data], distribua os títulos nas faixas de atraso da política da
casa. Monte uma tabela por faixa com quantidade de títulos, quantidade de clientes e valor total. Depois, liste os
dez clientes com maior valor em atraso e diga quanto eles representam do total vencido. Separe à parte os títulos
de clientes com prazo safra.
[cole aqui]
```

O que conferir: o total da tabela bate com o total do contas a receber do sistema?

### Passo 2: quem cobrar primeiro

```
Com as faixas do passo 1, cruze valor e atraso e monte a fila de cobrança desta semana:
1. valor alto e atraso longo: contato nesta semana, pela pessoa mais experiente;
2. valor alto e atraso curto: contato rápido, antes que vire hábito;
3. valor baixo e atraso longo: mensagem padrão e indicação para decisão de quem tem alçada;
4. valor baixo e atraso curto: lembrete.
Considere "valor alto" acima de R$ [valor]. Distribua a fila entre [pessoas], com no máximo [número] contatos por
pessoa por dia. Clientes estratégicos vão primeiro para o gestor.
```

O que conferir: a fila cabe no tempo real da equipe? Há cliente estratégico na fila que precisa de conversa antes?

### Passo 3: o hábito real de pagamento

Cole: os recebimentos dos últimos 12 meses, com código do cliente, vencimento, data do pagamento e valor.

```
Com o histórico abaixo, calcule para cada cliente o atraso médio em dias, ponderado pelo valor, e compare com o
prazo combinado. Classifique cada cliente em: paga em dia; atrasa pouco e paga; atrasa sempre; piorando. "Piorando"
é quem atrasou mais nos últimos três meses do que no restante do período. Liste primeiro os clientes que pioraram,
com o atraso médio antes e depois.
[cole aqui]
```

O que conferir: o atraso de algum cliente vem de um problema nosso (nota errada, entrega com divergência, boleto
não enviado)? Isso se resolve antes de cobrar.

### Passo 4: o prazo safra

Cole: os títulos dos clientes com prazo safra, com código, vencimento, valor, cultura e situação da entrega do grão
(se houver).

```
Para os títulos com prazo safra abaixo, separe o que está vencido de verdade do que vence com a colheita. Monte um
calendário por cliente com três marcos: contato de acompanhamento [30] dias antes da colheita, confirmação da
colheita e da entrega do grão, e a data do pagamento. Aponte os clientes em que algum marco está atrasado e sugira a
pergunta a fazer, em tom de parceria.
[cole aqui]
```

O que conferir: a situação da lavoura e da entrega vem da equipe comercial ou de campo, não da IA.

### Passo 5: a mensagem no tom da casa

Informe: a faixa, o valor, o vencimento e o histórico do cliente (por código).

```
Escreva a mensagem de cobrança para o cliente [código], faixa [faixa], título de R$ [valor] vencido em [data].
Histórico: [ex.: costuma pagar em dia; já prometeu uma vez]. Faça três versões, todas curtas e respeitosas:
1. amigável: lembrete, oferece segunda via e pergunta se houve algum problema;
2. firme: informa valor e vencimento, pede uma data de pagamento até [dia];
3. escalada: assinada pelo gestor, informa os próximos passos previstos na política, sem ameaça.
Faça a versão para WhatsApp (até cinco linhas) e a versão para e-mail (com assunto). Deixe [NOME], [CONTATO] e
[ASSINATURA] em branco.
```

O que conferir: o tom combina com a relação que a empresa tem com esse cliente? Leia antes de enviar.

### Passo 6: as promessas de pagamento

Cole: as promessas registradas na semana passada (código, valor prometido, data, quem recebeu, canal) e os
recebimentos da semana.

```
Compare as promessas de pagamento abaixo com os recebimentos da semana. Classifique cada promessa em cumprida,
cumprida em parte ou não cumprida. Para quem não cumpriu, sugira o próximo contato conforme a política da casa. Quem
tiver duas promessas não cumpridas sobe uma faixa de tom e vai para o gestor.
[promessas]
[recebimentos]
```

O que conferir: o recebimento identificado é mesmo daquele cliente? Pix sem identificação precisa de confirmação.

### Passo 7: a rotina de segunda

Cole: o contas a receber em aberto atualizado, os recebimentos da semana e as promessas registradas.

```
Faça a rotina de cobrança desta segunda, [data]:
1. atualize as faixas de atraso e compare com a semana passada;
2. monte a fila da semana, por pessoa;
3. liste as promessas vencidas e as não cumpridas;
4. aponte os clientes que pioraram o hábito de pagamento;
5. lembre os marcos de prazo safra da semana;
6. escreva um resumo de cinco linhas para o gestor, com os casos que pedem decisão dele.
[cole aqui]
```

O que conferir: o resumo para o gestor traz só o que precisa de decisão, com valor e prazo.

### Passo 8: a decisão com gente

```
Para os clientes abaixo, que estão acima de [dias] de atraso, organize as informações para a decisão do [cargo]:
valor, atraso, hábito de pagamento, promessas não cumpridas, contatos já feitos e importância comercial (informada
por mim). Liste as alternativas previstas na política (novo prazo, parcelamento, desconto, protesto, bloqueio de
crédito, cobrança judicial) com os prós e contras de cada uma. Não recomende uma alternativa: só organize.
[cole aqui]
```

O que conferir: a decisão fica registrada com o nome de quem aprovou, no sistema da empresa.

## Quando o kit não basta

Aqui a IA organiza o que você cola toda semana. Numa empresa com cérebro completo, a IA já conhece a política de
cobrança, o histórico de cada cliente e o calendário da safra, lê o contas a receber direto do sistema e entrega a
fila da segunda pronta, com controle do que faz. É o que a JCE monta com as empresas.

- **Quer ver como ficaria na sua empresa?** Fale com a JCE: https://jcefin.com.br
- **Siga Fabrício Escossi no LinkedIn** para receber os próximos kits: https://www.linkedin.com/in/fabricioescossi
- **Assine a newsletter "A Era dos Super-Humanos"**, com inteligência artificial para quem decide, duas vezes por
  semana, no perfil do LinkedIn.
