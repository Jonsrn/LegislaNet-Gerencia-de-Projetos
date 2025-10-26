
---

# 🏛️ Plano de Gerenciamento da Qualidade - LegislaNet

## 1. Introdução

Este documento descreve o Plano de Gerenciamento da Qualidade para o projeto **LegislaNet**. O objetivo é estabelecer os padrões, processos e responsabilidades necessários para garantir que o software desenvolvido atenda aos requisitos definidos e às necessidades dos usuários, promovendo uma "cultura da qualidade" em todo o ciclo de desenvolvimento.

## 2. Metas de Qualidade

A qualidade no LegislaNet é definida pelos seguintes pilares:

* **Qualidade de Produto (Funcional):** O software deve implementar todas as funcionalidades especificadas nos *Issues* do GitHub, atendendo aos requisitos dos usuários (Administrador, Vereador, Cidadão).
* **Qualidade de Produto (Intangível):** O código-fonte deve ser limpo, legível, manutenível e seguir os padrões de desenvolvimento estabelecidos. Isso inclui "aspectos intangíveis" como elegância e legibilidade.
* **Qualidade de Processo:** O desenvolvimento deve seguir um fluxo estruturado e rastreável, garantindo que todas as mudanças sejam solicitadas, analisadas, testadas e documentadas.

## 3. Processos de Garantia da Qualidade (QA)

Para atingir as metas de qualidade, os seguintes processos de gerenciamento serão adotados:

### 3.1 Gerenciamento de Mudanças e Rastreabilidade

Todo o trabalho de desenvolvimento seguirá o fluxo formal de Gerenciamento de Mudanças:

1.  **Solicitação de Mudança:** Nenhuma funcionalidade ou correção será implementada sem a criação prévia de um **Issue** no GitHub. Este Issue é a "Solicitação de Mudança" formal e deve ser atribuído a um *Milestone* (MVP Web ou App Flutter).
2.  **Análise de Impacto:** A equipe analisará o Issue para definir a prioridade, o responsável (*Assignee*) e as etiquetas (*Labels*) correspondentes (ex: `backend`, `frontend`, `bug`).
3.  **Desenvolvimento (Modifica Software):** O responsável criará uma *branch* separada para a tarefa (ex: `feat/issue-15-login-tablet`). Todos os membros devem contribuir com o desenvolvimento em suas próprias *branches*.
4.  **Testar Software:** O desenvolvedor é responsável por testar sua funcionalidade localmente antes de abrir um Pull Request (PR).
5.  **Fechar Solicitação:** Um PR será aberto e **obrigatoriamente vinculado ao Issue** (usando "Closes #ID"). O PR só será "mergeado" após a revisão e aprovação de, no mínimo, um outro membro da equipe.

### 3.2 Padrões de Código e Legibilidade

* **Commits:** As mensagens de commit devem ser claras e seguir o padrão de *Commits Semânticos* (ex: `feat:`, `fix:`, `docs:`).
* **Nomenclatura:** Nomes de variáveis, funções e arquivos devem ser claros e em português, para facilitar a leitura e manutenção.
* **Comentários:** Funções complexas ou lógicas de negócio críticas devem ser documentadas com comentários no código.

### 3.3 Revisão de Pares (Peer Review)

A revisão de pares é a principal ferramenta para garantir a "cultura da qualidade" e realizar a etapa de "Testar software".

* Nenhum PR pode ser "mergeado" pelo seu próprio autor.
* O revisor é responsável por verificar:
    1.  Se o código atende aos requisitos do Issue vinculado.
    2.  Se o código segue os padrões de legibilidade definidos.
    3.  Se a mudança não introduz novos bugs aparentes.
* A aprovação de, no mínimo, um outro membro da equipe é obrigatória para o *merge*.

### 3.4 Gerenciamento de Bugs (Issues Externos)

Bugs ou sugestões reportadas por outras equipes através dos Issues do GitHub serão tratadas com prioridade. Elas seguirão o mesmo fluxo de Gerenciamento de Mudanças:

1.  O Issue será etiquetado como `bug` ou `sugestao`.
2.  Será feita a análise de impacto e atribuído um responsável.
3.  Uma *branch* de correção (ex: `fix/issue-29-bug-login`) será criada.
4.  Um PR será aberto, revisado, "mergeado" e o Issue será fechado, notificando o autor da sugestão.

## 4. Artefatos de Qualidade

A "geração de documentação relacionada ao gerenciamento de qualidade" será evidenciada pelos seguintes artefatos:

1.  **Este Documento (`PLANO_DE_QUALIDADE.md`):** Define o processo.
2.  **`CHANGELOG.md`:** Um registro de todas as alterações feitas no sistema, atualizado a cada *merge* de PR, conforme exigido pela Aula 08.
3.  **`README.md`:** Documentação principal do projeto, contendo instruções de instalação e uso.
4.  **GitHub Issues e Pull Requests:** O histórico de Issues e PRs serve como evidência de rastreabilidade completa do processo de mudança.
5.  **GitHub Releases:** Ao final de cada *Milestone*, uma "Release" formal será criada no GitHub para "empacotar" a entrega.
    * `v1.0.0 - Conclusão do MVP Web`
    * `v1.1.0 - Conclusão da Aplicação Flutter`