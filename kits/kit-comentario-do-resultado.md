# Kit: 3 conferências antes de a IA comentar o resultado

Por Fabrício Escossi · JCE Consultoria · versão 1, novembro de 2026

Este arquivo leva para a sua IA a rotina do post "3 conferências antes de a IA comentar o resultado". Ele traz as
instruções fixas, uma ficha curta da sua empresa, um prompt para cada conferência e, só no fim, o prompt do
comentário aos sócios. Funciona no ChatGPT, no Claude, no Copilot e no Gemini.

## Como usar, em 4 passos

1. **Crie um espaço fixo na sua IA** chamado "Comentário do resultado":
   - ChatGPT ou Claude: um Projeto;
   - Gemini: um Gem;
   - Copilot: um Notebook, ou anexe este arquivo no início de cada conversa.
2. **Cole o bloco "Instruções para a IA"** nas instruções fixas desse espaço.
3. **Preencha a ficha "Sobre a nossa empresa"** e cole logo abaixo das instruções.
4. **Rode as três conferências, na ordem, antes de pedir o texto.** Responda às perguntas que a IA fizer e só depois
   rode o prompt do comentário.

## Cuidados com os dados (leia antes)

- Use a versão corporativa da ferramenta e confira a política de dados da empresa.
- Cliente e fornecedor entram por código, nunca por nome ou CPF. Salário individual não entra.
- Exporte só as colunas necessárias: produto, quantidade, valor, conta, data.
- A IA prepara a análise. O comentário só vai aos sócios depois que o controller conferir cada número com o
  balancete.

## Instruções para a IA (copie e cole)

```
Você é assistente da controladoria da empresa descrita em "Sobre a nossa empresa". Você ajuda a analisar o resultado
do período antes de o controller escrever o comentário aos sócios.

Regras:
- Responda em português, em tópicos curtos, com tabelas quando houver números.
- Nunca invente valor. Use só os dados que eu enviar e diga de onde veio cada número.
- Mostre as contas que você fez, para eu poder refazer.
- Quando faltar informação, pergunte antes de concluir.
- Marque com [CONFERIR] tudo que você deduziu ou que depende de julgamento.
- Não escreva o comentário aos sócios antes de eu pedir. Primeiro vêm as três conferências.
- Você prepara e sugere. Quem decide e assina é o controller.
```

## Sobre a nossa empresa (preencha e cole)

```
Empresa: [nome] · Setor: [setor] · Unidades: [quantas]
Produtos ou linhas principais: [ex.: soja, milho, armazenagem]
Unidade de volume: [ex.: saca de 60 kg, tonelada, unidade]
Períodos que comparamos: [ex.: mês contra mesmo mês do ano anterior; ano contra orçamento]
Fonte oficial do número: [sistema] · Quem fecha: [cargo] · Quem recebe o comentário: [sócios, conselho]
Eventos pontuais já conhecidos no período: [ex.: venda de máquina, acordo com cliente]
Contas estimadas todo mês: [ex.: energia, frete a pagar, comissões]
Termos da casa: [ex.: romaneio, quebra técnica, safra]
```

## Os prompts

### Conferência 1: preço, volume e mix

A receita pode mudar por três motivos, e cada um pede uma decisão diferente:

- **volume**: a empresa vendeu mais ou menos no total;
- **preço**: cada produto foi vendido mais caro ou mais barato;
- **mix**: a proporção entre produtos mudou, e um produto que vale mais por unidade perdeu espaço para outro que vale
  menos, ou o contrário.

Um exemplo simples e ilustrativo, de uma cerealista fictícia:

| Produto | Ano passado | Este ano |
|---|---|---|
| Soja | 100 mil sacas a R$ 120 = R$ 12,0 milhões | 80 mil sacas a R$ 135 = R$ 10,8 milhões |
| Milho | 50 mil sacas a R$ 60 = R$ 3,0 milhões | 70 mil sacas a R$ 60 = R$ 4,2 milhões |
| Total | 150 mil sacas, R$ 15,0 milhões | 150 mil sacas, R$ 15,0 milhões |

Volume: zero, porque o total de sacas é o mesmo. Preço: a soja subiu R$ 15 em 80 mil sacas, mais R$ 1,2 milhão.
Mix: 20 mil sacas saíram da soja (R$ 120) e foram para o milho (R$ 60), menos R$ 1,2 milhão. A receita não mudou, e
há duas notícias: o preço ajudou e a troca de produto tirou exatamente o que o preço deu.

