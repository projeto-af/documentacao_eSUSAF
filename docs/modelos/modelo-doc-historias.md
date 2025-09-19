# História de Usuário — {{Título curto}}

## HU### - 
**Como** {{persona}}  
**Quero** {{ação/objetivo}}  
**Para** {{valor/resultado}}

## Contexto
[Contextualização sobre a história de Usuário]

## Critérios de Aceite
1. [Insira aqui os critérios]
2. [Insira aqui os critérios]
3. [Insira aqui os critérios] 

## Definição de Pronto (DoD)
1. Regras de negócio aplicadas: [RN-###, RN-###].
2. Validações cliente/servidor conforme tabela de campos.
3. Mensagens exibidas exatamente como no Documento de Mensagens.
4. Domínios carregados conforme Documento de Domínios.
5. Acessibilidade básica: foco por teclado, aria-labels.
6. Telemetria: eventos {{evt_nome}}.
7. Testes: casos cobrindo cenários de sucesso/erro.
8. Documentação atualizada (se criou/alterou RN/MSG/DOM).

## Tabela de Campos (Negócio + Técnico + QA)
Cada linha = 1 campo da tela.

# Tabela de Campos — Exemplo

> Este modelo reúne em uma única tabela as visões de **Negócio**, **Técnico** e **QA**.  
> Cada linha representa **um campo da tela**.

| Field ID   | Rótulo (Negócio) | Descrição (Negócio) | Obrigatório? | Regras Negócio | Perfis de Usuário | Domínio | Tipo de Dado (Técnico) | Tamanho/Regex (Técnico) | Origem/Alvo (Técnico) | Validação (QA) | Mensagens de Erro (QA) | LGPD / Sensibilidade |
|------------|------------------|---------------------|--------------|----------------|-------------------|---------|------------------------|-------------------------|-----------------------|----------------|------------------------|----------------------|
| F-PAC-CPF  | CPF do paciente  | Identifica unicamente o paciente | Sim | RN-012: CPF válido; RN-045: Único por paciente | Atendente, Farmacêutico | DOM-001 | String | `^\d{11}$` | `paciente.cpf` | Front: regex; Back: algoritmo CPF + unicidade | [“CPF inválido”](../modelos/modelo-doc-mensagens.md#msg-004--cpf-inválido); “CPF já cadastrado” | Pessoal sensível |
| F-PAC-NOME | Nome completo    | Nome civil do paciente | Sim | RB-101: Nome ≥ 2 palavras | Atendente | DOM-002 | String | `^.{3,}$` | `paciente.nome` | Front: tamanho mínimo; Back: sanitização | “Informe nome e sobrenome” | Pessoal |
| F-PAC-UF   | UF               | Estado de origem do paciente | Não | — | Atendente | DOM-003 | Enum (2 letras) | `^[A-Z]{2}$` | `paciente.uf` | Back: enum válido | “UF inválida” | Não sensível |

---

## Como usar
- **Equipe de Negócio** preenche colunas até "Domínio”.
- **Time Técnico** completa colunas de tipo de dado, regex, origem/alvo.
- **QA** deriva cenários a partir das colunas de Validação e Mensagens de Erro.

## Protótipo
[Imagem do Protótipo](../imagens/)  
[Link para Protótipo]()

## Dependências
- API/Serviços: {{GET/POST …}}
- Integrações: {{CNES, RFB …}}
- Feature flag: {{FF-IDENT}} (se aplicável)

## Referências
- **Regras**: [Documento de Regras](../modelos/modelo-doc-regras.md)
- **Mensagens**: [Documento de Mensagens](../modelos/modelo-doc-mensagens.md)
- **Domínios**: [Documento de Domínios](../modelos/modelo-doc-dominios.md)

# Como Usar o Modelo
- Deverá ser transformado em um modelo de issue no GitLab
- Uma HU sempre deverá estar vinculada a um Épico
- Uma HU pode ter várias tarefas, visando facilitar a divisão do trabalho entre o time
- 