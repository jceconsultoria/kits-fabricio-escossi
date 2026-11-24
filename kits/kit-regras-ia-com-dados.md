# Kit: 5 regras para usar IA com dado financeiro

Por Fabrício Escossi · JCE Consultoria · versão 1, novembro de 2026

Este arquivo leva para a sua empresa as regras do post "5 regras para usar IA com dado financeiro sem expor a
empresa". Ele traz uma política de uso de IA de uma página para você adaptar, um checklist para rodar antes de colar
qualquer dado e um prompt que revisa a planilha e aponta o que não deveria sair da empresa. Funciona no ChatGPT, no
Claude, no Copilot e no Gemini.

## Como usar, em 4 passos

1. **Adapte a política.** Preencha a ficha "Sobre a nossa empresa", cole junto com a política modelo e use o prompt
   de adaptação. Leia o resultado com quem responde por tecnologia e pelo jurídico da empresa, se houver.
2. **Aprove e divulgue.** A política vale quando um diretor aprova e a equipe recebe. Uma reunião de 20 minutos com
   o financeiro basta para explicar as cinco regras.
3. **Imprima o checklist.** Ele fica ao lado de quem exporta relatório do sistema. Se uma resposta for "não", o
   arquivo não sai.
4. **Rode o prompt revisor antes de cada envio novo.** Na primeira vez que um tipo de planilha for para a IA, peça a
   revisão. Depois que o modelo estiver limpo, basta repetir o checklist.

## Cuidados com os dados (leia antes)

- Use a versão corporativa da ferramenta e confira a política de dados da empresa. Este kit não substitui essa
  política: ajuda a escrevê-la.
- Cliente, fornecedor e funcionário entram por código, nunca por nome, CPF ou salário.
- Para o prompt revisor, cole só o cabeçalho e poucas linhas de exemplo. Se você já sabe que as linhas têm nome ou
  CPF, cole só o cabeçalho.
- A IA prepara. Aprovar a política, liberar um arquivo e enviar qualquer coisa para fora continuam sendo decisão de
  gente.

## Instruções para a IA (copie e cole)

```
Você é assistente de controles internos da empresa descrita em "Sobre a nossa empresa". Você ajuda a usar
inteligência artificial com dados financeiros sem expor a empresa, os clientes, os fornecedores ou os funcionários.

Regras:
- Responda em português, em tópicos curtos e em linguagem de quem decide, sem jargão técnico.
- Nunca invente lei, norma, número ou prazo. Se algo depende de avaliação jurídica, diga isso.
- Quando faltar informação, pergunte antes de responder.
- Marque com [CONFERIR] tudo que depende de julgamento ou que você deduziu.
- Se eu colar algo que pareça dado pessoal (nome, CPF, CNPJ de pessoa física, salário, conta bancária, endereço,
  telefone, e-mail), avise na primeira linha da resposta e não repita o dado.
- Você prepara e sugere. Nada é aprovado, divulgado ou enviado sem a minha revisão.
```

## Sobre a nossa empresa (preencha e cole)

```
Empresa: [nome ou apelido] · Setor: [setor] · Pessoas no financeiro: [quantas]
Ferramenta de IA corporativa: [ChatGPT, Claude, Copilot ou Gemini, versão empresa / ainda não temos]
Quem administra a ferramenta: [cargo]
Sistema oficial (ERP): [nome] · Onde ficam as planilhas: [pasta ou serviço]
Dados que mais circulam no financeiro: [ex.: contas a receber, folha, extrato, contratos]
Quem aprova a política: [cargo] · Quem responde por dúvidas: [cargo]
O que nunca pode sair: [ex.: folha individual, contrato de cliente, senha, dado de produtor]
```

## A política de uso de IA, em uma página (adapte)

```
POLÍTICA DE USO DE INTELIGÊNCIA ARTIFICIAL COM DADOS DA EMPRESA
[Empresa] · versão [n] · aprovada por [cargo] em [data]

1. Para que serve
Esta política diz como usar ferramentas de inteligência artificial com dados da empresa sem expor clientes,
fornecedores, funcionários ou a própria empresa. Vale para todos que trabalham com dados financeiros.

2. Ferramenta permitida
Só a ferramenta corporativa [nome], na conta da empresa. É proibido usar conta pessoal, aplicativo gratuito ou
extensão de navegador com qualquer dado da empresa.

3. Pessoas por código
Cliente, fornecedor e funcionário entram por código. Nunca colar nome, CPF, CNPJ de pessoa física, salário, conta
bancária, endereço, telefone ou e-mail pessoal.

4. Só o necessário
O arquivo leva apenas as colunas que a pergunta exige. Na dúvida, menos colunas.

5. Nunca entra
Senhas, chaves de acesso, folha individual, contratos com cláusula de sigilo, dados de saúde e qualquer item da
lista "O que nunca pode sair": [lista].

6. Revisão com nome
Todo material preparado pela IA que vá para fora do financeiro (sócios, banco, cliente, fornecedor, governo) passa
por uma pessoa, com nome, que leu e aprovou. A IA não envia, não lança e não paga.

7. Registro e conferência
Quem usou a IA anota: data, ferramenta, arquivo usado (nome e data de exportação) e para que serviu. Todo número de
uma resposta é conferido com o sistema de origem antes de ser usado.

8. Quando algo der errado
Se um dado que não deveria ter saído for colado, avise [cargo] no mesmo dia. Sem punição para quem avisa; o
objetivo é corrigir rápido.

9. Dúvidas e revisão
Dúvidas vão para [cargo]. Esta política é revista a cada [período] ou quando a empresa trocar de ferramenta.
```

