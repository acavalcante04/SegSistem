# SegSistem

Sistema integrado para gestão de segurança eletrônica. Centraliza orçamentos, ordens de serviço, controle de estoque e fluxo de caixa. Inclui aplicativo externo para técnicos de campo e gestão fiscal/financeira completa (NFe e Boletos).

🛡️ SegSistem - ERP de Segurança Eletrônica
Sistema Integrado de Gestão e Automação para Empresas de Segurança e Monitoramento

O SegSistem é uma solução completa (Web e Mobile) desenvolvida para centralizar a operação de empresas de segurança eletrônica. O sistema gerencia desde o primeiro contato com o cliente até a execução técnica e o controle fiscal/financeiro, garantindo rastreabilidade total e eficiência operacional.

O projeto adota a metodologia Learning-Driven Development, utilizando Python e Django para criar um backend robusto e uma API para aplicativos móveis.

🎯 Visão Geral do Sistema
O sistema é dividido em duas interfaces principais:

Portal Web de Gerenciamento: Para administração, financeiro, estoque e recepção.

Aplicativo Externo (Mobile): Focado no atendimento de campo para técnicos e supervisão administrativa.

🚀 Funcionalidades Principais
👥 Gestão de Clientes Inteligente

Múltiplos Endereços: Cadastro de um único cliente (PF ou PJ) com suporte a múltiplos locais de instalação/endereços.

Controle de Inadimplência: Sistema de ativação e desativação automática de clientes baseado na confirmação de pagamentos e datas de previsão.

Histórico: Registro completo de orçamentos, O.S. e notas fiscais por cliente.

🛠️ Orçamentos e Ordens de Serviço (O.S.)

Criação Detalhada: Elaboração de orçamentos com produtos e serviços.

Direcionamento Técnico: A recepção pode alocar técnicos específicos para cada O.S. com base na disponibilidade.

Fluxo de Status: Acompanhamento em tempo real (Pendente → Em Execução → Finalizada).

Comprovantes: Impressão de termos de garantia e relatórios técnicos em PDF.

💰 Controle Financeiro & Fiscal

Contas a Pagar e Receber: Gestão completa do fluxo de caixa.

Notas Fiscais:

Emissão/Retirada de notas de produto e serviço.

Upload e recebimento de notas fiscais de clientes.

Previsão Financeira: Controle de datas de previsão de pagamento por cliente.

Pagamentos: Gestão de boletos e baixa de pagamentos integrada à ativação do cliente.

📦 Gerenciamento de Estoque
Controle de entrada e saída de materiais.

Baixa automática de produtos ao finalizar uma O.S..

Alertas de estoque mínimo.

🔐 Perfis de Acesso e Permissões
O sistema implementa controle rigoroso de permissões (ACL) para diferentes cargos:

1. 👑 Administrador (Admin)
Acesso: Total (Web e App Mobile).

Funções: Configuração do sistema, auditoria de logs, gestão de usuários e visão global de todos os módulos.

2. 📡 Técnico de Campo
Acesso: Predominantemente via App Externo (Mobile).

Funções:

Receber O.S. direcionadas.

Registrar execução do serviço, checklist e fotos (Antes/Depois).

Visualizar dados básicos do cliente e endereço da visita.

3. 💲 Financeiro
Acesso: Portal Web.

Funções:

Pagamento de notas e fornecedores.

Recebimento e conferência de notas de clientes.

Baixa de boletos.

Gerenciamento de ativação/desativação de clientes inadimplentes.

4. 🎧 Recepção / Atendimento
Acesso: Portal Web.

Funções:

Abertura de chamados e criação de Orçamentos.

Agendamento e direcionamento de Técnicos para O.S.

Atendimento inicial e cadastro de clientes.

🛠️ Stack Tecnológica

Backend: Python 3.12+ & Django 5.x.

API: Django REST Framework (Integração com App Mobile).

Banco de Dados: PostgreSQL.

Frontend Web: Django Templates + Bootstrap/Tailwind.

Mobile: React Native ou PWA (Consumindo API via JWT).

Documentos: WeasyPrint (Geração de PDFs e Notas).

📂 Estrutura do Projeto Atual
O repositório contém atualmente a Fase 1 (Prototipagem da Lógica):

classes.py: Protótipo funcional das classes Cliente e Endereco, demonstrando a lógica de encapsulamento e relacionamento One-to-Many (Um cliente, vários endereços).

SegSistem.pdf: Documentação técnica completa da arquitetura.

📅 Roadmap de Desenvolvimento
[x] Planejamento: Arquitetura e Regras de Negócio definidas.

[x] Prototipagem: Classes base (classes.py).

[ ] Configuração: Setup Django + PostgreSQL + Git.

[ ] Módulo Core: Cadastro de Usuários (Admin, Técnico, Financeiro) e Autenticação.

[ ] Módulo Clientes: CRUD completo com múltiplos endereços.

[ ] Módulo Estoque: Produtos, Serviços e Movimentação.

[ ] Módulo Financeiro: Contas a Pagar/Receber e Lógica de Bloqueio.

[ ] API & Mobile: Desenvolvimento dos endpoints e App dos técnicos.

🤝 Contribuição
Contribuições são bem-vindas! Este projeto segue um fluxo de Trello organizado. Por favor, abra uma issue ou discuta no quadro de tarefas antes de submeter um PR.
