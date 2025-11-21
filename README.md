# 🏋️‍♂️ Projeto – Sistema de Avaliação de Atletas em JavaScript (POO)

Este projeto foi desenvolvido como solução do desafio de certificação em JavaScript, utilizando Programação Orientada a Objetos (POO).
O objetivo é construir uma aplicação capaz de receber informações de um atleta, calcular diversos parâmetros — como categoria, IMC e média válida — e exibi-los de maneira organizada ao usuário.

# 📘 📌 Descrição do Desafio

A organização de uma competição esportiva solicitou um sistema capaz de gerenciar informações dos atletas e fornecer cálculos automáticos com base em critérios definidos.
Para isso, foi necessário criar uma classe Atleta, responsável por armazenar os dados e realizar todos os cálculos referentes ao competidor.

A aplicação deve:

- Receber dados de um atleta

- Calcular sua categoria etária

- Calcular seu IMC

- Calcular sua média válida de notas (desconsiderando maior e menor nota)

- Exibir todas as informações formatadas

# 🧠 Objetivos de Aprendizado

O projeto reforça os seguintes conceitos:

✔ Programação Orientada a Objetos (POO)

- Criação de classes

- Atributos

- Métodos

- Encapsulamento

✔ Manipulação de Arrays

- sort()

- slice()

- reduce()

✔ Estrutura e organização de código

- Modularidade

- Clareza na implementação de métodos

- Uso de console.log() para saída dos resultados

# 🏗️ Estrutura do Projeto

🔹 Classe Atleta

A classe concentra todos os atributos e métodos do atleta.

### Atributos

- nome

- idade

- peso

- altura

- notas (array com 5 valores numéricos)

### Métodos

### 🔍 Métodos de cálculo
| Método                 | Função                                        |
| ---------------------- | --------------------------------------------- |
| `calculaCategoria()`   | Retorna a categoria com base na idade         |
| `calculaIMC()`         | Retorna o IMC baseado na fórmula oficial      |
| `calculaMediaValida()` | Calcula a média, excluindo maior e menor nota |

### 📤 Métodos de acesso
| Método                | Retorno             |
| --------------------- | ------------------- |
| `obtemNomeAtleta()`   | Nome do atleta      |
| `obtemIdadeAtleta()`  | Idade               |
| `obtemPesoAtleta()`   | Peso                |
| `obtemAlturaAtleta()` | Altura              |
| `obtemNotasAtleta()`  | Notas               |
| `obtemCategoria()`    | Categoria calculada |
| `obtemIMC()`          | IMC calculado       |
| `obtemMediaValida()`  | Média válida        |

# 🧮 Regras de Cálculo

### 1️⃣ Categoria por Idade
| Idade           | Categoria     |
| --------------- | ------------- |
| 9–11            | Infantil      |
| 12–13           | Juvenil       |
| 14–15           | Intermediário |
| 16–30           | Adulto        |
| Fora das faixas | Sem categoria |

### 2️⃣ Cálculo do IMC

#### Fórmula:

`IMC = peso / (altura * altura)`

### 3️⃣ Cálculo da Média Válida

1. Ordenar as notas

2. Remover menor e maior

3. Realizar a média das três notas restantes

#### Exemplo:
`Notas: [10, 9.34, 8.42, 10, 7.88]
Ordenadas: [7.88, 8.42, 9.34, 10, 10]
Notas válidas: [8.42, 9.34, 10]
Média: (8.42 + 9.34 + 10) / 3
`