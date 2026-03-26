# Documentação Técnica: Sistema de Gestão de Ativos e Locações

**Empresa:** TechRent Soluções Tecnológicas S.A.  
**Documento:** Especificação de Requisitos e Regras de Negócio  
**Versão:** 1.0  
**Data de Emissão:** 24/05/2024  

---

## 1. Introdução

Este documento define as regras de negócio e a estrutura de dados para o novo sistema da **TechRent**, empresa especializada na locação de hardware de alto desempenho. O objetivo é garantir o controle total sobre o ciclo de vida dos ativos, desde o estoque até a devolução pelo cliente.

---

## 2. Regras de Negócio

As regras abaixo devem ser rigorosamente aplicadas no desenvolvimento do **Modelo Entidade-Relacionamento (MER)** e implementadas no banco de dados.

### 2.1 Gestão de Clientes

- **RN001 - Unicidade:** Todo cliente deve ser identificado unicamente pelo seu CPF (Pessoa Física) ou CNPJ (Pessoa Jurídica). O sistema não deve permitir registros duplicados.
- **RN002 - Integridade de Contato:** É obrigatório o preenchimento de e-mail e telefone para fins de cobrança e notificações contratuais.

### 2.2 Gestão de Equipamentos (Ativos)

- **RN003 - Patrimônio:** Cada equipamento possui uma etiqueta de patrimônio física única.
- **RN004 - Máquina de Estados:** Um equipamento deve obrigatoriamente estar em um dos seguintes estados:
  - `DISPONIVEL`: Pronto para ser alugado.
  - `LOCADO`: Atualmente em posse de um cliente.
  - `MANUTENCAO`: Indisponível para novos contratos devido a reparos técnicos.
  - `DESATIVADO`: Ativo que saiu de linha ou sofreu perda total.

### 2.3 Processo de Locação

- **RN005 - Bloqueio de Locação:** O sistema deve impedir a inclusão de equipamentos em contratos caso o status não seja `DISPONIVEL`.
- **RN006 - Histórico de Preços:** O valor da diária de um equipamento no contrato deve ser fixado no momento da locação. Se o preço da diária do equipamento mudar no futuro, os contratos antigos não devem ser alterados.
- **RN007 - Atendimento:** Toda locação deve obrigatoriamente registrar o funcionário (vendedor) responsável pela abertura do contrato.

---

#### AVISO ☢️

Qualquer entidade, data, pessoa ou similaridade citada nesse documento é fictícia, qualquer semelhança com a realidade é mera coincidência.

Este documento foi gerado por IA e posteriormente foi revisado.
