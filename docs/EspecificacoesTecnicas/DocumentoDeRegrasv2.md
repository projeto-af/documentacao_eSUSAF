# Documento de Regras

# RGN001
## Permissão de acesso por funcionalidade

| Funcionalidade              | Instalador          | Administrador (ADM) | Gestor (GST) | Gestor Estabelecimento (GEST) | Farmacêutico (FAR) | Atendente (ATD) | Administrativo (ATV) |
| ----------------------------| :-----------------: | :-----------------: | :----------: | :---------------------------: | :----------------: | :-------------: | :------------------: |
| **CONTROLE DE ACESSO**      |                     |                     |              |                               |                    |                 |                      |
| **MODERAR ACESSO**          |                     |                     |              |                               |                    |                 |                      |
| Consultar Permissões Acesso | X                   | X                   | X            | X                             |                    |                 |                      |
| Atribuir Perfil             | X                   | X                   | X            | X                             |                    |                 |                      |
| Detalhar Permissões Acesso  | X                   | X                   | X            | X                             |                    |                 |                      |
| **SOLICITAR PERFIL**        |                     |                     |              |                               |                    |                 |                      |
| Consultar Meu Perfil        |                     | X                   | X            | X                             | X                  | X               | X                    |
| Solicitar Perfil            |                     | X                   | X            | X                             | X                  | X               | X                    |
| Detalhar Meu Perfil         |                     | X                   | X            | X                             | X                  | X               | X                    |
| **GERENCIAR PERFIL**        |                     |                     |              |                               |                    |                 |                      |
| Consultar Perfil            |                     |                     | X            |                               |                    |                 |                      |
| Cadastrar Perfil            |                     |                     | X            |                               |                    |                 |                      |
| Detalhar Perfil             |                     |                     | X            |                               |                    |                 |                      |
| **CONFIGURAÇÃO**            |                     |                     |              |                               |                    |                 |                      |
| **GESTÃO DE INTEGRAÇÕES**   |                     |                     |              |                               |                    |                 |                      |
| Consultar Integrações       |                     | X                   |              |                               |                    |                 |                      |
| Configurar Integrações      |                     | X                   |              |                               |                    |                 |                      |
| Detalhar Integrações        |                     | X                   |              |                               |                    |                 |                      |
| **CADASTRO DE ENTES**       |                     |                     |              |                               |                    |                 |                      |
| Consultar Ente              |                     | X                   |              |                               |                    |                 |                      |
| Cadastrar Ente              |                     | X                   |              |                               |                    |                 |                      |
| **CADASTRO**                |                     |                     |              |                               |                    |                 |                      |
| **ESTABELECIMENTO**         |                     |                     |              |                               |                    |                 |                      |
| Consultar Estabelecimento   |                     |                     | X            | X                             | X                  | X               | X                    |
| Cadastrar Estabelecimento   |                     |                     | X            |                               |                    |                 |                      |
| Editar Estabelecimento      |                     |                     | X            | X                             | X                  |                 |                      |
| Detalhar Estabelecimento    |                     |                     | X            | X                             | X                  | X               | X                    |
| **USUÁRIO SUS**             |                     |                     |              |                               |                    |                 |                      |
| Consultar Usuário SUS       |                     |                     | X            | X                             | X                  | X               | X                    |
| Cadastrar Usuário SUS       |                     |                     | X            | X                             | X                  | X               | X                    |
| Editar Usuário SUS          |                     |                     | X            | X                             | X                  | X               | X                    |
| Detalhar Usuário SUS        |                     |                     | X            | X                             | X                  | X               | X                    |
| **MOVIMENTAÇÃO**            |                     |                     |              |                               |                    |                 |                      |
| **ENTRADA**                 |                     |                     |              |                               |                    |                 |                      |
| Consultar Entrada           |                     |                     | X            | X                             | X                  | X               | X                    |
| Cadastrar Entrada           |                     |                     | X            | X                             | X                  | X               | X                    |
| Editar Entrada              |                     |                     | X            | X                             | X                  | X               | X                    |
| Detalhar Entrada            |                     |                     | X            | X                             | X                  | X               | X                    |
| **SAÍDA**                   |                     |                     |              |                               |                    |                 |                      |
| Consultar Saída             |                     |                     | X            | X                             | X                  | X               | X                    |
| Cadastrar Saída             |                     |                     | X            | X                             | X                  | X               | X                    |
| Editar Saída                |                     |                     | X            | X                             | X                  | X               | X                    |
| Detalhar Saída              |                     |                     | X            | X                             | X                  | X               | X                    |
| **REQUISIÇÃO**              |                     |                     |              |                               |                    |                 |                      |
| Consultar Requisição        |                     |                     | X            | X                             | X                  |                 |                      |
| Cadastrar Requisição        |                     |                     | X            | X                             | X                  |                 |                      |
| Editar Requisição           |                     |                     | X            | X                             | X                  |                 |                      |
| Detalhar Requisição         |                     |                     | X            | X                             | X                  |                 |                      |
| **GESTÃO DE ESTOQUE**       |                     |                     |              |                               |                    |                 |                      |
| Consultar Estoque           |                     |                     | X            | X                             | X                  |                 |                      |
| Editar Estoque              |                     |                     | X            | X                             | X                  |                 |                      |
| **RELATÓRIOS**              |                     |                     |              |                               |                    |                 |                      |
| Posição de Estoque          |                     |                     | X            | X                             | X                  | X               | X                    |
| Movimentações               |                     |                     | X            | X                             | X                  | X               | X                    |
| Dispensação / Fornecimento  |                     |                     | X            | X                             | X                  | X               | X                    |

