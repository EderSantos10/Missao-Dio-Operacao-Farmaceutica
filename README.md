# Missao-Dio-Operacao-Farmaceutica

# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS

**Data:** 01/08/2025  
**Empresa:** Abstergo Industries  
**Responsável:** Eder Vinicius Aguiar Alves dos Santos

---

## 📌 INTRODUÇÃO

Este relatório apresenta o processo de implementação de serviços em Cloud Computing utilizando a AWS (Amazon Web Services) na empresa Abstergo Industries, uma distribuidora farmacêutica com o objetivo de fornecer produtos para outras farmácias.

A proposta contempla a migração e implementação do ambiente tecnológico do zero, com foco em escalabilidade, segurança, automação de processos e principalmente otimização do custo-benefício, visando reduzir gastos com infraestrutura física e possibilitar crescimento sustentável da empresa.

---

## 💡 DESCRIÇÃO DO PROJETO

O projeto foi dividido em **3 etapas**, cada uma responsável por um serviço essencial da AWS, interligando armazenamento, processamento e banco de dados de forma inteligente.

---

### 🔹 Etapa 1: Amazon RDS – Banco de Dados Relacional Gerenciado

**O que é:**  
O Amazon RDS (Relational Database Service) é um serviço de banco de dados gerenciado que permite criar, operar e escalar bancos de dados relacionais na nuvem. Suporta engines como MySQL, PostgreSQL, MariaDB, Oracle e SQL Server.

**Aplicação no contexto da farmácia:**  
A base de dados da Abstergo será centralizada no RDS, permitindo o cadastro e gestão de clientes, produtos farmacêuticos, histórico de pedidos e controle de estoque. Com backups automáticos, alta disponibilidade e escalabilidade sob demanda, o RDS garante desempenho consistente e segurança dos dados críticos do negócio.

**Benefícios esperados:**
- Redução de custos com servidores físicos.
- Backups automáticos e replicação para alta disponibilidade.
- Conformidade com requisitos de segurança e integridade de dados (LGPD).

---

### 🔹 Etapa 2: AWS Lambda – Computação Sob Demanda (Serverless)

**O que é:**  
O AWS Lambda é um serviço de computação sem servidor que executa código em resposta a eventos, sem necessidade de provisionar ou gerenciar servidores.

**Aplicação no contexto da farmácia:**  
Utilizaremos funções Lambda para automação de processos como:
- Envio de alertas e notificações (via SNS, e-mail, etc.) quando um pedido é finalizado.
- Validação e verificação do status de pagamento antes de liberar a separação do pedido.
- Integração com o Amazon S3 para analisar arquivos de comprovantes e registros.

**Benefícios esperados:**
- Redução de custos operacionais com processos automatizados.
- Alta escalabilidade sem necessidade de gerenciamento de infraestrutura.
- Processos executados apenas quando necessário (paga-se apenas pelo uso).

---

### 🔹 Etapa 3: Amazon S3 – Armazenamento de Objetos

**O que é:**  
O Amazon S3 (Simple Storage Service) é um serviço de armazenamento de objetos altamente escalável, seguro e durável, ideal para armazenar qualquer tipo de arquivo.

**Aplicação no contexto da farmácia:**  
O S3 será utilizado para armazenar documentos como:
- Comprovantes de pagamento dos pedidos.
- Receitas médicas digitalizadas.
- Relatórios de entrega e logística.

Além disso, o S3 será integrado com o AWS Lambda para ativar funções específicas (ex: validação de arquivos, atualização de status de pedidos) assim que novos arquivos forem adicionados ao bucket.

**Benefícios esperados:**
- Armazenamento seguro e ilimitado por um custo reduzido.
- Integração nativa com Lambda e outros serviços AWS.
- Controle de acesso refinado via políticas IAM e versionamento de arquivos.

---

## ✅ CONSIDERAÇÕES FINAIS

A adoção desses três serviços AWS proporciona à Abstergo Industries uma infraestrutura moderna, flexível e econômica. O uso conjunto de **Amazon RDS**, **AWS Lambda** e **Amazon S3** cobre de forma eficiente as áreas críticas da operação: banco de dados, automação e armazenamento.

Com essa base sólida, a empresa está pronta para crescer, atender com eficiência seus parceiros e manter um controle inteligente sobre suas operações, garantindo confiabilidade e segurança em cada etapa do processo.

---

