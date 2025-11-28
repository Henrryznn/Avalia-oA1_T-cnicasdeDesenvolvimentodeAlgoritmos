-----

# README — Exercícios de Python A1

Este repositório contém quatro exercícios em Python, cada um abordando conceitos fundamentais como listas, dicionários, estruturas de repetição e estruturas condicionais. Também representados em **Pseudocódigo**.

## 📁 Organização dos Arquivos

```
exercicios/
├── exercicio1_verificacao_idade_py.ipynb
├── exercicio2_contador_pares_py.ipynb
├── exercicio3_lista_alunos_py.ipynb
└── exercicio4_cadastro_produtos_py.ipynb
```

A pasta `exercicios/` reúne todos os arquivos .py desenvolvidos, cujas lógicas estão descritas abaixo em pseudocódigo.

-----

## 📘 Descrição dos Exercícios

### 1\. Verificação de Idade (exercicio1\_verificacao\_idade.py)

Programa que solicita a idade do usuário e utiliza **estruturas condicionais** (`if`, `elif`, `else`) para verificar se a entrada em um evento é permitida.

#### Pseudocódigo

```
INICIO
  // Entrada de dados
  LEIA idade

  // Verificação e saída
  SE idade < 0 ENTAO
    ESCREVA "Idade inválida!"
  SENAO SE idade < 12 ENTAO
    ESCREVA "Entrada permitida somente com responsável."
  SENAO SE idade < 18 ENTAO
    ESCREVA "Entrada permitida apenas para eventos classificados como 'menores acompanhados'."
  SENAO SE idade <= 120 ENTAO
    ESCREVA "Entrada liberada! Bem-vindo ao evento."
  SENAO
    ESCREVA "Idade fora do intervalo válido."
  FIM SE
FIM
```

-----

### 2\. Contador de Números Pares (exercicio2\_contador\_pares.py)

Exibe números pares de 1 a 100 utilizando duas abordagens: um laço **FOR** e um laço **WHILE**. Mostra o uso adequado de operadores lógicos e estruturas de repetição.

#### Pseudocódigo

**Abordagem com FOR**

```
INICIO
  ESCREVA "Contador com FOR (números pares de 1 a 100):"
  PARA num DE 1 ATÉ 100 FACA
    SE (num MÓDULO 2) == 0 ENTAO // Verifica se é par
      ESCREVA num
    FIM SE
  FIM PARA
FIM
```

**Abordagem com WHILE**

```
INICIO
  ESCREVA "Contador com WHILE (números pares de 1 a 100):"
  num = 1
  ENQUANTO num <= 100 FACA
    SE (num MÓDULO 2) == 0 ENTAO // Verifica se é par
      ESCREVA num
    FIM SE
    num = num + 1 // Incremento
  FIM ENQUANTO
FIM
```

-----

### 3\. Cadastro de Alunos (exercicio3\_lista\_alunos.py)
*(Lista é uma estrutra de dados que servepara armazenar vários valores em uma única variável.)*
Recebe nomes digitados pelo usuário e os armazena em uma **lista**. O cadastro encerra quando "sair" é digitado, e ao final todos os nomes são exibidos.

#### Pseudocódigo

```
INICIO
  alunos = LISTA VAZIA
  
  // Laço de cadastro
  ENQUANTO VERDADEIRO FACA
    LEIA nome ("Digite o nome do aluno (ou 'sair' para finalizar): ")
    
    SE nome em caixa baixa é igual a "sair" ENTAO
      PARE O LAÇO
    FIM SE
    
    ADICIONE nome NA LISTA alunos
  FIM ENQUANTO
  
  // Exibição dos dados
  ESCREVA "Lista de alunos cadastrados:"
  PARA CADA aluno EM alunos FACA
    ESCREVA aluno
  FIM PARA
FIM
```

-----

### 4\. Cadastro de Produtos (exercicio4\_cadastro\_produtos.py)
*(Dicionário é uma estrutura que armazena pares de chabe e valor.)*
Sistema simples que registra produtos com nome e preço, utilizando um **dicionário** (`dict`). O programa permite inserir quantos itens desejar e exibe todos ao final.

#### Pseudocódigo

```
INICIO
  produtos = DICIONÁRIO VAZIO
  
  // Laço de cadastro
  ENQUANTO VERDADEIRO FACA
    LEIA nome ("Digite o nome do produto (ou 'sair' para finalizar): ")
    
    SE nome em caixa baixa é igual a "sair" ENTAO
      PARE O LAÇO
    FIM SE
    
    LEIA preco (para o produto 'nome')
    
    ADICIONE/ATUALIZE PRODUTO nome COM VALOR preco NO DICIONÁRIO produtos
  FIM ENQUANTO
  
  // Exibição dos dados
  ESCREVA "Lista de produtos cadastrados:"
  PARA CADA nome, preco NO DICIONÁRIO produtos FACA
    ESCREVA "Produto: " + nome + " — Preço: R$ " + preco FORMATADO
  FIM PARA
FIM
```

-----

## 🤝 Contribuição

Este é um repositório para fins de estudo. Se você é um colega de classe, sinta-se à vontade para:

  * **Sugerir melhorias:** Abra uma `issue` para relatar problemas ou sugerir melhorias.
  * **Enviar correções:** Crie um `pull request` para propor alterações no código.

> **Aviso:** Este repositório é uma referência de estudo. Lembre-se de não copiar o código diretamente, mas de usá-lo como inspiração para aprender e aprimorar suas próprias soluções.

-----

## 📝 Autor

**Gabriel Henrry Silva De Oliveira**

GitHub: [https://github.com/Henrryznn](https://github.com/Henrryznn)

Linkedin: [https://www.linkedin.com/in/gabriel-henrry-1a911a317/](https://www.linkedin.com/in/gabriel-henrry-1a911a317/)

-----

Agradecimentos:
A professora Kadidja Valeria pela excelente condução da disciplina e aos colegas por tornarem o aprendizado colaborativo e enriquecedor.

-----