**OBSERVAÇÃO:**  
As açoes realizadas pelos perfis de acordo com os proviégios afetam:

* Perfil Instalador e Administrador: Instância; 
* Perfil Gestor: Instância e Estabelecimento (se vinculado a um estabelecimento); 
* Perfil Gestor Estabelecimento, Farmacêutico e Atendente: Estabelecimento. 

---
# RGN002
## Recuperação de Estabelecimento de Saúde vinculados aos participantes da instância: 
O sistema deve recuperar como resultado da consulta os estabelecimentos de saúde dentre os cadastrados e vinculados aos participantes da instância, configuração prévia deste.   

---
# RGN003
## Cadastro de Estabelecimento de Saúde/CNES 
Não é permitido o cadastro de mais de um Estabelecimento de Saúde com o mesmo CNES para a mesma instância.  

---
# RGN004
## Resultado de consultas 
A grid com resultados de consultas deve ser apresentada somente após ser acidonada a opção "Consultar" e permitir a ordenação por coluna, paginação, seleção de registro por página e filtrar o resultado da consulta.   

---
# RGN005
## Gravação do Responsável pela Operação 
O sistema deve gravar a data, hora e CPF e nome do usuário que a executou qualquer ação de alteração no registro (inclusão, edição, exclusão, armazenamento, estorno, saída, análise, devolução, em preenchimento, atendimento, atendimento automático, recusa, autorização, não autorização, dispensação). 

---
# RGN006
## Hierarquia de Endereçamento 
Somente será permitido a exclusão de um endereçamento quando este não possuir endereçamentos hierarquicamente abaixo dele, sendo necessário a exclusão destes subníveis. 

---
# RGN007
## Excluir de Endereçamento 
Não será permitido a exclusão de um endereçamento físico caso este possua, vinculado a ele, produto(s) no estoque do estabelecimento. 

---
# RGN008
## Inativar Estabelecimento de Saúde 
Somente será possível inativar estabelecimentos de saúde que não possuem itens em estoque. 

---
# RGN009 (removido)
## Recuperação de dados do estabelecimento do usuário logado

---
# RGN010 (removido)
## Recuperação de perfil vinculados ao Ente/Mantenedor:

---
# RGN011 (removido)
## Busca Textual do Estabelecimento

---
# RGN012
## Solicitação de perfil acesso.
O sistema deve permitir solicitar: 

* Perfis de acesso iguais em estabelecimentos diferentes;  
* Perfis de acesso para uma UF e/ou a um Município e/ou a um Estabelecimento;  
* Perfis de acesso para UF a qual já possui permissão de acesso no Município e/ou Estabelecimento desta UF; 
* Perfis de acesso para municípios distintos na mesma UF. 

