# Aula 01 - Fundamentos da Programação Python

**Data:** 06/10/2025  
**Carga Horária:** 4 horas  
**Docente:** Marcos Jhollyfer Felix Rodrigues

---

## Sumário

1. [Introdução às Linguagens de Programação](#1-introdução-às-linguagens-de-programação)
2. [História e Evolução do Python](#2-história-e-evolução-do-python)
3. [Conceito de Pseudocódigo e Algoritmos](#3-conceito-de-pseudocódigo-e-algoritmos)
4. [Apresentação do Curso](#4-apresentação-do-curso)
5. [Configuração do Ambiente de Desenvolvimento](#5-configuração-do-ambiente-de-desenvolvimento)

---

## 1. Introdução às Linguagens de Programação

### O que é uma Linguagem de Programação?

Uma linguagem de programação é um sistema de comunicação estruturado que permite aos seres humanos instruir computadores a realizar tarefas específicas. É um conjunto de regras, sintaxe e semântica que possibilita a criação de programas.

**Analogia:** Assim como usamos português para nos comunicar com outras pessoas, usamos linguagens de programação para nos comunicar com computadores.

### Níveis de Linguagens

#### Linguagens de Baixo Nível

Estão próximas da linguagem de máquina (0s e 1s):

**Exemplo de Assembly:**
```assembly
MOV AX, 5
ADD AX, 3
```

**Características:**
- Difícil de ler e escrever
- Controle total sobre o hardware
- Específica para cada processador
- Muito rápida na execução

#### Linguagens de Alto Nível

Mais próximas da linguagem humana:

**Exemplo em Python:**
```python
resultado = 5 + 3
```

**Características:**
- Fácil de ler e escrever
- Portável entre diferentes sistemas
- Abstrai detalhes do hardware
- Foca na lógica do problema

### Por que Python?

Python é considerado uma linguagem de **altíssimo nível** devido à sua sintaxe extremamente legível:

**Comparação entre linguagens:**

```c
// Em C
#include <stdio.h>
int main() {
    printf("Olá, Mundo!\n");
    return 0;
}
```

```java
// Em Java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Olá, Mundo!");
    }
}
```

```python
# Em Python
print("Olá, Mundo!")
```

### Paradigmas de Programação

Python suporta múltiplos paradigmas:

#### Programação Imperativa
Sequência de comandos que alteram o estado do programa:

```python
idade = 18
if idade >= 18:
    print("Você é maior de idade")
else:
    print("Você é menor de idade")
```

#### Programação Orientada a Objetos
Organização do código em objetos que possuem propriedades e comportamentos:

```python
class Pessoa:
    def __init__(self, nome, idade):
        self.nome = nome
        self.idade = idade
    
    def apresentar(self):
        print(f"Olá, meu nome é {self.nome}")
```

#### Programação Funcional
Uso de funções como elementos principais:

```python
def dobro(numero):
    return numero * 2

numeros = [1, 2, 3, 4, 5]
dobrados = list(map(dobro, numeros))
# Resultado: [2, 4, 6, 8, 10]
```

### Aplicações Práticas de Python

| Área | Aplicação | Exemplos |
|------|-----------|----------|
| **Web Development** | Sites e aplicações web | Instagram, Spotify, YouTube |
| **Data Science** | Análise de dados | Pandas, NumPy, Matplotlib |
| **Machine Learning** | Inteligência Artificial | TensorFlow, scikit-learn |
| **Automação** | Scripts e tarefas repetitivas | Web scraping, processamento de arquivos |
| **Games** | Desenvolvimento de jogos | Pygame |
| **DevOps** | Infraestrutura e deploy | Ansible, AWS CLI |

---

## 2. História e Evolução do Python

### A Criação

**Guido van Rossum**, programador holandês, criou Python em **1991** no Instituto de Pesquisa Nacional para Matemática e Ciência da Computação (CWI) na Holanda.

**Curiosidade:** O nome "Python" não vem da cobra, mas sim do grupo de comédia britânico **Monty Python's Flying Circus**, do qual Guido era grande fã!

### A Filosofia Python

Em 1999, Tim Peters escreveu **The Zen of Python** - 19 princípios que guiam o desenvolvimento em Python:

```python
import this
```

**Principais princípios:**

> **Beautiful is better than ugly.**  
> Bonito é melhor que feio.

> **Explicit is better than implicit.**  
> Explícito é melhor que implícito.

> **Simple is better than complex.**  
> Simples é melhor que complexo.

> **Readability counts.**  
> Legibilidade conta.

**Exemplo prático:**

```python
# Forma explícita e legível (Pythonic)
total = 0
for numero in numeros:
    total += numero

# Menos legível
t=0;[t:=t+n for n in nums]
```

### Linha do Tempo

```
1991  - Python 0.9.0 (primeira versão)
1994  - Python 1.0 (lambda, map, filter, reduce)
2000  - Python 2.0 (list comprehensions, garbage collector)
2008  - Python 3.0 (grande revisão, não retrocompatível)
2020  - Python 2.7 descontinuado
2023  - Python 3.12 (melhorias de performance)
2024  - Python 3.13 (compilador JIT experimental)
```

### Python 2 vs Python 3

**Python 2** (descontinuado em 2020):
```python
print "Olá, Mundo!"  # sem parênteses
```

**Python 3** (versão atual):
```python
print("Olá, Mundo!")  # com parênteses
```

**Outras diferenças importantes:**

```python
# Python 2
5 / 2  # Resultado: 2 (divisão inteira)

# Python 3
5 / 2  # Resultado: 2.5 (divisão real)
5 // 2 # Resultado: 2 (divisão inteira explícita)
```

### Python no Mercado Atual

**Estatísticas (2024):**

- **3ª linguagem mais popular** no GitHub
- **1ª linguagem** em Data Science e Machine Learning
- **Crescimento de 40%** em vagas de emprego nos últimos 3 anos
- Usada por **gigantes da tecnologia**: Google, Facebook, Netflix, NASA

**Salários médios no Brasil (2024):**
- Júnior: R$ 3.000 - R$ 5.000
- Pleno: R$ 6.000 - R$ 10.000
- Sênior: R$ 12.000 - R$ 20.000+

---

## 3. Conceito de Pseudocódigo e Algoritmos

### O que é um Algoritmo?

Um algoritmo é uma sequência finita de passos bem definidos para resolver um problema ou realizar uma tarefa.

**Características de um algoritmo:**
1. **Finito** - deve terminar em algum momento
2. **Definido** - passos claros e não ambíguos
3. **Entrada** - recebe dados (pode ser zero ou mais)
4. **Saída** - produz resultado
5. **Efetivo** - cada passo deve ser executável

### Algoritmos do Cotidiano

#### Exemplo 1: Fazer um Café

```
Algoritmo: FazerCafé
Entrada: Café em pó, água, filtro
Saída: Café pronto

Início
    1. Pegar o suporte do filtro
    2. Colocar o filtro de papel
    3. Adicionar 2 colheres de café em pó
    4. Ferver 500ml de água
    5. Despejar água quente lentamente
    6. Aguardar o café coar completamente
    7. Servir na xícara
Fim
```

#### Exemplo 2: Calcular Média de Notas

```
Algoritmo: CalcularMédia
Entrada: nota1, nota2, nota3
Saída: média

Início
    1. Ler nota1
    2. Ler nota2
    3. Ler nota3
    4. soma ← nota1 + nota2 + nota3
    5. média ← soma / 3
    6. Mostrar média
Fim
```

### O que é Pseudocódigo?

Pseudocódigo é uma forma de escrever algoritmos usando uma linguagem intermediária entre a linguagem natural e a linguagem de programação.

**Vantagens:**
- Foca na lógica, não na sintaxe
- Facilita o planejamento antes de codificar
- Independente de linguagem de programação
- Mais fácil de entender e revisar

### Estruturas Básicas em Pseudocódigo

#### Entrada e Saída

```
LEIA variável
ESCREVA "mensagem"
ESCREVA variável
```

**Exemplo:**
```
LEIA nome
ESCREVA "Olá, ", nome
```

#### Atribuição

```
variável ← valor
```

**Exemplo:**
```
idade ← 25
nome ← "João"
preco ← 49.90
```

#### Estruturas Condicionais

```
SE condição ENTÃO
    comandos
SENÃO
    comandos
FIM SE
```

**Exemplo:**
```
LEIA idade
SE idade >= 18 ENTÃO
    ESCREVA "Maior de idade"
SENÃO
    ESCREVA "Menor de idade"
FIM SE
```

#### Estruturas de Repetição

**Enquanto (while):**
```
ENQUANTO condição FAÇA
    comandos
FIM ENQUANTO
```

**Para (for):**
```
PARA variável DE início ATÉ fim FAÇA
    comandos
FIM PARA
```

**Exemplo completo:**
```
PARA i DE 1 ATÉ 10 FAÇA
    ESCREVA i
FIM PARA
```

### Do Pseudocódigo ao Python

Vamos converter um algoritmo em pseudocódigo para Python:

**Pseudocódigo:**
```
Algoritmo: VerificarParImpar
Entrada: numero
Saída: "Par" ou "Ímpar"

Início
    LEIA numero
    SE numero % 2 = 0 ENTÃO
        ESCREVA "Par"
    SENÃO
        ESCREVA "Ímpar"
    FIM SE
Fim
```

**Python:**
```python
# Verificar se número é par ou ímpar
numero = int(input("Digite um número: "))

if numero % 2 == 0:
    print("Par")
else:
    print("Ímpar")
```

### Exercício Prático

**Desafio:** Criar um algoritmo em pseudocódigo para:

**Problema:** Calcular a área de um retângulo

**Solução em Pseudocódigo:**
```
Algoritmo: CalcularÁreaRetângulo
Entrada: base, altura
Saída: área

Início
    LEIA base
    LEIA altura
    área ← base * altura
    ESCREVA "A área é: ", área
Fim
```

**Solução em Python:**
```python
# Calcular área do retângulo
base = float(input("Digite a base: "))
altura = float(input("Digite a altura: "))

area = base * altura

print(f"A área é: {area}")
```


### Expectativas e Dicas de Sucesso

**Para ter sucesso no curso:**

1. **Pratique diariamente** - Programação é como um esporte, requer prática constante
2. **Não tenha medo de errar** - Erros são parte do aprendizado
3. **Colabore** - Ajude e peça ajuda aos colegas
4. **Seja curioso** - Explore além do conteúdo da aula
5. **Faça anotações** - Documente seu aprendizado
6. **Tire dúvidas** - Não deixe dúvidas acumularem
7. **Desenvolva projetos pessoais** - Aplique o que aprende em projetos próprios

---

## 5. Configuração do Ambiente de Desenvolvimento

Você pode programar em Python de diversas formas:

#### Opção 1: Python + IDLE (Mais Simples)
- IDE nativa do Python
- Leve e fácil de usar
- Ideal para iniciantes

#### Opção 2: Visual Studio Code (Recomendado)
- Editor poderoso e gratuito
- Muitos recursos e extensões
- Usado profissionalmente

#### Opção 3: PyCharm Community
- IDE completa para Python
- Muitos recursos profissionais
- Versão gratuita disponível

#### Opção 4: Ambientes Online
- Google Colab (gratuito, não requer instalação)
- Replit (gratuito, interface simples)

### Entendendo o Primeiro Programa

```python
print("Olá, Mundo!")
```

**Análise:**

- `print()` - função que exibe texto na tela
- `"Olá, Mundo!"` - string (texto) entre aspas
- `()` - parênteses obrigatórios em funções Python 3

### Variações do Olá, Mundo!

#### Variação 1: Múltiplas Linhas

```python
print("Olá, Mundo!")
print("Bem-vindo ao Python!")
print("Vamos aprender programação!")
```

**Saída:**
```
Olá, Mundo!
Bem-vindo ao Python!
Vamos aprender programação!
```

#### Variação 2: Personalização

```python
nome = "João"
print("Olá,", nome)
print("Bem-vindo ao curso de Python!")
```

**Saída:**
```
Olá, João
Bem-vindo ao curso de Python!
```

#### Variação 3: Formatação

```python
nome = "Maria"
idade = 20
print(f"Olá, meu nome é {nome} e tenho {idade} anos")
```

**Saída:**
```
Olá, meu nome é Maria e tenho 20 anos
```

#### Variação 4: Caracteres Especiais

```python
print("=" * 40)
print("    BEM-VINDO AO PYTHON!")
print("=" * 40)
```

**Saída:**
```
========================================
    BEM-VINDO AO PYTHON!
========================================
```

### Exercícios Práticos

#### Exercício 1: Apresentação Pessoal

Crie um programa que exiba:
- Seu nome
- Sua idade
- Sua cidade
- O que você espera aprender

**Exemplo de solução:**

```python
nome = "Carlos Silva"
idade = 22
cidade = "Benjamin Constant"
objetivo = "criar aplicações web"

print("=" * 50)
print("         APRESENTAÇÃO PESSOAL")
print("=" * 50)
print(f"Nome: {nome}")
print(f"Idade: {idade} anos")
print(f"Cidade: {cidade}")
print(f"Objetivo: {objetivo}")
print("=" * 50)
```

#### Exercício 2: Calculadora Simples

Crie um programa que some dois números:

```python
numero1 = 10
numero2 = 25
soma = numero1 + numero2

print(f"{numero1} + {numero2} = {soma}")
```

#### Exercício 3: Mensagem Criativa

Crie uma mensagem criativa usando print():

```python
print("    /\\_/\\  ")
print("   ( o.o ) ")
print("    > ^ <  ")
print("Olá! Sou um gato programador!")
```

### Recursos Adicionais

#### Documentação Oficial
- https://docs.python.org/pt-br/3/

#### Tutoriais Interativos
- https://www.learnpython.org/
- https://www.codecademy.com/learn/learn-python-3


#### Canais no YouTube
- Curso em Vídeo - Python
- Otávio Miranda

---

## Atividades para Casa

### Tarefa 1: Prática

Crie os seguintes programas:

1. Um programa que exiba seu nome
2. Um programa que calcule e exiba a soma de três números


### Tarefa 3: Pesquisa

Pesquise e anote:
- 3 empresas que usam Python
- 3 áreas de atuação com Python
- 1 projeto interessante feito em Python

---

## Recapitulando

Nesta aula você aprendeu:

- O que são linguagens de programação e seus níveis
- A história e evolução do Python
- Por que Python é tão popular
- O conceito de algoritmos e pseudocódigo
- Como converter pseudocódigo para Python
- Os objetivos e estrutura do curso
- Como configurar o ambiente de desenvolvimento
- Como criar seu primeiro programa em Python

---

## Contato

**Docente:** Marcos Jhollyfer Felix Rodrigues  
**Instituição:** CETAM - Benjamin Constant  
**Período:** 06/10/2025 a 04/11/2025

---

*Material elaborado para o Curso de Qualificação Profissional em Linguagem de Programação Python - CETAM 2025*
