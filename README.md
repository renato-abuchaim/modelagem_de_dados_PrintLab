🧩 Sistema de Gerenciamento de Impressões 3D – PrintLab

Este repositório contém os scripts SQL desenvolvidos para a Experiência Prática 4 da disciplina de Modelagem e Análise de Banco de Dados.
O projeto representa um sistema completo para gerenciar pedidos de impressão 3D, arquivos enviados, materiais utilizados e estado das impressoras.

📋 Estrutura do Projeto

O banco de dados DB_PRINTLAB gerencia:

👤 Clientes

Dados pessoais

Contato

Associação com arquivos enviados e pedidos realizados

🖨️ Impressoras

Modelos

Status operacional (Disponível, Ocupada, Manutenção)

Vinculação aos pedidos durante a execução

🧵 Materiais

Tipo de filamento (PLA, ABS…)

Cor

Temperatura de extrusão

📁 Arquivos 3D

Arquivos enviados pelos clientes

Formato (STL, OBJ…)

Tamanho

Associação ao cliente

📝 Pedidos

Status do pedido (Recebido, Em fila, Imprimindo, Concluído)

Impressora utilizada

Material selecionado

Data de criação

🛠️ Tecnologias Utilizadas

SGBD: MySQL Server 8.0

Ferramenta: MySQL Workbench

Linguagem: SQL (DDL, DML e consultas)

📂 Como Executar

Criação da Estrutura
Abra o arquivo:
01_criacao_tabelas.sql
Execute no MySQL Workbench para criar todas as tabelas, chaves primárias e estrangeiras.

Inserção de Dados
Execute o arquivo:
02_insercao_dados.sql
Ele popula o banco com registros de exemplo (clientes, impressoras, materiais, pedidos).

Consultas e Manipulações
Utilize:
03_consultas_e_operacoes.sql
Nele você encontrará:

Consultas com JOIN

Relatórios com GROUP BY

Filtros com WHERE

Exemplos de UPDATE e DELETE

Verificações de integridade

📊 Requisitos Atendidos

✔ Criação de tabelas totalmente normalizadas até a 3FN
✔ Relacionamentos 1:N, N:1 e 1:1 corretamente implementados
✔ Chaves Primárias e Estrangeiras com integridade referencial
✔ Scripts de INSERT para todas as tabelas
✔ Consultas SQL com:

JOIN (INNER/LEFT)

GROUP BY

ORDER BY

Funções de agregação
✔ Operações de manipulação:

UPDATE

DELETE
✔ Modelo lógico, DER e estrutura pronta para implantação

📦 Organização do Repositório
/PrintLab-Database
│
├── 01_criacao_tabelas.sql
├── 02_insercao_dados.sql
├── 03_consultas_e_operacoes.sql
│
├── /diagramas
│     ├── DER_conceitual.png
│     └── DER_logico.png
│
└── README.md

📜 Licença

Este projeto é acadêmico e pode ser utilizado para estudos, prática e aperfeiçoamento de modelagem e SQL.