O sistema não deve permitir solicitar mais de um perfil de acesso por estabelecimento. 

---
# RGN013
## Aprovação e reativação de permissões de acesso.
Para permissões de acesso com situação: 

* “Solicitado” o sistema deve permitir aprovar ou reprovar; 
* “Aprovado” o sistema deve permitir inativar; 
* “Reprovado” ou “Inativo” o sistema não deve permitir aprovar ou reativar, sendo necessário realizar uma nova solicitação. 

---
# RGN014
## Recuperação de dados do cabeçalho 
Os dados do CNES, Nome, Município e UF, do cabeçalho (Emitido por:), devem ser recuperados do cadastro do estabelecimento do usuário logado. Já o Nome e CPF do usuário responsável pela última alteração no registro do cadastro e a data dessa ação devem ser recuperados do histórico do registro da funcionalidade em questão. 

---
# RGN015
## Recuperação do Produto 
Os campos de Produto apresentarão a lista de produtos ativos no sistema a partir da indicação do 3º caractere ou código de barras ou CATMAT Raiz, conforme as máscaras: 

* Para Medicamentos:
    * (Código de Barras)
    * Princípios ativos cadastrados para o medicamento no formato: {[(Princípio Ativo 1) (Concentração 1) (Sigla da Unidade de Medida 1)] + [(Princípio Ativo 2) (Concentração 2) (Sigla da Unidade de Medida 2)]  + ....}
    * CATMAT: (CATMAT Raiz)
    * Forma Farmacêutica: (Forma Farmacêutica)
    * Fabricante: [(CNPJ) - (Razão Social)]
 
* Para Produtos para Saúde e Equipamentos:
    * (Descrição do produto CATMAT)
    * CATMAT: (CATMAT Raiz)

---
# RGN016
## Exclusão de um registro 
As exclusões permitidas no sistema sempre serão lógicas, sendo necessário manter o histórico temporal da existência do registro. Exceto para registro(s) na situação “Em preenchimento” a qual deve ser física e para todos os seus descendentes.   

---
# RGN017
## Estorno de entrada de produto(s) 
O sistema não deve permitir estornar uma entrada se ao menos um do(s) produto(s) vinculado(s) a ela foi movimentado, ou seja, distribuído, dispensado ou uma saída diversa foi registrada no estoque. 

---
# RGN018
## Registro de Saída por Estorno de entrada de produto(s)
A realizar o estorno da entrada do(s) produto(s), o sistema deve: 

* Debitar o(s) produto(s) do estoque do estabelecimento da entrada estornada, através da criação de um registro de saída, gravando as seguintes informações: 
    * Tipo de Saída = “Saída por Estorno de Entrada”;  
    * Fornecedor = CNES ou CNPJ do estabelecimento que realizou entrada; 
    * Tipo de Documento = “Estorno de Entrada”; 
    * Número do Documento = Número da entrada que foi estornada; 
    * Produto, recupera os dados conforme gravado na entrada contendo: 
        * Princípio ativo 
        * Forma farmacêutica 
        * Fabricante 
        * Lote 
        * Validade 
        * Valor Unitário 
        * Quantidade  
    * Situação do registro de saída como “Registrada”; 
* Alterar a situação do registro da entrada para “Estornada”.

---
# RGN019
## Atualização de estoque após estorno de entrada 
O sistema, identificando que uma entrada de produto(s) foi estornada, deve debitar a quantidade do saldo deste(s), considerando o lote e validade e atualizar a posição de estoque do estabelecimento que realizou o estorno da entrada. 

---
# RGN020
## Consultar Razão Social no CNES ou Receita Federal do Brasil (RFB)
O sistema deve consultar: 

* A razão social no cadastro de estabelecimentos a partir da indicação do número do CNES. 
* A razão social na RFB a partir da indicação do número do CNPJ. 

---
# RGN021
## Retorno do Nome do Estabelecimento

* Ao consultar o nome através do CNES, o sistema deve retornar o nome do estabelecimento cadastrado na base de dados do CNES. Caso a consulta retorne vazia, considerar o campo “Nome Empresarial”. 
* Ao consultar o nome através do CNPJ, o sistema deve retornar a razão social da pessoa jurídica através da consulta à base da RFB.


