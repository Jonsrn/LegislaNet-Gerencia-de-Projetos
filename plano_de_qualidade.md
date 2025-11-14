

---

# 🏛️ Plano de Gerenciamento da Qualidade - LegislaNet

## 1. Introdução

Este documento descreve o Plano de Gerenciamento da Qualidade para o projeto LegislaNet.
O objetivo é estabelecer os padrões, processos e responsabilidades da equipe (Jonathan, Henrique e João) para garantir que o software desenvolvido atenda aos requisitos e às necessidades dos usuários, conforme definido em nosso Plano de Gerenciamento.

Este plano formaliza nosso processo de desenvolvimento e promove uma **cultura da qualidade** em todo o ciclo de vida do projeto.

---

## 2. Metas de Qualidade

A qualidade no LegislaNet é definida pelos seguintes pilares:

### **Qualidade de Produto (Funcional)**

O software deve implementar todas as funcionalidades especificadas nos Issues do GitHub, atendendo aos requisitos dos Casos de Uso e passando nos Critérios de Aceite.

### **Qualidade de Produto (Intangível)**

O código-fonte deve ser limpo, legível, manutenível e seguir os padrões de desenvolvimento estabelecidos, incluindo aspectos como organização, clareza arquitetural e boa legibilidade.

### **Qualidade de Processo**

O desenvolvimento deve seguir um fluxo estruturado, transparente e rastreável, garantindo que todas as mudanças sejam solicitadas, analisadas, testadas e documentadas.

---

## 3. Processos de Garantia da Qualidade (QA)

Para atingir as metas de qualidade, estes processos serão adotados:

---

### 3.1 Gerenciamento de Mudanças e Rastreabilidade

Todo o trabalho seguirá o fluxo formal de Gerenciamento de Mudanças:

#### **Solicitação de Mudança**

Nenhuma funcionalidade ou correção será implementada sem a criação prévia de um Issue no GitHub.
Este Issue é a solicitação formal e deve ser atribuído a um Milestone (ex.: “Conclusão do MVP Web”).

#### **Análise de Impacto**

A equipe analisará o Issue para definir prioridade, responsável (Assignee) e etiquetas (Labels) no GitHub Projects e ClickUp.

#### **Desenvolvimento (Modifica Software)**

O responsável criará uma branch separada para a tarefa (ex.: `feat/issue-15-login-tablet`).
Todos os membros devem contribuir em suas próprias branches.

#### **Testar Software**

O desenvolvedor testará localmente sua funcionalidade antes de abrir um Pull Request (PR).

#### **Fechar Solicitação**

O PR deve ser vinculado ao Issue (“Closes #ID”).
Ele só será mergeado após revisão e aprovação de pelo menos um outro membro.

---

### 3.2 Padrões de Código e Legibilidade

* **Commits**: Devem seguir o padrão de Commits Semânticos (`feat:`, `fix:`, `docs:`, `style:`…)
* **Nomenclatura**: Variáveis, funções e arquivos devem ter nomes claros e em português, alinhados ao domínio.
* **Comentários**: Devem ser usados para explicar lógicas complexas ou partes essenciais da regra de negócio.

---

### 3.3 Revisão de Pares (Peer Review)

A revisão de pares é uma das principais ferramentas para garantir qualidade no projeto.

#### **Regra de Ouro**

Nenhum PR pode ser mergeado pelo próprio autor.

#### **Obrigatoriedade**

A aprovação de pelo menos um membro da equipe (não autor) é obrigatória.

#### **Checklist do Revisor**

O revisor deve verificar se:

* O código atende aos requisitos do Issue vinculado.
* O padrão de qualidade, legibilidade e nomenclatura foi seguido.
* Não há bugs aparentes ou quebra de funcionalidades existentes.

---

### 3.4 Gerenciamento de Bugs (Issues Externos)

Bugs ou sugestões reportados por outras equipes serão tratados com o mesmo rigor:

1. Issue externo é rotulado como **bug** ou **sugestão**.
2. A equipe realiza análise de impacto e define responsável.
3. É criada uma branch de correção (ex.: `fix/issue-29-bug-login`).
4. O PR correspondente é aberto, revisado e mergeado.
5. O Issue é fechado e o autor é notificado.

---

## 4. Artefatos de Gerenciamento da Qualidade

A documentação e evidências de qualidade incluem:

### **PLANO_DE_QUALIDADE.md**

Este documento, definindo todo o processo de QA.

### **CHANGELOG.md**

Registro de todas as alterações — atualizado a cada merge.

### **Histórico de Issues e Pull Requests**

O GitHub funciona como evidência viva de rastreabilidade, conectando solicitações, discussões, implementações e revisões.

### **GitHub Releases**

Ao final de cada Milestone, será criada uma Release formal
(ex.: v1.0.0 — MVP Web, v1.1.0 — App Flutter).

---

