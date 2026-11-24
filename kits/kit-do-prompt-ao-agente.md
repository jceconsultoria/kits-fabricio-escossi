# Kit: do prompt ao agente, em que degrau está a sua empresa

Por Fabrício Escossi · JCE Consultoria · versão 1, novembro de 2026

Este arquivo acompanha o post "Do prompt ao agente: os 3 degraus da IA na empresa". Ele traz um diagnóstico de 10
perguntas para saber em que degrau a sua empresa está, como ler o resultado e o que fazer em cada degrau, com um
prompt para dar o próximo passo. Você pode responder sozinho, em dez minutos, ou pedir para a IA conduzir a conversa.
Funciona no ChatGPT, no Claude, no Copilot e no Gemini.

Os três degraus, em resumo:

- **Degrau 1, a pessoa usa IA com prompt.** O ganho é individual e depende de quem sabe pedir.
- **Degrau 2, a empresa tem um cérebro.** Um contexto comum, escrito, que toda IA da empresa lê antes de responder.
  As respostas ficam consistentes.
- **Degrau 3, agentes fazem rotinas todo dia.** Ligados aos sistemas, com quem aprova, o que podem fazer sozinhos e
  registro do que fizeram.

## Como usar, em 4 passos

1. **Responda às 10 perguntas** com sim ou não, pensando na empresa como um todo, não só em você. Na dúvida, a
   resposta é não.
2. **Leia o resultado** com a regra da seção "Como ler o resultado". O degrau da empresa é o último em que todas as
   respostas foram sim.
3. **Faça o próximo passo do seu degrau**, e só ele. Pular degrau costuma custar caro: agente sem cérebro, ou cérebro
   sem controle.
4. **Repita o diagnóstico em três meses.** Compare as respostas e veja o que mudou.

## Cuidados com os dados (leia antes)

- O diagnóstico não precisa de nenhum dado da empresa: só sim, não e uma descrição curta. Não cole relatórios.
- Use a versão corporativa da ferramenta e confira a política de dados da empresa.
- Cliente, fornecedor e funcionário, se aparecerem, entram por código, nunca por nome, CPF ou salário.
- A IA prepara o plano. Escolher o próximo passo, quem responde por ele e o que um agente pode fazer continuam sendo
  decisão de gente.

## Instruções para a IA (copie e cole)

```
Você é assistente da direção da empresa descrita em "Sobre a nossa empresa". Você ajuda a entender em que degrau a
empresa está no uso de inteligência artificial e a planejar o próximo passo, com controle.

Os três degraus:
1. A pessoa usa IA com prompt: ganho individual.
2. A empresa tem um cérebro: contexto comum escrito, que toda IA lê; respostas consistentes.
3. Agentes ligados aos sistemas fazem rotinas todo dia, com responsável, limites e registro.

Regras:
- Responda em português, em tópicos curtos e em linguagem de quem decide, sem jargão técnico.
- Nunca invente número, prazo ou resultado esperado. Não prometa economia de tempo ou de custo.
- Quando faltar informação, pergunte antes de responder.
- Marque com [CONFERIR] tudo que você deduziu.
- Nunca recomende pular um degrau.
- Termine com: próximo passo, responsável e prazo.
- Você prepara e sugere. A decisão é da direção.
```

## Sobre a nossa empresa (preencha e cole)

```
Empresa: [nome ou apelido] · Setor: [setor] · Pessoas: [quantas] · Unidades: [quantas]
Ferramenta de IA corporativa: [qual / ainda não temos]
Quem usa IA hoje: [áreas ou cargos]
Sistema oficial (ERP): [nome] · Outros sistemas importantes: [quais]
Rotinas que mais pesam: [até três, ex.: conciliação, cobrança, fechamento]
Quem patrocina o uso de IA na direção: [cargo / ninguém ainda]
O que nunca fazer: [ex.: IA enviar mensagem a cliente sem aprovação]
```

## O diagnóstico: 10 perguntas

Responda sim ou não. Na dúvida, não.

```
DEGRAU 1: A PESSOA USA IA
1. A empresa tem uma ferramenta de IA corporativa, com política de dados, e as pessoas usam essa e não a conta
   pessoal?
2. Existe uma regra escrita sobre o que pode e o que não pode ser colado na IA (dado pessoal, cliente por código)?
3. Pelo menos uma rotina de cada área já é feita com ajuda da IA, com alguém conferindo o resultado?

DEGRAU 2: A EMPRESA TEM UM CÉREBRO
4. Existe um documento escrito com quem somos, quem decide o quê, quais sistemas valem e o vocabulário da casa?
5. Esse documento está nas instruções fixas da IA que a equipe usa, e não só numa pasta?
6. Ele tem um dono, com nome, e foi atualizado nos últimos três meses?
7. A mesma pergunta, feita por duas pessoas diferentes, recebe da IA respostas consistentes?

DEGRAU 3: AGENTES FAZEM ROTINAS
8. Existe ao menos uma rotina feita por um agente ligado a um sistema, todo dia ou toda semana, sem alguém colar
   dados à mão?
9. Cada agente tem uma pessoa responsável e uma lista escrita do que faz sozinho e do que só prepara para aprovação?
10. Tudo o que o agente faz fica registrado, e alguém confere uma amostra com regularidade?
```