---
# RGN022 (removido)
## Verificação de Código de Barras  

---
# RGN023
## Apresentação e validação do Produto
Para a apresentação e/ou validação de produtos, o sistema deverá seguir as máscaras abaixo: 

* Para Medicamentos com forma farmacêutica em estado “Semissólidas” ou “Gasosa” ou “Líquida” (no cadastro de medicamentos): 
    * (Código de Barras)
    * Princípios ativos cadastrados para o medicamento no formato: {[(Princípio Ativo 1) (Concentração 1) (Sigla da Unidade de Medida 1)] + [(Princípio Ativo 2) (Concentração 2) (Sigla da Unidade de Medida 2)]  + ....}
    * CATMAT: (CATMAT Raiz + Unidade CATMAT)
    * Forma Farmacêutica: (Forma Farmacêutica) - (Volume) (Unidade de Medida)
    * Fabricante: (CNPJ) - (Razão Social)
 
* Para Medicamentos com forma farmacêutica em estado “Sólidas” (no cadastro de medicamentos):
    * (Código de Barras)
    * Princípios ativos cadastrados para o medicamento no formato: {[(Princípio Ativo 1) (Concentração 1) (Sigla da Unidade de Medida 1)] + [(Princípio Ativo 2) (Concentração 2) (Sigla da Unidade de Medida 2)]  + ....}
    * CATMAT: (CATMAT Raiz + Unidade CATMAT)
    * Forma Farmacêutica: (Forma Farmacêutica) - (Volume) (Unidade de Medida)
    * Fabricante: (CNPJ) - (Razão Social)
 
* Para Produtos para Saúde (no cadastro de produtos): 
    * (Descrição CATMAT)
    * CATMAT: (CATMAT)

---
# RGN024
## Restringir Campos da Entrada de Produto para Tipo de Movimentação
* No campo “Tipo de Movimentação”, caso o usuário selecione:
    * “Saldo de Implantação” ou “Ajuste de Estoque”, os campos abaixo deixam de ser obrigatórios:
        * “Modalidade de Licitação”
        * “CNES/CNPJ” (fornecedor)
        * “Razão Social” (fornecedor)
        * “Tipo de Documento”
        * “Número do Documento”
        * “Data do Documento”
    * “Produção Própria”, os campos abaixo deixam de ser obrigatórios:
        * “Tipo de Documento”
        * “Número do Documento”
        * “Data do Documento” 

---
# RGN025
## Exclusão de produto na entrada 
Somente será permitida a exclusão de um produto adicionado à entrada se não houver nenhum detalhamento vinculado a ele. 

---
# RGN026
## Cálculo do Valor do Documento na Entrada do Produto 
O sistema deve calcular o Valor do Documento, somando todos os valores totais dos produtos adicionados à entrada. 

---
# RGN027
## Cálculo do Valor Total da Entrada para o Produto 
O sistema deve calcular o Valor Total da Entrada, pela fórmula:  Qtd Total Recebida X Valor Unitário do produto. 

---
# RGN028
## Arredondamento de Valores
Para fins de arredondamento de valores, o sistema deve:    

* Quando o algarismo a ser conservado for seguido de algarismo inferior a 5, o algarismo a ser conservado permanece sem alteração. Exemplo: 4,303 arredondado em duas casas decimais torna-se 4,30; 
* Quando o algarismo a ser conservado for seguido de algarismo superior ou igual a 5 seguido de um algarismo diferente de zero, soma-se uma unidade ao algarismo a ser conservado. Exemplo: 15,4875 arredondado em duas casas decimais torna-se 15,49; 
* Quando o algarismo a ser conservado for ímpar, seguido de 5 e posteriormente de zeros, soma-se uma unidade ao algarismo a ser conservado. Exemplo: 25,7750 arredondado em duas casas decimais fica 25,78; 
* Quando o algarismo a ser conservado for par, seguido de 5 e posteriormente de zeros, o algarismo a ser conservado permanece sem alteração. Exemplo: 31,7250 arredondado em duas casas decimais fica 31,72.  
 
