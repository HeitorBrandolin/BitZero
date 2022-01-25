# BitZero
Projeto de sistema de manipulação de informações de clientes da empresa Bitzero, realizado por alunos de ESOFT da UniCesumar

## Divisão de cargos.
### Product Owner: Alan Minoru
### Scrum Master: Rodrigo Branco
### Desenvolvedores: Michelle Fregnani, Allan Ogawa, Heitor Brandolin

## Problemática

Foi solicitado a construção de um algoritmo/programa de forma modular (procedimentos e funções) em visualG, a fim de resolver o problema de uma empresa fictícia. A empresa BitZero necessita manipular algumas informações de clientes e contas a receber com os dados disponibilizados de um sistema de terceiro, dois arquivos do tipo    texto (.txt) foram gerados. O programa a ser desenvolvido, deverá efetuar a importação dos arquivos e tratar os dados para que posteriormente, possibilite consultas e alterações das informações. As informações importantes para os Clientes são CODIGO, NOME, CIDADE, ESTADO e CPF/CNPJ. As informações importantes para as Parcelas são NUMERO, CODIGO DO CLIENTE, DATA VENCIMENTO, DATA DE RECEBIMENTO (somente alguns registros possuem esta informação), VALOR e CODIGO DO BANCO.

Os códigos de bancos são:
- 0   – CARTEIRA (sem cobrança bancária)
- 001 – Banco do Brasil
- 104 – CEF - Caixa Econômica Federal
- 237 – Bradesco
- 260 - Nubank

## O sistema deverá contemplar:
- importação de Clientes e Parcelas (não permitir importar mais de uma vez)
- possibilidade de Classificar Clientes por NOME ou CODIGO
- inclusão de clientes (validar CODIGO pois não poderá haver duplicidade)
- alteração de clientes (exceto do campo CODIGO que será chave)
- exclusão de clientes (somente se não houver parcelas vinculadas a eles)
- Possibilidade de Classificar Parcelas por NUMERO ou VENCIMENTO
- inclusão de parcelas (atenção ao validar o campo NUMERO pois não poderá haver
duplicidade). Atenção também ao CODIGO do CLIENTE pois o mesmo deverá existir.
- alteração de parcelas (se alterado o campo CODIGO do CLIENTE, este deverá ser validado pois
necessita haver um código válido – cliente existente)
- exclusão de parcelas

## O sistema deverá proporcionar consultas como:
- Clientes Geral, por cidade ou estado
- Receitas em aberto (não recebidas) de um cliente específico ou todos (com dias em atraso)
- Receitas em aberto (não recebidas) de um banco específico ou todos (com dias em atraso)
- Receitas recebidas de um cliente específico ou todos
- Receitas recebidas de um banco específico ou todos
- Receitas por cliente específico (independente de recebido ou não)
- Receitas por banco específico (independente de recebido ou não)
- Resumo sintético de receitas em aberto por banco (banco a banco com o total)
- Resumo sintético de Receitas recebidas por banco (banco a banco com o total)
- Total em aberto (geral)
- Total recebido (geral)
- Total Geral (em aberto e recebidas)
Outras consultas e funcionalidades que considerarem importantes poderão ser
implementadas, e é aí que entra a contribuição intelectual e técnica de cada um.

## Algumas observações:
- O Sistema deverá conter MENU e SUBMENUS (a critério dos programadores de acordo com os
requisitos observados)
- A exclusão de um registro poderá ser LÓGICA ou FÍSICA
- Há nos arquivos, 147 clientes e 76 parcelas (os arquivos não poderão ser modificados e serão
entregues a vocês)
- Deverá haver uma opção para mostrar os créditos do programa (quem são os
desenvolvedores)
- Os campos deverão ser validados (quando possível)
- Deverá haver mensagens de erro ao usuário
- As listagens/consultas deverão possuir paradas para avanço da próxima página.
