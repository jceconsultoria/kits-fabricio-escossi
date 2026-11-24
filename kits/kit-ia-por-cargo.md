# Kit: a IA em cada cargo do financeiro

Por Fabrício Escossi · JCE Consultoria · versão 1, novembro de 2026

Este arquivo leva para a sua IA as rotinas do post "O que muda com a IA em cada cargo do financeiro". São três
prompts para cada cargo (controller, tesoureiro, contador e analista financeiro), com as instruções fixas, a ficha
da empresa e do cargo e, depois de cada prompt, o que conferir e o que continua sendo decisão sua. Funciona no
ChatGPT, no Claude, no Copilot e no Gemini.

## Como usar, em 4 passos

1. **Crie um espaço fixo na sua IA** com o nome do seu cargo, por exemplo "Tesouraria":
   - ChatGPT: um Projeto;
   - Claude: um Projeto;
   - Gemini: um Gem;
   - Copilot: um Notebook, ou anexe este arquivo no início de cada conversa.
2. **Cole o bloco "Instruções para a IA"** nas instruções fixas desse espaço.
3. **Preencha a ficha "Sobre a nossa empresa e o meu cargo"** e cole logo abaixo. Cinco minutos bastam.
4. **Escolha um prompt do seu cargo e use por um mês.** Um só, na rotina real. Quando ele estiver confiável, passe
   para o próximo.

## Cuidados com os dados (leia antes)

- Use a versão corporativa da ferramenta e confira a política de dados da empresa.
- Cliente, fornecedor, banco e funcionário entram por código, nunca por nome, CPF ou salário.
- Exporte só as colunas necessárias para a pergunta.
- A IA prepara. Lançamento, pagamento, negociação, assinatura e envio aos sócios continuam sendo decisão de gente.

## Instruções para a IA (copie e cole)

```
Você é assistente do financeiro da empresa descrita em "Sobre a nossa empresa e o meu cargo". Você trabalha para a
pessoa que ocupa o cargo informado na ficha e prepara o trabalho para ela decidir.

Regras:
- Responda em português, em tópicos curtos, com tabelas quando houver números.
- Nunca invente valor, taxa, norma ou prazo. Use só os dados que eu enviar e diga de onde veio cada número.
- Quando faltar informação, pergunte antes de responder.
- Marque com [CONFERIR] tudo que depende de julgamento ou que você deduziu.
- Separe sempre "o que os dados mostram" de "o que eu sugiro".
- Termine com: próximos passos, responsável e prazo.
- Você prepara e sugere. Nada é lançado, pago, assinado, negociado ou enviado sem a minha revisão.
```

## Sobre a nossa empresa e o meu cargo (preencha e cole)

```
Empresa: [nome ou apelido] · Setor: [setor] · Unidades: [quantas]
Sistema oficial (ERP): [nome] · Bancos com que trabalhamos: [códigos, ex.: Banco A, Banco B]
Meu cargo: [controller / tesoureiro / contador / analista financeiro]
A quem respondo: [cargo] · Quem aprova o meu trabalho: [cargo]
Rotinas que mais tomam o meu tempo: [até três]
Datas fixas: [fechamento, folha, impostos, safra, vencimentos grandes]
Termos da casa: [ex.: romaneio, safra, quebra técnica, adiantamento a produtor]
O que nunca fazer: [ex.: pagar sem duas aprovações]
```

## Controller

### 1. O comentário do resultado

Cole: o balancete ou DRE do mês, o do mês anterior e, se houver, o orçamento.

```
Compare o resultado de [mês] com o mês anterior e com o orçamento. Liste as variações relevantes e separe cada uma
em preço, volume, custo ou efeito pontual. Depois, rascunhe o comentário aos sócios em meia página: o resultado em
uma frase, os três motivos principais e os dois riscos do próximo mês. Marque com [CONFERIR] toda explicação que
você deduziu sem dado.
[cole aqui]
```

O que conferir: os motivos batem com o que você sabe da operação? Qual motivo pesa de verdade é decisão sua.

### 2. As perguntas aos gestores

Cole: as contas que mais variaram no mês, com o responsável de cada área.

```
Para cada conta abaixo, escreva uma pergunta objetiva ao gestor responsável, sem tom de cobrança, para entender a
variação. Agrupe as perguntas por gestor, em uma mensagem curta para cada um, e sugira um prazo de resposta antes
do fechamento.
[cole aqui]
```

O que conferir: as perguntas vão para as pessoas certas e não expõem número de outra área sem necessidade.

### 3. O mapa de riscos do fechamento

Cole: a lista de tarefas do fechamento, com responsável e o que deu errado nos últimos meses.

```
Com a lista abaixo, aponte as etapas do fechamento com mais risco de erro ou atraso. Para cada uma: o que pode dar
errado, como perceber cedo e qual conferência simples evitaria o problema. Termine com as três conferências que eu
deveria tornar obrigatórias.
[cole aqui]
```

O que conferir: as conferências sugeridas cabem na equipe que você tem? Quem as executa é você quem define.

## Tesoureiro

### 1. O caixa da semana

Cole: o saldo de cada conta (por código), o contas a receber e o contas a pagar das próximas semanas.