---
# RGN029
## Validar Entrada do Produto
O sistema deve validar se já existe uma entrada com o mesmo tipo, número de documento e fornecedor de uma entrada armazenada ou em preenchimento para o estabelecimento.  

---
# RGN030
## Número de Registro da Entrada
Ao salvar uma entrada de produtos, caso ainda não exista, o sistema deve gerar um número identificador único para a entrada e apresentá-lo ao usuário.  

---
# RGN031
## Atualização de estoque após armazenar uma entrada
O sistema, identificando que uma entrada de produto(s) foi armazenada, deve creditar a quantidade no saldo deste(s), considerando o lote, validade e programa de saúde e atualizar a posição de estoque do estabelecimento que realizou a entrada. 

---
# RGN032
## Registro de Entrada por Estorno de Saída de produto(s)
Ao realizar o estorno da saída do(s) produto(s), o sistema deve:

* Creditar o(s) produto(s) no estoque do estabelecimento da saída estornada, através da criação de um registro de entrada, gravando as seguintes informações: 
    * Modalidade de Licitação = “Saída ”;
    * Tipo de Movimentação = “Entrada por Estorno de Saída";  
    * Fornecedor = CNES ou CNPJ do estabelecimento que realizou saída;  
    * Tipo de Documento = “Estorno de Saída ”;  
    * Número do Documento = Número da saída que foi estornada; 
    * No detalhamento do produto:  
        * Princípio ativo ou Descrição do produto 
        * Concentração + Forma farmacêutica (se for medicamento) 
        * CATMAT 
        * Fabricante 
        * Lote 
        * Validade 
        * Valor Unitário 
        * Quantidade  
    * Estado do registro de entrada como “Ativo”; 
    * Situação do registro de entrada como “Armazenada”; 
* Manter o estado do registro da Saída como “Ativo”; 
* Alterar a situação do cadastro da saída para “Estornada”

---
# RGN033
## Atualização de estoque após estorno de saída
O sistema, identificando que uma saída de produto(s) foi estornada, deve creditar a quantidade no saldo deste(s), considerando o lote, validade e programa de saúde e atualizar a posição de estoque do estabelecimento que realizou o estorno da saída.  

---
# RGN034
## Apresentação de Lotes/Validades do produto

* Quando o tipo de saída for "Distribuição sem Requisição", “Requisição”, "Usuário SUS não Identificado", o sistema deve permitir incluir produtos com estoque igual a O (zero).
* Quando o tipo de saída for “Validade Vencida”, somente serão considerados os lotes com a data de validade inferior a data atual ou com vencimento nos próximos 90 dias.
* Quando o tipo de saída for “Ajuste de Estoque”, ““Apreensão Sanitária”, “Distribuição sem Requisição”, “Empréstimo”, “Requisição”, “Saída para Departamento”, “Transferência” ou “Usuário SUS Não Identificado”, somente serão considerados os lotes com a data de validade igual ou superior a data atual. 
* Quando o tipo de saída for “Amostra”, “Exposição e Análise”, “Perda” ou “Roubo”, serão considerados todos os lotes, independente da data de validade.

---
# RGN035
## Exclusão de produto na saída
Somente será permitida a exclusão de um produto adicionado à saída se não tiver nenhum detalhamento vinculado a ele.  

---
# RGN036
## Saldo Estoque Atual
O sistema deve carregar e apresentar o saldo do produto em estoque, no momento, do estabelecimento logado, independente de lote, /validade, /programa de saúde e endereçamento físico. 

---
# RGN037
## Cálculo da Quantidade Total Recebida na Entrada do Produto
O sistema deve calcular a Quantidade Total Recebida somando todas as quantidades informadas nos detalhamentos adicionados ao produto.  

---
# RGN038
## Cálculo do Valor Total da Saída
O sistema deve calcular o Valor Total da Saída somado todos os valores totais dos produtos adicionados à saída.  

---
# RGN039
## Cálculo da Quantidade Total a Expedir da Saída por Produto
O sistema deve calcular a Quantidade a Expedir da Saída somando todas as quantidades a expedir informadas nos detalhamentos adicionados ao produto. 

