# Kit: os 12 indicadores do sócio

Por Fabrício Escossi · JCE Consultoria · versão 1, novembro de 2026

Este arquivo leva para a sua IA a folha de cola do post "Os 12 indicadores que o sócio precisa entender". Ele traz
as fórmulas, a conta do balancete que entra em cada uma e um prompt que calcula e explica os 12 a partir do
balancete. Funciona no ChatGPT, no Claude, no Copilot e no Gemini.

## Como usar, em 4 passos

1. **Crie um espaço fixo na sua IA** chamado "Indicadores do sócio":
   - ChatGPT ou Claude: um Projeto;
   - Gemini: um Gem;
   - Copilot: um Notebook, ou anexe este arquivo no início de cada conversa.
2. **Cole o bloco "Instruções para a IA"** e a seção "As 12 fórmulas" nas instruções fixas.
3. **Preencha a ficha "Sobre a nossa empresa"** e cole logo abaixo. É ela que diz à IA quais contas do seu plano de
   contas entram em cada fórmula.
4. **Todo mês, depois do fechamento, rode os prompts.** Primeiro o cálculo, depois a leitura para o sócio. Na
   primeira vez, rode também o mapa das contas.

## Cuidados com os dados (leia antes)

- Use a versão corporativa da ferramenta e confira a política de dados da empresa.
- Cole o balancete, não o razão. O balancete não traz nome de cliente, funcionário ou fornecedor; se o seu trouxer
  contas com nome de pessoa, troque por código antes.
- Indicador calculado com balancete não fechado engana. Use o balancete do mês já fechado.
- Confira as contas com o contador na primeira vez. Cada plano de contas agrupa as despesas de um jeito.
- A IA prepara a leitura. A decisão continua com o sócio.

## Instruções para a IA (copie e cole)

```
Você é assistente da controladoria da empresa descrita em "Sobre a nossa empresa". Todo mês você calcula e explica
12 indicadores para os sócios, a partir do balancete.

Regras:
- Responda em português, direto, em linguagem de quem decide, sem jargão contábil sem explicação.
- Use só as fórmulas da seção "As 12 fórmulas" e só os números que eu enviar.
- Para cada indicador, mostre a conta: quais linhas do balancete entraram e com que valor.
- Nunca invente valor. Se faltar uma conta ou um dado (por exemplo, compras do período), diga o que falta e peça.
- Marque com [CONFERIR] tudo que for estimativa, aproximação ou classificação sua de uma conta.
- Os indicadores de prazo usam o número de dias do período informado. Não misture mês com acumulado do ano.
- Não dê nota de "bom" ou "ruim" sem referência. Compare com o mês anterior, com o orçamento ou com a meta da ficha.
- Você prepara. Quem conclui e decide é o sócio.
```

## Sobre a nossa empresa (preencha e cole)

```
Empresa: [nome] · Setor: [setor] · Unidades: [quantas]
Sistema oficial (ERP): [nome] · Balancete: [mensal / acumulado no ano]
Quem fecha o balancete: [cargo ou escritório] · Até o dia: [dia útil]
Custos e despesas variáveis (contas): [ex.: custo da mercadoria, fretes de venda, comissões]
Custos e despesas fixas (contas): [ex.: folha administrativa, aluguel, sistemas]
Empréstimos e financiamentos (contas): [curto e longo prazo]
Metas ou limites combinados: [ex.: dívida líquida até 2 vezes o EBITDA; prazo de recebimento até 45 dias]
Sazonalidade: [ex.: estoque alto de março a junho por causa da safra]
Termos da casa: [ex.: saca, romaneio, safra e safrinha]
```

## As 12 fórmulas (copie e cole junto com as instruções)

```
O RESULTADO
1. Margem bruta = (receita líquida - custo do que foi vendido) / receita líquida
   Pergunta: o preço paga o que eu vendo?
2. Margem de contribuição = (receita líquida - custos e despesas variáveis) / receita líquida
   Variáveis são os que sobem e descem com a venda: mercadoria, frete de venda, comissão.
   Pergunta: qual produto ou cliente ajuda mais a pagar a estrutura?
3. EBITDA = resultado operacional (antes de juros e de imposto de renda e contribuição social)
   + depreciação e amortização
   Pergunta: a operação se paga, antes de juros e impostos?
4. Ponto de equilíbrio (em receita) = custos e despesas fixos / margem de contribuição em %
   Pergunta: quanto preciso vender por mês para não ter prejuízo?

OS PRAZOS (em dias; "dias" = número de dias do período, por exemplo 30 no mês ou 360 no ano)
5. Prazo médio de recebimento = contas a receber de clientes / receita bruta do período x dias
   Pergunta: estou financiando o cliente?
6. Prazo médio de pagamento = fornecedores / compras do período x dias
   Se não houver compras no relatório: compras = custo do que foi vendido + estoque final - estoque inicial
   Pergunta: quem financia a minha compra?
7. Giro de estoque = custo do que foi vendido no período / estoque médio
   Em dias: estoque médio / custo do que foi vendido x dias
   Pergunta: tem dinheiro parado no armazém ou na prateleira?
8. Ciclo de caixa = prazo de estoque em dias + prazo de recebimento - prazo de pagamento
   Pergunta: quanto tempo fico descoberto entre pagar e receber?

O FÔLEGO
9. Geração de caixa da operação (aproximada) = EBITDA
   - aumento do capital de giro no período (ou + redução)
   - imposto de renda e contribuição social pagos
   Pergunta: o lucro virou dinheiro?
10. Capital de giro (necessidade) = (contas a receber + estoques + adiantamentos a fornecedores)
    - (fornecedores + salários e impostos a pagar + adiantamentos de clientes)
    Pergunta: crescer vai pedir quanto de caixa?
11. Dívida líquida sobre EBITDA = (empréstimos e financiamentos de curto e longo prazo - caixa e aplicações)
    / EBITDA dos últimos 12 meses
    Pergunta: em quantos anos a operação pagaria a dívida? A dívida está pesada?
12. Cobertura de juros = EBITDA do período / despesas com juros do mesmo período
    (versão mais conservadora: use o resultado operacional, sem somar a depreciação)
    Pergunta: os juros cabem no resultado?
```

