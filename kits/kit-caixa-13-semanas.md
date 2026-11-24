# Kit: projeção de caixa de 13 semanas com IA

Por Fabrício Escossi · JCE Consultoria · versão 1, novembro de 2026

Este arquivo leva para a sua IA a rotina do post "Projeção de caixa de 13 semanas com IA". Você monta uma vez e, toda
segunda, só cola os relatórios do sistema. Funciona no ChatGPT, no Claude, no Copilot e no Gemini.

## Como usar, em 4 passos

1. **Crie um espaço fixo na sua IA** chamado "Caixa 13 semanas":
   - ChatGPT ou Claude: um Projeto;
   - Gemini: um Gem;
   - Copilot: um Notebook, ou anexe este arquivo no início de cada conversa.
2. **Cole o bloco "Instruções para a IA"** nas instruções fixas.
3. **Preencha "As premissas da casa"** e cole abaixo das instruções. É o que faz a projeção parecer com a sua
   empresa.
4. **Toda segunda, rode o prompt da semana** com os três relatórios. Na primeira vez, rode também o prompt de
   comparação com a sua planilha.

## Cuidados com os dados (leia antes)

- Use a versão corporativa da ferramenta e confira a política de dados da empresa.
- Clientes e fornecedores por código, nunca por nome.
- A IA monta a partir do que você entrega: dado ruim gera projeção ruim.
- Confira o saldo inicial com o banco antes de levar qualquer número para a reunião.

## Instruções para a IA (copie e cole)

```
Você é assistente de tesouraria da empresa descrita em "As premissas da casa". Toda semana você atualiza a projeção
de caixa das próximas 13 semanas.

Regras:
- Semana começa na segunda. Valores em reais, sem centavos.
- Saída sempre em tabela: semana, saldo inicial, entradas, saídas, saldo final, folga sobre o saldo mínimo.
- Use as premissas da casa para prazos e datas. Se um dado contrariar a premissa, avise.
- Nunca invente valor. Se faltar um relatório, pergunte.
- Marque com [CONFERIR] tudo que for estimativa.
- No fim, aponte a semana mais apertada e três ações possíveis antes dela.
- Você prepara. A decisão de pagar, antecipar ou negociar é minha.
```

## As premissas da casa (preencha e cole)

```
Empresa: [nome] · Setor: [setor]
Contas bancárias consideradas: [bancos]
Saldo mínimo aceitável: R$ [valor]
Prazo médio real de recebimento: [dias] (prazo combinado: [dias])
Clientes que costumam atrasar: [códigos]
Dias de pagamento: [ex.: fornecedores às quintas; folha no 5º dia útil; impostos no dia 20]
Parcelas de empréstimos: [vencimentos e valores]
Sazonalidade: [ex.: safra de soja de fevereiro a abril; vendas maiores em dezembro]
Entradas e saídas extraordinárias previstas: [ex.: venda de máquina, distribuição de lucro]
```

## Os prompts

### Toda segunda: a projeção da semana

Cole: o saldo de cada conta (do extrato), o contas a receber em aberto e o contas a pagar em aberto, exportados do
sistema.

```
Com os relatórios abaixo e as premissas da casa, atualize a projeção de caixa das próximas 13 semanas, a partir de
segunda, [data].
1. Confira se o saldo inicial da soma das contas bate com os extratos.
2. Distribua os recebimentos pelo prazo real de cada cliente, não pelo vencimento.
3. Inclua folha, impostos, parcelas e as saídas fixas das premissas.
4. Monte a tabela das 13 semanas e um gráfico simples do saldo final.
5. Aponte a semana mais apertada e três ações possíveis antes dela.
[saldo por conta]
[contas a receber]
[contas a pagar]
```

### Toda segunda: o que mudou desde a semana passada

```
Compare a projeção desta semana com a da semana passada (abaixo). Liste as cinco maiores mudanças por semana, a causa
de cada uma (atraso de cliente, compra nova, premissa errada) e qual premissa da casa eu deveria corrigir.
[cole a projeção da semana passada]
```

### Só na primeira vez: a prova contra a sua planilha

```
Abaixo está a projeção que fazemos hoje na planilha, para as mesmas semanas. Compare com a sua, semana a semana,
mostre onde as duas divergem mais de 10% e explique por quê. Diga o que eu deveria ajustar nas premissas ou nos
relatórios para as duas convergirem.
[cole a planilha atual]
```

### Quando a semana apertada aparecer

```
A semana de [data] fica abaixo do saldo mínimo. Liste as alternativas para cobrir a diferença, com o efeito de cada
uma no caixa e o custo ou risco: cobrar antes clientes em atraso, renegociar prazo com fornecedores, antecipar
recebíveis, adiar compras ou investimentos, usar linha de crédito. Ordene da menos para a mais custosa.
```

## Quando o kit não basta

Aqui a IA projeta com o que você cola toda semana. Com o cérebro completo da empresa e os sistemas ligados, a
projeção chega pronta toda segunda, já conferida com o banco, com o histórico de quem paga em dia e com as decisões
já tomadas. É o que a JCE monta com as empresas.

- **Quer ver como ficaria na sua empresa?** Fale com a JCE: https://jcefin.com.br
- **Siga Fabrício Escossi no LinkedIn** para receber os próximos kits: https://www.linkedin.com/in/fabricioescossi
- **Assine a newsletter "A Era dos Super-Humanos"**, com inteligência artificial para quem decide, duas vezes por
  semana, no perfil do LinkedIn.