---
# RGN040
## Cálculo da Média do Valor Unitário do Produto
O sistema deve calcular o Valor Unitário do Produto através da média simples dos valores unitários do produto informados na(s) entrada(s), independente de Nº do Lote, Validade, Fabricante, Programa de Saúde e Endereçamento Físico, ou seja, realiza-se o somatório de todos os elementos do rol e divide-se essa soma pela quantidade de elementos. 

---
# RGN041
## Cálculo do Valor Total da Saída para o Produto
O sistema deve calcular o Valor Total da Saída pela fórmula:  Quantidade Expedida da Saída X Valor Unitário do produto (média simples dos valores unitários informados na entrada do referido produto).

---
# RGN042
## Produto da Saída
O sistema deve permitir apenas saída de produtos que possuem estoque no estabelecimento logado, exceto se no campo “Tipo de Saída” for selecionada a opção: "Distribuição sem Requisição" ou “Requisição” ou "Usuário SUS não Identificado". 

---
# RGN043
## Quantidade Expedida do Produto
O sistema somente deve permitir informar uma quantidade expedida menor ou igual ao estoque disponível do produto, lote, validade, programa de saúde e endereçamento físico no estabelecimento logado. 

---
# RGN044
## Validar Saída do Produto
O sistema deve validar se já existe uma Saída com o mesmo tipo de Saída, tipo e número de documento e justificativa de uma Saída registrada ou em preenchimento para o estabelecimento. 

---
# RGN045
## Número de Registro da Saída
Ao salvar uma Saída de produtos, caso ainda não exista, o sistema deve gerar um número identificador único para a Saída e apresentá-lo ao usuário. 

---
# RGN046
## Atualização de estoque após registrar uma Saída
O sistema, identificando que uma Saída de produto(s) foi registrada, deve debitar a quantidade no saldo deste(s), considerando o lote, validade, programa de saúde e endereçamento físico e atualizar a posição de estoque do estabelecimento que realizou a Saída.

---
# RGN047
## Validade do token de recuperação de senha
O tempo de validade do token gerado para recuperação de senha é de 20 minutos.

---
# RGN048
## Recuperação de dados do estabelecimento do usuário logado
Os dados de UF, Município e Estabelecimentos devem ser recuperados do cadastro do estabelecimento vinculado ao perfil do usuário logado.

---
# RGN049
## Cadastro de Ente 
O sistema não deve permitir o cadastro de um ente:
    - Com o mesmo CNPJ;
    - Com a mesma UF e/ou Município na mesma esfera de gestão;

---
# RGN050
## Gerenciar perfil 
O sistema não deve permitir editar e inativar perfis do tipo “Padrão” e do tipo “Personalizado” que estão atribuídos ao cadastrado de ao menos um usuário do sistema. 

---
# RGN051
## Cadastro de Perfil 
O sistema não deve permitir o cadastro de um perfil com a mesma descrição de um perfil já cadastrado para a instância. 

---
# RGN052
## Recuperação e apresentação das permissões de acesso
O sistema deve apresentar as ações observando o perfil solicitado e a situação do registro conforme: 

* Para perfil “Instalador” a opção “Detalhar” para todas as permissões de acesso, inclusive as dos perfis personalizados; 
* Para perfil “Administrador”: 
    * A opção “Inativar” para permissões de acesso com perfil “Administrador” e “Gestor” atribuídos por ele; 
    * A opção “Detalhar” para todas as permissões de acesso, inclusive as dos perfis personalizados. 
* Para perfil “Gestor”: 
    * As opções “Aprovar”, “Reprovar” e “Inativar” para todas as permissões de acesso exceto do perfil de “Administrador”; 
    * A opção “Detalhar” para todas as permissões de acesso, inclusive as dos perfis personalizados. 
* Para perfil “Gestor Estabelecimento”: 
    * As opções “Aprovar”, “Reprovar” e “Inativar” para todas as permissões de acesso relacionadas ao seu estabelecimento; 
    * A opção “Detalhar” para todas as permissões de acesso, inclusive as dos perfis personalizados. 