Exemplo ilustrativo do ponto de equilíbrio: uma empresa com R$ 300 mil de custos fixos por mês e margem de
contribuição de 30% precisa vender R$ 1 milhão por mês para não ter prejuízo (300 mil / 0,30).

## Os prompts

### Só na primeira vez: o mapa das contas

Cole: o balancete do último mês fechado e a ficha da empresa.

```
Com o balancete abaixo, monte o mapa das contas para as 12 fórmulas: para cada componente (receita líquida, custo
do que foi vendido, custos variáveis, custos fixos, depreciação, contas a receber, estoques, fornecedores,
empréstimos, caixa, juros), liste as contas do balancete que entram nele. Marque com [CONFERIR] toda conta que você
classificou por dedução, e liste no fim as contas que você não soube onde colocar.
[cole o balancete]
```

O que conferir: a classificação de cada conta, com o contador. Depois de aprovado, guarde o mapa no espaço fixo da
IA; ele vale para todos os meses.

### Todo mês: o cálculo dos 12

Cole: o balancete do mês fechado, o do mesmo mês do período anterior (ou o do início do ano) e o mapa das contas.

```
Com os balancetes abaixo, o mapa das contas e as 12 fórmulas, calcule os 12 indicadores do mês [mês/ano]. Monte uma
tabela com: indicador, valor deste período, valor do período anterior, variação e a conta feita (linhas e
valores usados). Para a dívida líquida sobre EBITDA, use o EBITDA dos últimos 12 meses; se não houver os 12 meses,
diga e pare. Liste no fim os dados que faltaram e as aproximações que você fez.
[cole o balancete deste período]
[cole o balancete do período anterior]
```

O que conferir: a receita líquida e o caixa batem com o que o financeiro já conhece? Se um indicador mudou muito,
confira primeiro se não foi uma conta reclassificada.

### Todo mês: a leitura para o sócio

```
Com a tabela dos 12 indicadores acima, escreva uma página para os sócios, em linguagem de quem decide:
1. Em uma frase cada, o que os três grupos dizem: resultado, prazos e fôlego.
2. Os três indicadores que mais mudaram e a causa provável de cada um, com a pergunta que eu devo fazer ao
   responsável.
3. Quais indicadores passaram das metas ou limites da ficha.
4. Duas perguntas que os sócios deveriam fazer na próxima reunião.
Não dê conselho de investimento nem conclua por mim. Marque com [CONFERIR] o que for interpretação sua.
```

O que conferir: a causa apontada pela IA é hipótese. Confirme com quem conhece a operação antes de levar à reunião.

### Quando um indicador acender: o que mexe nele

```
O indicador [nome] ficou em [valor], contra [valor anterior ou meta]. Explique, com as contas do balancete, o que
mais pesou na mudança. Depois, liste as alavancas que mexem nesse indicador (por exemplo: prazo com clientes,
compras, preço, mix, renegociação de dívida), com o efeito esperado de cada uma e o risco. Ordene da mais simples
para a mais difícil de executar.
```

O que conferir: o efeito de cada alavanca é direção, não promessa. Qualquer simulação com valores precisa ser
refeita com os números do financeiro antes de virar decisão.

## Quando o kit não basta

Aqui a IA calcula com o balancete que você cola todo mês. Com o cérebro completo da empresa e os sistemas ligados,
os 12 indicadores chegam prontos depois do fechamento, já com o mapa das contas aprovado, com as metas combinadas
pelos sócios e com o histórico das decisões tomadas por causa deles. É o que a JCE monta com as empresas.

- **Quer ver como ficaria na sua empresa?** Fale com a JCE: https://jcefin.com.br
- **Siga Fabrício Escossi no LinkedIn** para receber os próximos kits: https://www.linkedin.com/in/fabricioescossi
- **Assine a newsletter "A Era dos Super-Humanos"**, com inteligência artificial para quem decide, duas vezes por
  semana, no perfil do LinkedIn.
