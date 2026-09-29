# 🚗 Query-Estacionamento

Este repositório contém o script SQL para a modelagem, criação e manipulação de um banco de dados voltado ao gerenciamento de uma **Loja de Carros / Estacionamento**. O projeto foi desenvolvido com foco no aprendizado prático de restrições de integridade, relacionamentos entre tabelas e comandos DML.

## 🛠️ Tecnologias Utilizadas

*   **Banco de Dados:** Microsoft SQL Server / T-SQL (Transact-SQL)
*   **Ambiente de Desenvolvimento:** SQL Server Management Studio (SSMS)

## 📌 Estrutura do Banco de Dados

O banco de dados é composto por duas tabelas principais fortemente relacionadas através de chaves estrangeiras:

1.  **`tbl_carros`**: Armazena as informações dos veículos (Placa, Marca, Modelo, Ano e Combustível).
2.  **`tbl_vendedores`**: Armazena o cadastro dos funcionários da loja, vinculando-os diretamente ao veículo sob sua responsabilidade através da placa do carro.

### 📐 Modelo Relacional

*   A tabela `tbl_carros` possui a coluna `placa_do_carro` como sua **Chave Primária (Primary Key)**.
*   A tabela `tbl_vendedores` possui o `codigo_do_vendedor` como **Chave Primária (Primary Key)** e referencia os veículos utilizando `placa_do_carro` como **Chave Estrangeira (Foreign Key)**.

## 🚀 Como Executar o Projeto

1. Certifique-se de ter o **SQL Server** e o **SSMS** instalados em sua máquina.
2. Clone este repositório:
   ```bash
   git clone https://github.com/JeremiasDaSilva/Query-Estacionamento.git
   ```
3. Abra o arquivo `Estacionamento.sql` no seu ambiente SQL Server.
4. Execute o script em blocos ou por completo para criar a database `loja_de_carros`, povoar as tabelas com os dados de exemplo e testar as consultas.

## 📋 Funcionalidades Demonstradas no Script

*   Criação e seleção automática do banco de dados (`CREATE DATABASE` e `USE`).
*   Definição correta de restrições (`PRIMARY KEY` e `FOREIGN KEY`).
*   Inserção em massa de dados de teste (`INSERT INTO`).
*   Demonstração de comandos de atualização condicional (`UPDATE` com regras de integridade).
*   Scripts utilitários para reinicialização do ambiente (`DROP TABLE`).

---
Desenvolvido por [Jeremias da Silva](https://github.com/JeremiasDaSilva).