* Para registro com situação “Aguardando Aprovação”, as opções “Aprovar”, “Reprovar” e “Detalhar”;  
* Para registro com situação “Aprovado”, as opções “Inativar” e “Detalhar”; 
* Para registro com situação “Reprovado” ou “Inativo”, a opção “Detalhar”.  

---
# RGN053
## Inclusão justificativa 
Ao solicitar ou reprovar ou inativar uma solicitação de permissão de acesso ao sistema, o usuário deve informar obrigatoriamente uma justificativa. 

---
# RGN054
## Atribuição de perfil de acesso 
O sistema deve permitir a atribuição de perfis conforme: 

* Usuário com perfil de “Instalador” atribui somente perfil de “Administrador”; 
* Usuário com perfil de “Administrador” atribui perfil de “Administrador” e “Gestor”; 
* Usuário com perfil de “Gestor” atribui qualquer perfil cadastrado e ativo, exceto perfil de “Administrador; 
* Usuário com perfil de “Gestor Estabelecimento” atribui qualquer perfil de acesso para seu estabelecimento; 
* Perfis de acesso iguais para o mesmo usuário em estabelecimentos diferentes;  
* Vincular perfis de acesso a uma UF e/ou a um Município e/ou a um Estabelecimento;  
* Para UF as quais o usuário já possua perfil de acesso no Município ou Estabelecimento desta UF; 
* Para municípios distintos na mesma UF para o mesmo usuário; 
* À um usuário que ainda não possui cadastro para acesso ao sistema.  

O sistema não deve permitir atribuir mais de um perfil de acesso por estabelecimento. 

---
# RGN055
## Indicação de estabelecimento na atribuição de perfil de acesso 
~~Para atribuição de perfil de acesso é obrigatória a indicação de um estabelecimento exceto para os perfis de “Administrador” e “Gestor”.~~

---
# RGN056
## Indicação de estabelecimento na solicitação de perfil de acesso 
Para solicitações de acesso é obrigatória a indicação de um estabelecimento exceto para os perfis de “Gestor”. 

---
# RGN057 - REMOVIDA

---
# RGN058
## Emissão do Relatório de Posição de Estoque 
Caso o usuário não informe nenhum filtro de pesquisa, o sistema deve considerar todas as opções ao gerar o relatório. Exceto para usuários com perfil de “Gestor” que desejam emitir a posição de estoque de todos os estabelecimentos de sua instância, que deve indicar ao menos um produto.

---
# RGN059
## Cálculo do Valor Total do Produto em estoque 
O sistema deve calcular o Valor Total do Produto em estoque somando os valores totais de cada detalhamento do produto. 

---
# RGN060
## Cálculo da Quantidade Total do Produto em estoque 
O sistema deve calcular a Quantidade Total do Produto em estoque somando as quantidades em estoque no detalhamento de cada produto.

---
# RGN061
## Cálculo do Valor Total de cada detalhamento do Produto em estoque 
O sistema deve calcular o Valor Total de cada detalhamento do Produto em estoque pela fórmula: Qtd Estoque X Valor Unitário do produto (média simples dos valores unitários informados na entrada do produto). 

---
# RGN062
## Recuperação de Usuários SUS vinculados à instância 
O sistema deve recuperar como resultado da consulta o(s) Usuário(s) SUS dentre os cadastrados e vinculados à instância. 

---
# RGN063
## Cadastro de Usuário SUS 
Não será permitido o cadastro de mais de um usuário SUS com o mesmo CPF. 

---
# RGN064
## Validação do Estabelecimento de Destino 
O CNES/CNPJ do Estabelecimento de Destino informado no registro da saída deve ser diferente do CNES/CNPJ do Estabelecimento logado. 

