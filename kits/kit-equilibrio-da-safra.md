# Kit: o ponto de equilíbrio da safra

Por Fabrício Escossi · JCE Consultoria · versão 1, novembro de 2026

Este arquivo leva para a sua IA a conta do post "O ponto de equilíbrio da safra, em sacas por hectare". Ele traz a
ficha da safra para preencher, a conta explicada e os prompts para calcular o equilíbrio, ver quanto da produção já
está comprometido e montar os cenários de preço e produtividade. Serve para o produtor e para quem atende produtor
(revenda, cerealista, cooperativa, consultor). Funciona no ChatGPT, no Claude, no Copilot e no Gemini.

## Como usar, em 4 passos

1. **Crie um espaço fixo na sua IA** chamado "Equilíbrio da safra":
   - ChatGPT ou Claude: um Projeto;
   - Gemini: um Gem;
   - Copilot: um Notebook, ou anexe este arquivo no início de cada conversa.
2. **Cole o bloco "Instruções para a IA"** e a seção "A conta" nas instruções fixas.
3. **Preencha "A ficha da safra"**, uma por cultura e por safra (soja e milho safrinha são fichas separadas). Os
   custos vêm do orçamento da lavoura ou das notas; os preços, da sua referência de mercado.
4. **Rode os prompts na ordem**: o equilíbrio, a produção comprometida e os cenários. Repita os cenários sempre que
   o preço ou a expectativa de colheita mudar.

## Cuidados com os dados (leia antes)

- Use a versão corporativa da ferramenta e confira a política de dados da empresa.
- Produtor, fazenda e comprador entram por código, nunca por nome, CPF ou matrícula do imóvel.
- A IA não sabe o preço da saca nem a produtividade da sua região. Ela usa o que você informar.
- Confira os custos com o agrônomo e o financeiro antes de usar a conta para vender ou travar preço.
- A IA monta os cenários. Vender, travar preço, esperar ou renegociar é decisão de quem produz.

## Instruções para a IA (copie e cole)

```
Você é assistente financeiro de uma operação agrícola descrita em "A ficha da safra". Você calcula o ponto de
equilíbrio da safra em sacas por hectare e monta cenários de preço e produtividade.

Regras:
- Responda em português, direto, com tabelas.
- Valores em reais por hectare e em sacas por hectare. Saca de 60 kg, salvo se a ficha disser outra coisa.
- Use só os números da ficha. Nunca invente preço, custo ou produtividade. Se faltar, pergunte.
- Separe sempre custeio, arrendamento, parcelas e produção comprometida. Não misture o que é custo da safra com o que
  é parcela de investimento.
- Mostre a conta de cada número.
- Marque com [CONFERIR] tudo que for estimativa ou dedução sua.
- Não recomende vender, travar preço ou esperar. Mostre o efeito de cada caminho; a decisão é do produtor.
```

## A conta (copie e cole junto com as instruções)

```
1. Equilíbrio do custeio (sacas/ha) = custeio por hectare / preço da saca
2. Arrendamento (sacas/ha) = arrendamento combinado em sacas por hectare
   (se for em reais: valor por hectare / preço da saca)
3. Parcelas da safra (sacas/ha) = parcelas de máquinas e investimentos que vencem nesta safra / área plantada
   / preço da saca
4. Equilíbrio total (sacas/ha) = 1 + 2 + 3
5. Produção esperada (sacas/ha) = produtividade esperada
6. Sobra (sacas/ha) = 5 - 4
7. Produção comprometida (sacas/ha) = (vendas antecipadas + troca de insumo por grão + outras entregas combinadas)
   / área plantada
8. Sacas livres para vender (sacas/ha) = 5 - 7 - arrendamento pago em sacas
```

Exemplo ilustrativo, só para mostrar a conta (o preço é um número redondo de exemplo, não é cotação): custeio de
R$ 6.000 por hectare e saca a R$ 100 dão 60 sacas por hectare só para pagar o custeio (6.000 / 100). Com mais 10 sacas
de arrendamento e 5 sacas de parcelas, o equilíbrio total é de 75 sacas por hectare. Se a produtividade esperada for de
80 sacas, sobram 5 sacas por hectare antes de qualquer imprevisto.

## A ficha da safra (preencha e cole)

