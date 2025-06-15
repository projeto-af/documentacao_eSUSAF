# ESPECIFICAÇÃO TÉCNICA 040: INTEGRAÇÃO AO SERVIÇO PDQ DO CNS

| **ETE:**     | 040                                        |
|--------------|--------------------------------------------|
| **Título:**  | Integração ao serviço PDQ do CNS           |
| **Autor:**   | Jessé Azevêdo <jesse.azevedo@saude.gov.br> |
| **Status:**  | Em validação                               |
| **Versão:**  | 1.0                                        |

## Histórico de Revisões

| **Versão** | **Data**   | **Autor**     | **Descrição**        |
|------------|------------|---------------|----------------------|
| 1.0        | 07/04/2025 | Jessé Azevêdo | Criação do documento |

## História de Usuário

Eu como usuário do e-SUS AF, desejo que o sistema esteja integrado ao serviço PDQ do CNS, para que eu possa consultar os dados de usuários do SUS de forma rápida e eficiente.

## Motivação

O e-SUS AF possui registro específico para Usuários SUS, esses dados são utilizados para o registro de dispensação ou fornecimento de medicamentos e são essenciais para o envio de dados ao serviço de interoperabilidade do Registro Eletrônico de Dispensação ou Fornecimento de Medicamentos (REDFM).
De forma a facilitar o processo de inclusão de um usuário SUS na aplicação, a integração com o serviço PDQ do CNS traz inúmeras vantagens, evitando que o usuário redigite um conjunto de informações como CPF, nome, data de nascimento e nome da mãe. Essa integração permitirá que o sistema e-SUS AF tenha acesso a informações atualizadas e precisas sobre os usuários do SUS, facilitando a gestão da assistência farmacêutica.

## Implementação

A integração com o serviço PDQ do CNS será realizada através de um serviço REST, utilizando o padrão FHIR (Fast Healthcare Interoperability Resources). O sistema e-SUS AF fará uma requisição ao serviço PDQ do CNS, passando o CPF ou CNS do usuário como parâmetro de busca. O serviço PDQ retornará os dados do usuário, que serão exibidos na tela de cadastro de usuários SUS do e-SUS AF.
Para integração, o e-SUS AF deverá ser capaz de gerenciar os recursos necesssários para a comunicação com o serviço PDQ do CNS, incluindo autenticação, autorização e tratamento de erros. O sistema deverá garantir que os dados recebidos do serviço PDQ sejam armazenados de forma segura e em conformidade com as normas de proteção de dados pessoais.
A princípio, a o administrador deverá contar com um recurso para configurar a integração com o serviço PDQ do CNS na tela de "Gestão de Integrações", onde deverá informar o endereço do serviço, e fazer o upload do certificado digital necessário a integração.