---
# RGN065
## Preenchimento e habilitação dos campos na Saída conforme Tipo de Saída  
* Quando o usuário selecionar no campo “Tipo de Saida” a opção: Ajuste de Estoque, Amostra, Exposição e Análise, Apreensão Sanitária, Perda, Usuário SUS Não Identificado, Validade Vencida, o sistema deve preencher os campos “CNES/CNPJ do Estabelecimento de Destino" e "Estabelecimento de Destino” com os dados do estabelecimento logado e mantendo-os desabilitados para edição e desabilitar para edição o campo: “Departamento de Destino”;  
* Quando o usuário selecionar no campo “Tipo de Saida” a opção: "Distribuição sem Requisição" ou “Empréstimo” ou “Requisição” ou "Transferência", o sistema deve habilitar e tornar obrigatório o preenchimento dos campos "CNES/CNPJ do Estabelecimento de Destino" e "Estabelecimento de Destino” e manter desabilitado para edição o campo “Departamento de Destino”;  
* Quando o usuário selecionar no campo “Tipo de Saida” a opção: "Saída para Departamento", o sistema deve preencher os campos “CNES/CNPJ do Estabelecimento de Destino" e "Estabelecimento de Destino” com os dados do estabelecimento logado e mantendo-os desabilitados para edição e habilitar e tornar obrigatório a seleção de um item no campo "Departamento de Destino"; 

---
# RGN066
## Cálculo da Quantidade Expedida da Saída por Produto
O sistema deve calcular a Quantidade Expedida da Saída somando todas as quantidades expedidas informadas nos detalhamentos adicionados ao produto. 

---
# RGN067
## Quantidade a Expedir
O sistema deve permitir informar um valor independente do saldo em estoque do produto 

---
# RGN068
## Credenciais SI Bnafar  
As configurações de credenciais e transmissão de dados para o SI Bnafar será realizada a nível estadual, e será aplicada para todos os entes vinculados a instância estadual.   

---
# RGN069
## Tipo Rename SI Bnafar
O gestor de integração pode configurar para sua instância se o sistema irá transmitir todos os produtos com registro em banco para os serviços federais (SI Bnafar e RNDS), ou apenas os itens da RENAME.   

---
# RGN070
## Auditoria Serviços Federais
O sistema deve auditar as transmissões de dados realizadas para os serviços federais (SI Bnafar e RNDS) e persistir no banco por prazo parametrizável. As consultas não precisam ser auditadas. Após o vencimento do prazo de auditoria, uma rotina deve realizar a exclusão física dos registros.    

---
# RGN071
## Selecionar Municípios Transmissão Federal
O gestor de integração deve selecionar os municípios de sua instância para não realizar o envio de dados para os serviços federais (SI Bnafar e RNDS).  

---
# RGN072
## Configuração ativa SI Bnafar
A transmissão de dados para o SI Bnafar somente deve ocorrer caso a configuração do serviço esteja salva no sistema para a UF e com o campo “Ativo” selecionado com a opção “Sim”.    

---
# RGN073
## Tipos Saída SI Bnafar
O sistema deverá transmitir os dados de saída e posição de estoque para o SI Bnafar. As saídas do tipo “Saída por Estorno de Entrada” e “Saída por Dispensação” não deverão ser transmitidas.    

---
# RGN074
## Registros Saída SI Bnafar
Para o envio dos dados de saída para o SI Bnafar devem ser contabilizadas as saídas que foram registradas no dia anterior (00:00:00 até as 23:59:59), bem como as saídas dos dias anteriores que ainda não foram enviadas devido a algum problema.  

---
# RGN075
## Registros Posição Estoque SI Bnafar
Para o envio dos dados de posição de estoque para o SI Bnafar, deve ser considerado a posição de estoque da meia-noite (início da rotina de transmissão), bem como as posições de estoque dos dias anteriores que não foram enviadas (também da meia-noite do respectivo dia). Caso a transmissão seja iniciada em outro horário diferente da meia-noite, o cálculo do estoque deverá levar em consideração o estoque da meia-noite.  

---
# RGN076
## Estorno SI Bnafar
As saídas com registro de estorno não deverão ser transmitidas para o SI Bnafar.  

---
# RGN077
## Prazo Estorno Saída SI Bnafar
Caso uma saída seja estornada no sistema após o envio do registro para o SI Bnafar, o sistema deverá identificar o protocolo e código do registro relativo a saída e transmitir a exclusão desse registro para o SI Bnafar. Isso somente deve ocorrer caso o estorno ocorra até o último dia do mês subsequente da saída (ex: saída realizada em 05/11 somente poderá ser excluída no SI Bnafar até 31/12).