```
Produtor ou fazenda: [código] · Região: [município ou região]
Cultura: [soja / milho / outra] · Safra: [ex.: 2026/27] · Área plantada: [hectares]
Custeio por hectare: semente R$ [ ] · adubo e corretivo R$ [ ] · defensivos R$ [ ] · operação e combustível R$ [ ]
  · colheita e frete R$ [ ] · outros R$ [ ]
Juros do custeio: R$ [ ] por hectare (se houver financiamento)
Arrendamento: [sacas por hectare] ou R$ [ ] por hectare · Área arrendada: [hectares]
Parcelas que vencem nesta safra: [bem, valor, vencimento]
Vendas antecipadas: [quantidade em sacas, preço, data de entrega]
Troca de insumo por grão: [quantidade em sacas]
Preço da saca de referência hoje: R$ [ ] · Fonte: [ ]
Produtividade esperada: [sacas/ha] · Histórico dos últimos anos: [sacas/ha por safra]
```

## Os prompts

### O ponto de equilíbrio

Cole: a ficha da safra preenchida.

```
Com a ficha da safra abaixo e a conta, calcule o ponto de equilíbrio em sacas por hectare. Monte uma tabela com:
custeio, juros do custeio, arrendamento, parcelas da safra e equilíbrio total, em reais por hectare e em sacas por
hectare. Depois, compare com a produtividade esperada e diga a sobra por hectare. Liste os itens de custo que
faltaram ou que parecem fora do padrão da própria ficha, marcados com [CONFERIR].
[cole a ficha da safra]
```

O que conferir: o custeio por hectare bate com o orçamento da lavoura e com as notas? A área usada é a plantada, não
a total da fazenda?

### Quanto da produção já está comprometido

```
Com a ficha da safra, calcule quanto da produção esperada já está comprometido: vendas antecipadas, troca de insumo
por grão e arrendamento pago em sacas. Mostre, em sacas por hectare e no total:
1. produção esperada;
2. produção comprometida, item por item, com o preço já fechado de cada um;
3. sacas livres para vender;
4. o preço médio que as sacas livres precisam alcançar para fechar a conta do equilíbrio.
Se as sacas comprometidas passarem de uma safra com quebra, avise.
```

O que conferir: as quantidades batem com os contratos e com o que a revenda ou a trading tem registrado? Contrato
com entrega obrigatória pesa mais do que expectativa de venda.

### Os cenários de preço e produtividade

```
Monte os cenários da safra numa tabela de três por três:
- preço da saca: [preço baixo], [preço de hoje] e [preço alto];
- produtividade: [com quebra], [esperada] e [acima da média], em sacas por hectare.
Para cada combinação, mostre: equilíbrio em sacas por hectare, sobra ou falta por hectare e o resultado total da área.
Lembre que as sacas comprometidas já têm preço fechado: só as sacas livres mudam com o preço.
Depois, diga em quais combinações a safra não se paga e o que mais pesa nelas.
```

O que conferir: os preços e as produtividades dos cenários são seus, não da IA. Use o histórico da propriedade e uma
referência de preço que você confie.

### Antes de decidir: o que cada caminho muda

```
Com os cenários acima, mostre o efeito de cada caminho no equilíbrio e nas sacas livres: travar preço de parte das
sacas livres agora, esperar para vender depois da colheita, renegociar o prazo das parcelas, reduzir algum item do
custeio ainda não comprado. Para cada um, diga o que melhora, o que piora e o risco. Não recomende nenhum: a
decisão é minha.
```

O que conferir: o efeito é uma direção, não uma promessa. Antes de travar preço ou renegociar, refaça a conta com o
financeiro e com quem compra a sua produção.

## Quando o kit não basta

Aqui a IA calcula com a ficha que você preenche a cada safra. Com o cérebro completo da empresa e os sistemas
ligados, o equilíbrio de cada talhão e de cada cultura fica atualizado conforme as notas entram e os contratos são
fechados, com o histórico das safras anteriores e das decisões de venda já tomadas. É o que a JCE monta com as
empresas.

- **Quer ver como ficaria na sua empresa?** Fale com a JCE: https://jcefin.com.br
- **Siga Fabrício Escossi no LinkedIn** para receber os próximos kits: https://www.linkedin.com/in/fabricioescossi
- **Assine a newsletter "A Era dos Super-Humanos"**, com inteligência artificial para quem decide, duas vezes por
  semana, no perfil do LinkedIn.
