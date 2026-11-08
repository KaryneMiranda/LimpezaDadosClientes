# Limpeza de Dados de Clientes

Projeto da Sprint 1 em que avalio e preparo dados de clientes da Store 1, uma loja de comércio eletrônico, usando os fundamentos de Python.

## Objetivo

A Store 1 começou a coletar dados sobre seus clientes e quer usá-los para tomar decisões e melhorar a experiência online. Neste projeto, avalio a qualidade de uma amostra desses dados, corrijo os problemas encontrados e calculo algumas métricas simples de consumo.

## Etapas

### 1. Avaliação da qualidade dos dados
Identificação de problemas nos dados de um usuário:
- Nome com espaços desnecessários e sublinhado entre nome e sobrenome
- Idade armazenada como `float` em vez de inteiro
- Categorias favoritas em letras maiúsculas

### 2. Limpeza dos dados
- Remoção de espaços com `strip()` e troca do sublinhado por espaço com `replace()`
- Separação do nome e sobrenome com `split()`
- Conversão da idade para inteiro com `int()`
- Tratamento de erro com `try/except` para idades que não podem ser convertidas
- Conversão das categorias para letras minúsculas com um laço `for`

### 3. Métricas de consumo
- Valor total, mínimo e máximo gasto por um usuário
- Simulação de novas compras com um laço `while` até o cliente atingir US$ 1.500 e se tornar elegível para desconto
- Criação de um resumo formatado do usuário com `format()`

### 4. Análise da tabela de clientes
Usando uma lista aninhada com os dados de vários clientes:
- Cálculo da receita total da empresa
- Clientes com menos de 30 anos
- Clientes com menos de 30 anos e gastos acima de US$ 1.000
- Clientes que compraram roupas

## Principais resultados

- O usuário analisado gastou **US$ 1.280** no total (máximo de US$ 894 e mínimo de US$ 173).
- A receita total dos dois primeiros clientes é **US$ 2.109**.
- Dos 10 clientes da tabela, 5 têm menos de 30 anos. Só **Samantha Smith** e **James Lee** também gastaram mais de US$ 1.000.
- 5 clientes compraram roupas: Kate Morgan, Samantha Smith, Maria Garcia, Lisa Wilson e James Lee.

## Conceitos praticados

- Tipos de dados e conversão de tipos
- Métodos de string (`strip`, `replace`, `split`, `lower`, `join`, `format`)
- Listas e listas aninhadas
- Laços `for` e `while`
- Condicionais
- Tratamento de exceções (`try/except`)
- Funções nativas (`sum`, `min`, `max`)

## Tecnologias

- Python
- Jupyter Notebook

## Como executar

1. Clone o repositório
2. Instale o Jupyter:
   ```bash
   pip install jupyter
   ```
3. Abra o notebook:
   ```bash
   jupyter notebook projetosprint1.ipynb
   ```

> O projeto não depende de arquivos externos. Todos os dados estão no próprio notebook.
