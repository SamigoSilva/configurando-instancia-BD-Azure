# 🚀 Laboratório Azure SQL Database

![Azure SQL](https://img.shields.io/badge/Microsoft_Azure_SQL-0089D6?style=for-the-badge&logo=microsoft-sql-server&logoColor=white)

## 📋 Sumário
- [Visão Geral](#-visão-geral)
- [Configuração Técnica](#%EF%B8%8F-configuração-técnica)
- [Conceitos Aplicados](#-conceitos-aplicados)
- [Lições Aprendidas](#-lições-aprendidas)
- [Estrutura do Projeto](#-estrutura-do-projeto)
- [Referências](#-referências)

## 🌐 Visão Geral
Documentação completa do processo de implementação de um Banco de Dados SQL no Azure, abordando:
- Modelo PaaS (Platform as a Service)
- Configurações de alta disponibilidade
- Estratégias de segurança e monitoramento

## ⚙️ Configuração Técnica

### 🔧 Especificações
| **Componente**       | **Configuração**                  |
|----------------------|-----------------------------------|
| **Tipo de Serviço**  | Azure SQL Database                |
| **Tier**             | Standard S0 (10 DTUs)             |
| **Redundância**      | Geo-Redundant (GRS)               |
| **Região**           | Brazil South                      |
| **Autenticação**     | SQL + Azure AD                    |

### 🛠️ Implementação
1. **Criação do Servidor Lógico**
   ```powershell
   az sql server create `
     --name meu-sql-server `
     --resource-group meu-rg `
     --location brazilsouth `
     --admin-user sqladmin `
     --admin-password Senha@Segura123