Cole: a receita por produto nos dois períodos, com a quantidade e o preço médio (ou a receita e a quantidade).

```
Com os dados abaixo, separe a variação da receita entre [período anterior] e [período atual] em três efeitos:
1. volume: a variação da quantidade total, ao preço médio do período anterior;
2. preço: a variação do preço de cada produto, aplicada à quantidade do período atual;
3. mix: a troca entre produtos, ou seja, o que sobra da variação depois de volume e preço.
Mostre uma tabela por produto e outra com os três efeitos somados. Confira se a soma dos três é igual à variação
total da receita e mostre essa conta. Depois, explique cada efeito em uma frase, em linguagem de quem decide.
Se tiver o custo por produto, repita a análise para o resultado bruto de cada produto.
[cole aqui]
```

O que conferir: a soma dos três efeitos fecha com a variação total? Todos os produtos estão na mesma unidade de
volume? Se não estiverem, o efeito volume não tem sentido.

### Conferência 2: tirar os efeitos pontuais

Cole: os lançamentos do período acima de R$ [valor], com conta, histórico e valor, e a lista de eventos pontuais que
você já conhece.

```
Com os lançamentos abaixo, identifique os efeitos que não devem se repetir no próximo período: venda de máquina ou
imóvel, acordo ou indenização, ajuste de estoque, imposto recuperado de anos anteriores, multa, lançamento que
pertence a outro mês, reversão de valor estimado. Para cada um: conta, valor, motivo e documento de apoio.
Depois, monte uma tabela com três linhas: resultado do período, efeitos pontuais e resultado sem os efeitos
pontuais, para os dois períodos comparados. Marque com [CONFERIR] o que você classificou por dedução.
[cole os lançamentos]
[cole os eventos conhecidos]
```

O que conferir: a regra vale para os dois lados? Efeito pontual negativo sai do resultado da mesma forma que o
positivo. Cada item tem documento.

### Conferência 3: o que se esconde atrás da variação zero

Cole: o resultado por conta, e se possível por unidade ou produto, dos dois períodos e dos últimos seis meses.

```
Com os dados abaixo, procure o que uma variação pequena pode estar escondendo:
1. contas com variação total abaixo de [5]% em que as unidades ou os produtos mudaram muito em sentidos opostos;
2. contas com valor igual, ou quase igual, por três meses ou mais (possível estimativa repetida sem revisão);
3. contas que deveriam acompanhar o volume vendido e não acompanharam (ex.: frete, comissão, energia de secagem,
   embalagem).
Para cada achado, escreva uma pergunta objetiva ao responsável, sem acusar.
[cole aqui]
```

O que conferir: as estimativas repetidas foram revistas por alguém? Mande as perguntas antes de escrever o
comentário.

### Só depois: o comentário aos sócios

Cole: as respostas das três conferências, as respostas dos responsáveis e o saldo de caixa do período.

```
Com as três conferências abaixo, escreva o comentário do resultado de [período] para os sócios, em no máximo uma
página:
1. o resultado em uma frase, com e sem os efeitos pontuais;
2. o que explica a receita, separando preço, volume e mix;
3. o que a variação pequena escondia, se houver;
4. a posição de caixa e quanto do resultado virou dinheiro;
5. três decisões ou riscos para o próximo período.
Não use termo contábil sem explicar. Não traga número que não esteja nas conferências. Marque com [CONFERIR]
qualquer frase que dependa de julgamento.
[cole aqui]
```

O que conferir: todo número bate com o balancete. Você consegue explicar cada frase se um sócio perguntar. Só depois
envie.

## Quando o kit não basta

Aqui a IA analisa o que você cola, uma conferência de cada vez. Numa empresa com cérebro completo, a IA já conhece os
produtos, as contas estimadas e o histórico de efeitos pontuais da casa, lê os números direto dos sistemas e entrega
as três conferências prontas para o controller revisar, com controle do que faz. É o que a JCE monta com as
empresas.

- **Quer ver como ficaria na sua empresa?** Fale com a JCE: https://jcefin.com.br
- **Siga Fabrício Escossi no LinkedIn** para receber os próximos kits: https://www.linkedin.com/in/fabricioescossi
- **Assine a newsletter "A Era dos Super-Humanos"**, com inteligência artificial para quem decide, duas vezes por
  semana, no perfil do LinkedIn.
