# 🏛️ Changelog - LegislaNet

Este documento registra todas as mudanças significativas no projeto LegislaNet, conforme o processo de Gerenciamento de Mudanças e o Plano de Qualidade do projeto.

O formato é baseado no **Keep a Changelog**.

---

## [1.1.0] - 2025-11-13

Esta release marca a conclusão da Aplicação Flutter, finalizando o ecossistema mobile para os vereadores e concluindo o Milestone **"Conclusão da Aplicação Flutter"**.

### Added — Funcionalidades Adicionadas

- **(PR #12)** Estrutura inicial do projeto para o Backend do Tablet. *(Closes #19)*
- **(PR #13)** Configuração do Logger Winston e conexão com Supabase no Backend do Tablet. *(Closes #20)*
- **(PR #14)** Implementação da autenticação do vereador e endpoints de consulta de dados (perfil, pautas) na API do Tablet. *(Closes #21, #23)*
- **(PR #15)** Implementação do serviço de WebSocket (`websocketService.js`) no Backend do Tablet. *(Closes #24)*
- **(PR #16)** Implementação do endpoint de registro de voto na API do Tablet. *(Closes #25)*
- **(PR #17)** Estruturação do projeto Flutter, incluindo dependências (`pubspec.yaml`) e o serviço de autenticação (`auth_service.dart`). *(Closes #26, #27)*
- **(PR #18)** Desenvolvimento das telas de Login, Dashboard do Vereador e implementação do serviço de WebSocket no App Flutter. *(Closes #28, #29, #30)*
- **(PR #19)** Desenvolvimento da UI da Tela de Votação no App Flutter. *(Closes #31)*
- **(PR #20)** Implementação do serviço de Toast customizado no App Flutter. *(Closes #32)*
- **(PR #20)** Adição dos scripts de teste do projeto. *(Closes #53)*

### Documentation

- **(PR #20)** Adição e atualização dos arquivos `README.md` do ecossistema mobile (`/Apps/tablet_backend/` e `/Apps/tablet_app/`). *(Closes #22)*

---

## [1.0.0] - 2025-11-06

Esta release marca a conclusão do MVP (Minimum Viable Product) do sistema web, incluindo:
- Painéis de administração (Super Admin e Admin de Câmara)
- Portal público
- Serviços de transparência

Conclui o Milestone **"Conclusão do MVP Web"**.

### Added — Funcionalidades Adicionadas

- **(PR #02)** Organização básica de diretórios para o projeto principal e a futura aplicação Flutter. *(Closes #02, #18)*
- **(PR #03)** Estrutura básica do backend (Node.js, Supabase, middlewares de segurança e autenticação JWT). *(Closes #3, #4, #5, #6)*
- **(PR #04)** Implementação da API (CRUD) de Câmaras. *(Closes #07)*
- **(PR #05)** Implementação da API (CRUD) de Partidos Políticos. *(Closes #08)*
- **(PR #06)** Implementação da API (CRUD) de Vereadores e gestão de usuários. *(Closes #09)*
- **(PR #07)** Implementação da API (CRUD) de Sessões Plenárias e Pautas. *(Closes #10)*
- **(PR #08)** Implementação da API de Controle da Votação e endpoints públicos para o portal. *(Closes #11)*
- **(PR #09)** Implementação de serviços adicionais no backend do administrador (ex: `adminService.js`, `sessionService.js`). *(Closes #12)*
- **(PR #10)** Implementação de todo o frontend da aplicação web, incluindo:
  - Painel do Super Admin  
  - Painel do Admin da Câmara  
  - Portal da Transparência  
  - Tela de Votação da TV  
  *(Closes #13, #14, #15, #16)*
- **(PR #11)** Implementação dos serviços de transparência (Livestream YouTube, Votação ao Vivo e Auditoria). *(Closes #17)*

### Documentation

- **(PR #01)** Adição da documentação inicial do projeto (Plano de Gerenciamento, Requisitos, Casos de Uso, etc.). *(Closes #01)*

---