```
Monte o caixa das próximas [n] semanas, semana a semana, começando na segunda: saldo inicial, entradas, saídas e
saldo final. Aponte a semana mais apertada e os cinco pagamentos que mais pesam nela. Sugira três ações para
aliviar essa semana, sem decidir por mim.
[cole aqui]
```

O que conferir: o saldo inicial bate com o banco? Sem isso, nada do resto vale.

### 2. A ordem de pagamento

Cole: os pagamentos da semana, com vencimento, valor, fornecedor por código e se há multa ou desconto.

```
Organize os pagamentos abaixo em três grupos: pagar no vencimento sem discussão (impostos, folha, contratos com
multa alta), pagar no vencimento se o caixa permitir, e candidatos a negociar prazo. Para o terceiro grupo,
explique o critério e o custo de atrasar quando houver.
[cole aqui]
```

O que conferir: o critério respeita a relação com cada fornecedor? Quem decide adiar e quem avisa o fornecedor é
você.

### 3. A conversa com o banco

Cole: as linhas de crédito em uso, com taxa, prazo e garantia, e a necessidade de caixa que você identificou.

```
Prepare a minha conversa com o banco [código]. Compare as linhas abaixo em uma tabela (custo, prazo, garantia,
flexibilidade). Liste as cinco perguntas que eu devo fazer ao gerente e os pontos que posso negociar. Não recomende
uma linha: mostre o que pesa a favor e contra cada uma.
[cole aqui]
```

O que conferir: as taxas são as do contrato, não as que a IA supôs. A negociação e a escolha são suas.

## Contador

### 1. A revisão dos lançamentos

Cole: o razão do mês das contas que você quer revisar, sem nome de pessoa física.

```
Revise os lançamentos abaixo e aponte: lançamentos sem histórico claro, valores redondos ou repetidos fora do
padrão, contas com saldo de natureza invertida, lançamentos de ajuste feitos no fim do mês e possíveis duplicidades.
Para cada ponto, diga o que eu deveria verificar no documento.
[cole aqui]
```

O que conferir: cada ponto apontado foi checado no documento? A IA levanta a suspeita; a conclusão é sua.

### 2. A lista de documentos que faltam

Cole: os lançamentos do mês com indicação de documento anexado ou não.

```
Liste os lançamentos sem documento de suporte, agrupados por área responsável. Para cada área, rascunhe uma
mensagem curta pedindo os documentos, com a lista e o prazo de [data]. Ordene pelo valor, do maior para o menor.
[cole aqui]
```

O que conferir: a mensagem vai para quem de fato tem o documento, e o prazo respeita o calendário do fechamento.

### 3. O caso difícil

Cole: a descrição da operação, sem nome de cliente ou fornecedor, e as dúvidas de classificação.

```
Tenho dúvida sobre como tratar a operação abaixo. Organize o raciocínio: quais são as alternativas de
classificação, que informação decide entre elas e que perguntas eu devo fazer a quem conhece a operação. Não cite
norma ou artigo que você não tenha certeza de que existe; quando for o caso, diga apenas onde procurar.
[cole aqui]
```

O que conferir: toda referência a norma foi conferida na fonte oficial. A interpretação e a assinatura são suas.

## Analista financeiro

### 1. A base organizada

Cole: o relatório exportado do sistema, só com as colunas da análise.

```
Organize os dados abaixo para análise: padronize datas e valores, aponte linhas incompletas ou duplicadas e diga o
que você corrigiu e o que deixou como estava. Depois, sugira três cortes úteis (por período, unidade, produto ou
cliente por código) para a pergunta: [sua pergunta].
[cole aqui]
```

O que conferir: o total depois da limpeza bate com o total do relatório original?

### 2. A primeira leitura

Cole: a base organizada no passo anterior.

```
Faça a primeira leitura dos dados abaixo para a pergunta [sua pergunta]. Liste: o que os dados mostram, com o
número de apoio; o que parece estranho; e as três hipóteses que valem ser investigadas. Não tire conclusão que os
dados não sustentam.
[cole aqui]
```

O que conferir: os números citados estão na base? As hipóteses são ponto de partida; a investigação é sua.

### 3. A apresentação para quem decide

Cole: as conclusões que você validou.

```
Transforme as conclusões abaixo em uma página para o diretor: a mensagem principal em uma frase, três evidências
com número, um gráfico sugerido (que tipo e o que mostrar) e a decisão que ele precisa tomar. Linguagem simples,
sem termo técnico sem explicar.
[cole aqui]
```

O que conferir: a recomendação é sua e você consegue defendê-la sem a IA na sala.

## Quando o kit não basta

Este kit faz a IA trabalhar com o que você cola, um cargo de cada vez. Numa empresa com cérebro completo, a IA
conhece a estrutura, os sistemas e o histórico da casa, lê os números direto dos sistemas e entrega o trabalho de
cada cargo preparado, com controle do que faz e de quem aprova. É o que a JCE monta com as empresas.

- **Quer ver como ficaria na sua empresa?** Fale com a JCE: https://jcefin.com.br
- **Siga Fabrício Escossi no LinkedIn** para receber os próximos kits: https://www.linkedin.com/in/fabricioescossi
- **Assine a newsletter "A Era dos Super-Humanos"**, com inteligência artificial para quem decide, duas vezes por
  semana, no perfil do LinkedIn.