### O prompt de adaptação

Cole: a ficha "Sobre a nossa empresa" preenchida e a política modelo acima.

```
Adapte a política abaixo para a nossa empresa, usando a ficha "Sobre a nossa empresa". Mantenha uma página e as
nove seções. Preencha os campos entre colchetes com o que a ficha informa e marque com [CONFERIR] o que não foi
informado. Depois da política, liste em tópicos:
1. as três situações do nosso dia a dia em que alguém tem mais chance de quebrar uma regra;
2. as perguntas que devo levar ao jurídico ou a quem cuida de tecnologia antes de aprovar.
[cole a ficha]
[cole a política]
```

O que conferir: a política ficou com uma página e linguagem que a equipe entende? Os cargos citados existem de
verdade? As perguntas ao jurídico foram respondidas antes da aprovação?

## O checklist antes de colar dados

Imprima e deixe ao lado de quem exporta relatório. Todas as respostas precisam ser "sim".

```
ANTES DE COLAR QUALQUER DADO NA IA
[ ] Estou na ferramenta corporativa, na conta da empresa?
[ ] Cliente, fornecedor e funcionário aparecem só por código?
[ ] Tirei nome, CPF, salário, conta bancária, endereço, telefone e e-mail?
[ ] O arquivo tem só as colunas que a pergunta precisa?
[ ] Não há senha, chave de acesso nem item da lista "nunca pode sair"?
[ ] Sei de qual sistema e de que data é o arquivo, e anotei no registro?
[ ] Sei quem vai revisar a resposta antes de ela ser usada?
Se alguma resposta for "não", o arquivo não sai.
```

## O prompt revisor (antes do envio)

Cole: o cabeçalho da planilha e até cinco linhas de exemplo, já na ferramenta corporativa. Se você sabe que as linhas
têm dado pessoal, cole só o cabeçalho.

```
Antes de eu usar esta planilha com você, revise-a como um auditor de controles internos. A pergunta que quero
responder com ela é: [escreva a pergunta, ex.: "quais clientes atrasaram mais de 30 dias no trimestre"].
Faça, em tabela:
1. cada coluna, com o que ela parece conter e se é dado pessoal, dado sensível da empresa ou dado neutro;
2. as colunas que não são necessárias para a pergunta e podem ser retiradas;
3. as colunas que precisam virar código antes do envio (nome, CPF, CNPJ, conta, e-mail, telefone, endereço);
4. qualquer sinal de dado que nunca deveria sair (senha, salário individual, saúde, contrato sigiloso).
No fim, diga "pode seguir" ou "não siga ainda" e, se for o segundo, o que mudar. Não repita nenhum dado pessoal que
você encontrar.
[cole o cabeçalho e as linhas de exemplo]
```

O que conferir: as colunas apontadas como pessoais saíram ou viraram código? A versão limpa passou no checklist? A
IA ajuda a enxergar, mas quem libera o arquivo é você.

### Depois de usar: o registro

Uma linha por uso, numa planilha simples do financeiro. É ela que responde, meses depois, "quem usou o quê".

```
Data | Pessoa | Ferramenta | Arquivo usado (sistema e data) | Para que serviu | Quem revisou | Conferido com a origem?
```

## Quando o kit não basta

Este kit põe as regras no papel e cria o hábito. Numa empresa com cérebro completo, as regras ficam escritas onde a
IA lê antes de responder, os agentes trabalham ligados aos sistemas com acesso só ao que precisam, e cada ação fica
registrada com quem aprovou. É o que a JCE monta com as empresas, e é como a própria JCE trabalha no dia a dia.

- **Quer ver como ficaria na sua empresa?** Fale com a JCE: https://jcefin.com.br
- **Siga Fabrício Escossi no LinkedIn** para receber os próximos kits: https://www.linkedin.com/in/fabricioescossi
- **Assine a newsletter "A Era dos Super-Humanos"**, com inteligência artificial para quem decide, duas vezes por
  semana, no perfil do LinkedIn.
