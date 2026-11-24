# Kit: a semana de fechamento com IA

Por Fabrício Escossi · JCE Consultoria · versão 1, novembro de 2026

Este arquivo leva para a sua IA a rotina de fechamento do post "A semana de fechamento com IA, dia a dia". Ele traz
as instruções fixas, uma ficha curta da sua empresa e um prompt para cada dia da semana. Funciona no ChatGPT, no
Claude, no Copilot e no Gemini.

## Como usar, em 4 passos

1. **Crie um espaço fixo na sua IA** chamado "Fechamento do mês":
   - ChatGPT: um Projeto;
   - Claude: um Projeto;
   - Gemini: um Gem;
   - Copilot: um Notebook, ou anexe este arquivo no início de cada conversa.
2. **Cole o bloco "Instruções para a IA"** nas instruções fixas desse espaço.
3. **Preencha a ficha "Sobre a nossa empresa"** e cole logo abaixo das instruções. Cinco minutos bastam.
4. **Na semana do fechamento, rode o prompt do dia.** Cole junto o relatório indicado e confira o que a IA devolver
   antes de usar.

## Cuidados com os dados (leia antes)

- Use a versão corporativa da ferramenta e confira a política de dados da empresa.
- Cliente, fornecedor e funcionário entram por código, nunca por nome ou CPF.
- Exporte só as colunas necessárias.
- A IA prepara. Lançamento, envio aos sócios e qualquer pagamento continuam sendo decisão de gente.

## Instruções para a IA (copie e cole)

```
Você é assistente da controladoria da empresa descrita em "Sobre a nossa empresa". Você ajuda no fechamento
contábil e gerencial do mês.

Regras:
- Responda em português, em tópicos curtos, com tabelas quando houver números.
- Nunca invente valor. Use só os dados que eu enviar e diga de onde veio cada número.
- Quando faltar informação, pergunte antes de responder.
- Marque com [CONFERIR] tudo que depende de julgamento ou que você deduziu.
- Termine sempre com: próximos passos, responsável e prazo.
- Você prepara e sugere. Nada é lançado, enviado ou aprovado sem a minha revisão.
```

## Sobre a nossa empresa (preencha e cole)

```
Empresa: [nome] · Setor: [setor] · Unidades: [quantas]
Sistema oficial (ERP): [nome] · Planilhas usadas no fechamento: [quais]
Quem faz o fechamento: [cargos] · Quem aprova: [cargo]
Prazo do fechamento: até o dia [dia útil] do mês seguinte
Orçamento do ano: [existe / não existe]
Termos da casa: [ex.: romaneio, safra, quebra técnica]
O que nunca fazer: [ex.: lançar sem aprovação do controller]
```

## Os prompts da semana

### Segunda: o calendário do fechamento

Cole: a lista de tarefas do fechamento passado, com o responsável, o prazo e a data em que cada uma foi concluída de
verdade.

```
Com a lista do fechamento passado abaixo, monte o calendário do fechamento deste mês, dia a dia, com tarefa,
responsável e prazo. Aponte as tarefas que atrasaram da última vez e a causa provável, e diga quem eu preciso
lembrar primeiro. No fim, sugira duas mudanças de ordem para o fechamento andar mais rápido.
[cole aqui]
```

O que conferir: as datas propostas cabem na agenda real da equipe?

### Terça: a conciliação bancária

Cole: o extrato do banco do mês (OFX convertido em planilha, ou CSV) e o razão da conta banco no sistema.

```
Compare o extrato bancário e o razão da conta banco abaixo, do mês [mês]. Liste em uma tabela:
1. o que está no banco e não está no sistema;
2. o que está no sistema e não está no banco;
3. valores que batem na data mas não no valor.
Para cada diferença, dê a causa provável (tarifa, Pix não identificado, lançamento em duplicidade, data de
compensação) e a ação sugerida. No fim, diga o saldo conciliado e a diferença que sobra sem explicação.
[cole o extrato]
[cole o razão]
```

O que conferir: a diferença final é zero? Se não for, nada segue para os sócios.

### Quarta: as provisões

Cole: as notas recebidas depois do corte, as despesas recorrentes do mês e os contratos com pagamento fora do mês.

```
Com os dados abaixo, liste as despesas que pertencem ao mês [mês] mas ainda não foram lançadas. Para cada uma: valor,
conta sugerida, documento de apoio e se é estimativa ou valor firme. Depois, rascunhe o lançamento de provisão em
tabela (débito, crédito, valor, histórico). Marque com [CONFERIR] tudo que for estimativa.
[cole aqui]
```

O que conferir: as estimativas têm base? O lançamento só entra no sistema depois da sua aprovação.

### Quinta: o balancete comparado

Cole: o balancete do mês, o do mês anterior e, se houver, o orçamento.

```
Compare o balancete de [mês] com o mês anterior e com o orçamento. Liste as dez contas que mais mudaram, em valor e
em percentual. Para cada uma, escreva uma pergunta objetiva ao responsável, sem acusar, para entender a variação.
Separe o que parece recorrente do que parece pontual.
[cole os balancetes]
```

O que conferir: as perguntas vão para as pessoas certas? Mande antes de sexta.

### Sexta: o comentário aos sócios

Cole: o resultado do mês, o saldo de caixa e as respostas que você recebeu na quinta.

```
Escreva o comentário do resultado de [mês] para os sócios, em linguagem de quem decide e em no máximo uma página:
1. o resultado em uma frase;
2. os três maiores motivos, separando preço, volume e efeitos pontuais;
3. a posição de caixa e quanto do resultado virou dinheiro;
4. três riscos ou decisões para o próximo mês.
Não use termo contábil sem explicar. Marque com [CONFERIR] qualquer número que não veio dos dados enviados.
[cole aqui]
```

O que conferir: todo número do comentário bate com o balancete. Só depois envie.

## Quando o kit não basta

Este kit faz a IA trabalhar com o que você cola, um dia de cada vez. Numa empresa com cérebro completo, a IA conhece
a estrutura, os sistemas e o histórico da casa, lê os números direto dos sistemas e entrega o fechamento preparado,
com controle do que faz. É o que a JCE monta com as empresas.

- **Quer ver como ficaria na sua empresa?** Fale com a JCE: https://jcefin.com.br
- **Siga Fabrício Escossi no LinkedIn** para receber os próximos kits: https://www.linkedin.com/in/fabricioescossi
- **Assine a newsletter "A Era dos Super-Humanos"**, com inteligência artificial para quem decide, duas vezes por
  semana, no perfil do LinkedIn.
