# Documento de Regras

# RGN001
## Permissão de acesso por funcionalidade

| Funcionalidade | Instalador | Administrador (ADM) | Gestor (GST) | Gestor Estabelecimento (GEST) | Farmacêutico (FAR) | Atendente (ATD) |
| -------------- | :-----------------: | :-----------------: | :----------: | :---------------------------: | :----------------: | :-------------: |
| **CONTROLE DE ACESSO** |
| **MODERAR ACESSO** | 
| Consultar Permissões Acesso | X | X | X | X |
| Atribuir Perfil | X | X | X | X |
| Detalhar Permissões Acesso | X | X | X | X |
| **SOLICITAR PERFIL** | 
| Consultar Meu Perfil | | X | X | X | X | X |
| Solicitar Perfil | | X | X | X | X | X |
| Detalhar Meu Perfil | | X | X | X | X | X |
| **GERENCIAR PERFIL** | 
| Consultar Perfil | | | X | 
| Cadastrar Perfil | | | X |
| Detalhar Perfil | | | X |
| **CONFIGURAÇÃO** | 
| **Cadastro de Entes** | 
| Consultar Ente | | X | 
| Cadastrar Ente | | X | 
| **CADASTRO** | 
| **Estabelecimento** | 
| Consultar Estabelecimento | | | X | X | X | X |
| Cadastrar Estabelecimento | | | X |
| Editar Estabelecimento | | | X | X | X | X |
| Detalhar Estabelecimento | | | X | X | X | X |
| **MOVIMENTAÇÃO** | 
| **Entrada** | 
| Consultar Entrada | | | X | X | X | X |
| Cadastrar Entrada | | | X | X | X | X |
| Editar Entrada | | | X | X | X | X |
| Detalhar Entrada | | | X | X | X | X |
| **Saída Diversa** | 
| Consultar Saída Diversa | | | X | X | X | X |  
| Cadastrar Saída Diversa | | | X | X | X | X |
| Editar Saída Diversa | | | X | X | X | X |
| Detalhar Saída Diversa | | | X | X | X | X |

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
# RGN012 (removido)
## Solicitação de perfil acesso.
 
---
# RGN013 (removido)
## Solicitações com status:

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
As exclusões permitidas no sistema sempre serão lógicas, sendo necessário manter o histórico temporal da existência do registro. Exceto para registro(s) na situação “Em preenchimento” a qual deve ser física.  

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
## Registro de Entrada por Estorno de Saída Diversa de produto(s)
Ao realizar o estorno da saída diversa do(s) produto(s), o sistema deve:

* Creditar o(s) produto(s) no estoque do estabelecimento da saída estornada, através da criação de um registro de entrada, gravando as seguintes informações: 
    * Modalidade de Licitação = “Saída Diversa”;
    * Tipo de Movimentação = “Entrada por Estorno de Saída Diversa”;  
    * Fornecedor = CNES ou CNPJ do estabelecimento que realizou saída;  
    * Tipo de Documento = “Estorno de Saída Diversa”;  
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
    * Situação do registro de entrada como “Armazenada”; 
* Alterar a situação do cadastro da saída diversa para “Estornada”

---
# RGN033
## Atualização de estoque após estorno de saída diversa
O sistema, identificando que uma saída diversa de produto(s) foi estornada, deve creditar a quantidade no saldo deste(s), considerando o lote, validade e programa de saúde e atualizar a posição de estoque do estabelecimento que realizou o estorno da saída diversa.  

---
# RGN034
## Apresentação de Lotes/Validades do produto

* Quando o tipo de saída for “Validade Vencida”, somente serão considerados e/ou apresentados os lotes/validades que estejam com a data de validade inferior a data atual. 
* Quando o tipo de saída for “Ajuste de Estoque”, “Usuário SUS”, “Apreensão Sanitária”, “Empréstimo” ou “Transferência”, somente serão considerados e/ou apresentados os lotes/validades que estejam válidos, com a data de validade igual ou superior a data atual. 
* Quando o tipo de saída for “Perda” ou “Roubo”, serão considerados e/ou apresentados todos os lotes/validades. independente da data de validade.

---
# RGN035
## Exclusão de produto na saída diversa
Somente será permitida a exclusão de um produto adicionado à saída se não tiver nenhum detalhamento vinculado a ele.  

---
# RGN036
## Saldo Estoque Atual
O sistema deve carregar e apresentar o saldo do produto em estoque, no momento, do estabelecimento logado, independente de lote/validade/programa de saúde.  

---
# RGN037
## Cálculo da Quantidade Total Recebida na Entrada do Produto
O sistema deve calcular a Quantidade Total Recebida somando todas as quantidades informadas nos detalhamentos adicionados ao produto.  

---
# RGN038
## Cálculo do Valor Total da Saída Diversa
O sistema deve calcular o Valor Total da Saída Diversa somado todos os valores totais dos produtos adicionados à saída diversa.  

---
# RGN039
## Cálculo da Quantidade Total da Saída por Produto
O sistema deve calcular a Quantidade Total da Saída somando todas as quantidades informadas nos detalhamentos adicionados ao produto.  

---
# RGN040
## Cálculo da Média do Valor Unitário do Produto
O sistema deve calcular o Valor Unitário do Produto através da média simples dos valores unitários do produto informados na(s) entrada(s), independente de lota, validade ou programa de saúde, ou seja, realiza-se o somatório de todos os elementos do rol e divide-se essa soma pela quantidade de elementos.  

---
# RGN041
## Cálculo do Valor Total da Saída para o Produto
O sistema deve calcular o Valor Total da Saída pela fórmula:  Quantidade Total da Saída X Valor Unitário do produto (média simples dos valores unitários informados na entrada do referido produto).  

---
# RGN042
## Produto da Saída
O sistema deve permitir apenas saída de produtos que possuem estoque no estabelecimento logado.  

---
# RGN043
## Quantidade de Saída do Produto
O sistema somente deve permitir informar uma quantidade de saída menor ou igual ao estoque disponível do produto, lote, validade e programa de saúde no estabelecimento logado.  

---
# RGN044
## Validar Saída Diversa do Produto
O sistema deve validar se já existe uma saída diversa com o mesmo tipo de saída diversa, tipo e número de documento e justificativa de uma saída diversa registrada ou em preenchimento para o estabelecimento.  

---
# RGN045
## Número de Registro da Saída Diversa
Ao salvar parcial ou registar uma saída diversa de produtos, caso ainda não exista, o sistema deve gerar um número identificador único para a saída diversa e apresentá-lo ao usuário.  

---
# RGN046
## Atualização de estoque após registrar uma saída diversa
O sistema, identificando que uma saída diversa de produto(s) foi registrada, deve debitar a quantidade no saldo deste(s), considerando o lote, validade e programa de saúde e atualizar a posição de estoque do estabelecimento que realizou a saída diversa.

---
# RGN047
## Validade do token de recuperação de senha
O tempo de validade do token gerado para recuperação de senha é de 20 minutos.

