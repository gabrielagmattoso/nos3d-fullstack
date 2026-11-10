# Documentação - Nós 3D

Esta pasta reúne a documentação do projeto de banco de dados do **Nós 3D**, um negócio de impressão 3D que hoje controla clientes, pedidos e materiais de forma espalhada (WhatsApp, e-mail e planilhas). O objetivo do projeto é centralizar essas informações em um banco de dados relacional.

A documentação segue as etapas de um projeto de banco de dados, da ideia até a implementação. Tudo o que está aqui também fica disponível no repositório principal do grupo.

## O que vai ter nesta pasta

**Levantamento de requisitos**
Explica o que o negócio precisa e quais problemas o banco deve resolver. Inclui o questionário feito com a parceira e a definição de personas (quem usa o sistema e para quê).

**MER (Modelo Entidade-Relacionamento)**
É o modelo conceitual, também chamado de DER. Ele mostra, em forma de diagrama, as entidades do negócio (como cliente, pedido, material e fornecedor), seus atributos e como elas se relacionam. Ainda não pensa em tabelas, só em como a informação funciona no mundo real.

**Modelo lógico**
É o MER transformado em tabelas. Mostra as colunas de cada tabela, as chaves primárias e estrangeiras e as cardinalidades dos relacionamentos. Foi feito no brModelo, e o arquivo editável é o `LogicoNos3D.brM3`. Para abrir, instale o brModelo e use *Arquivo → Abrir*.

**Dicionário de dados**
Explica o que significa cada tabela e cada coluna do banco: o tipo do dado, se é obrigatório e para que serve.

**Documento do projeto**
O documento com a descrição completa do trabalho, reunindo o diagnóstico da situação-problema, as decisões tomadas e os resultados de cada etapa.

## Como as etapas se conectam

1. **Requisitos:** o que o negócio precisa.
2. **MER:** como a informação se organiza.
3. **Modelo lógico:** como isso vira tabelas.
4. **Projeto físico:** o código SQL que cria o banco, na pasta `sql/`.

## Padrão de nomes

Os nomes das regras do banco seguem um prefixo que indica o tipo:

- `pk_` chave primária
- `fk_` chave estrangeira
- `uq_` valor único
- `ck_` regra de validação