## Como ler o resultado

O degrau da empresa é o último bloco em que todas as respostas foram sim. Um não num bloco de baixo vale mais que
vários sim num bloco de cima: a base vem primeiro.

- **Algum não entre 1 e 3: antes do degrau 1.** A IA já é usada, mas sem regra. O próximo passo é dar ferramenta
  corporativa e regra escrita, antes de ampliar o uso.
- **Sim de 1 a 3, algum não entre 4 e 7: degrau 1.** O ganho é individual. O próximo passo é escrever a primeira
  versão do cérebro e colocá-la nas instruções fixas da IA da equipe.
- **Sim de 1 a 7, algum não entre 8 e 10: degrau 2.** O contexto é comum. O próximo passo é escolher uma rotina
  repetitiva e de baixo risco para o primeiro agente, já com responsável, limites e registro definidos antes de
  ligar.
- **Sim nas 10: degrau 3.** O próximo passo é ampliar com o mesmo controle: uma rotina nova de cada vez, revisão
  periódica dos limites de cada agente e o cérebro sempre atualizado.

## O próximo passo, com um prompt para cada degrau

### Para quem está antes do degrau 1 ou no degrau 1: as regras e a primeira rotina

Cole: a ficha "Sobre a nossa empresa" e as respostas do diagnóstico.

```
Com a ficha e as respostas do diagnóstico abaixo, monte o plano dos próximos 30 dias para a empresa usar IA com
regra. Inclua: as cinco regras de uso que devem estar escritas, a reunião para apresentá-las à equipe e, para cada
área, uma rotina simples para começar, com quem confere o resultado. Termine com o que medir para saber se deu certo,
sem inventar meta numérica.
[cole a ficha]
[cole as respostas]
```

O que conferir: as rotinas escolhidas são de baixo risco e alguém com nome confere cada uma?

### Para quem está no degrau 1: a primeira versão do cérebro

Cole: a ficha "Sobre a nossa empresa".

```
Quero escrever a primeira versão do cérebro da empresa, com uma a duas páginas. Me entreviste, uma pergunta por
vez, sobre: quem somos, quem decide o quê, sistemas e fonte oficial do número, rotinas que mais pesam e datas fixas,
a decisão dos próximos 90 dias, o vocabulário da casa e o que nunca fazer. No fim, monte o documento com o que eu
respondi, marque as lacunas e não invente nada.
[cole a ficha]
```

O que conferir: o documento diz só o que você respondeu? Quem vai ser o dono dele e de quanto em quanto tempo ele
será revisado?

### Para quem está no degrau 2: o desenho do primeiro agente

Cole: a ficha, o cérebro da empresa e a descrição da rotina candidata.

```
Quero desenhar o primeiro agente da empresa para a rotina abaixo. Antes de qualquer coisa técnica, monte a ficha do
agente:
1. a função dele em uma frase (o que entrega do começo ao fim);
2. a pessoa responsável;
3. o que ele faz sozinho (ler, organizar, calcular, redigir) e o que só prepara para aprovação (pagar, enviar,
   apagar, alterar cadastro);
4. de quais sistemas ele lê e o que não pode acessar;
5. o que fica registrado e como o responsável confere;
6. o que ele nunca pode fazer.
Depois, aponte os três maiores riscos dessa rotina e a conferência que evita cada um.
[cole a ficha]
[cole o cérebro]
[cole a rotina]
```

O que conferir: a rotina é repetitiva e de baixo risco? Tudo que não tem volta está em "só prepara"? Se não estiver,
o agente ainda não está pronto.

### Para quem está no degrau 3: a revisão dos agentes

Cole: a ficha de cada agente em uso e as exceções ou erros dos últimos meses.

```
Revise os agentes abaixo como um auditor de controles internos. Para cada um: a função ainda faz sentido, os limites
estão claros, o registro permite saber o que ele fez e quem aprovou, e algum erro recente mostra um limite que deveria
mudar. Termine com a próxima rotina candidata a ganhar um agente e o que precisa estar no cérebro antes disso.
[cole as fichas]
[cole as exceções]
```

O que conferir: cada agente continua com um responsável ativo? Nenhum ganhou permissão que ninguém aprovou?

## Quando o kit não basta

Este kit mostra onde a empresa está e qual é o próximo passo. Subir os degraus com segurança pede um cérebro
completo, validado com a equipe e ligado aos sistemas, e agentes com função, responsável, limites e registro desde o
primeiro dia. É o que a JCE monta com as empresas, e é como a própria JCE trabalha no dia a dia.

- **Quer ver como ficaria na sua empresa?** Fale com a JCE: https://jcefin.com.br
- **Siga Fabrício Escossi no LinkedIn** para receber os próximos kits: https://www.linkedin.com/in/fabricioescossi
- **Assine a newsletter "A Era dos Super-Humanos"**, com inteligência artificial para quem decide, duas vezes por
  semana, no perfil do LinkedIn.
