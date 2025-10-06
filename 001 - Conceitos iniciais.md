# Aula 01 - Introdução ao Mundo da Programação com Python

**Centro de Educação Tecnológica do Amazonas - CETAM**  
**Curso:** Qualificação Profissional em Linguagem de Programação Python  
**Data:** 06/10/2025 | **Carga Horária:** 4 horas

---

## Bem-vindo ao Mundo da Programação!

Hoje você dará os primeiros passos em uma jornada empolgante. Vamos descobrir juntos o que é programação, conhecer a linguagem Python e aprender como transformar ideias em instruções que o computador pode executar.

---

## Sumário

1. [Introdução às Linguagens de Programação](#1-introdução-às-linguagens-de-programação)
2. [História e Evolução do Python](#2-história-e-evolução-do-python)
3. [Conceito de Pseudocódigo e Algoritmos](#3-conceito-de-pseudocódigo-e-algoritmos)
4. [Atividades Práticas](#4-atividades-práticas)

---

## 1. Introdução às Linguagens de Programação

### O que é Programação?

Programação é a arte de ensinar o computador a fazer coisas. É como escrever uma receita de bolo, mas em vez de instruir uma pessoa, você instrui uma máquina.

**Pense assim:**
- Quando você diz para um amigo "vá até a padaria e compre pão", ele entende naturalmente
- Um computador precisa de instruções muito mais detalhadas e precisas
- A programação é a linguagem que usamos para dar essas instruções

### O que é uma Linguagem de Programação?

Uma linguagem de programação é um conjunto de regras e palavras especiais que usamos para nos comunicar com o computador.

**Analogia simples:**
- Português é a língua que usamos para falar com pessoas brasileiras
- Inglês é a língua que usamos para falar com pessoas de outros países
- Python é a "língua" que usamos para falar com computadores

### Como o Computador Entende?

Os computadores só entendem uma linguagem: **zeros e uns** (linguagem binária).

```
01001000 01100101 01101100 01101100 01101111
```

Isso significa "Hello" em binário!

Mas imagina ter que escrever assim? Seria muito difícil! Por isso existem as linguagens de programação.

### Níveis de Linguagens

#### Linguagens de Baixo Nível

Estão mais próximas da linguagem que o computador entende diretamente.

**Exemplo - Assembly:**
```assembly
MOV AX, 5
ADD AX, 3
```

**Características:**
- Difícil de escrever e entender
- Muito próxima do hardware
- Usada em situações muito específicas

#### Linguagens de Alto Nível

Estão mais próximas da linguagem humana, mais fáceis de ler e escrever.

**Exemplo - Python:**
```python
resultado = 5 + 3
```

**Características:**
- Fácil de ler e escrever
- Mais próxima da linguagem natural
- Funciona em diferentes computadores
- É o que vamos aprender!

### Comparando Linguagens

Vamos ver como diferentes linguagens fazem a mesma coisa: mostrar "Olá, Mundo!" na tela.

**Em C:**
```c
#include <stdio.h>
int main() {
    printf("Olá, Mundo!\n");
    return 0;
}
```

**Em Java:**
```java
public class OlaMundo {
    public static void main(String[] args) {
        System.out.println("Olá, Mundo!");
    }
}
```

**Em Python:**
```python
print("Olá, Mundo!")
```

Viu a diferença? Python é muito mais simples e direto!

### Por que Aprender Programação?

1. **Resolver Problemas do Dia a Dia**
   - Automatizar tarefas repetitivas
   - Organizar informações
   - Criar soluções personalizadas

2. **Oportunidades Profissionais**
   - Alta demanda no mercado
   - Bons salários
   - Trabalho remoto possível

3. **Desenvolver o Raciocínio**
   - Pensar de forma lógica
   - Decompor problemas complexos
   - Criar soluções criativas

4. **Criar Suas Próprias Ferramentas**
   - Aplicativos
   - Websites
   - Jogos
   - Análise de dados

### Onde a Programação é Usada?

**Você usa programação todos os dias, mesmo sem perceber:**

- **Celular:** Todos os aplicativos foram programados
- **Redes Sociais:** Instagram, Facebook, TikTok
- **Streaming:** Netflix, Spotify, YouTube
- **Jogos:** Fortnite, Free Fire, Minecraft
- **Banco:** Aplicativo do seu banco
- **Transporte:** Uber, 99, aplicativos de ônibus

**Tudo que é digital foi programado por alguém!**

---

## 2. História e Evolução do Python

### A Criação do Python

Python foi criado por **Guido van Rossum**, um programador holandês, no final de 1989, e lançado em 1991.

**Curiosidade:** O nome "Python" não vem da cobra! Guido era fã de um grupo de comédia britânico chamado **Monty Python**, e decidiu homenageá-los.

### Por que Guido Criou o Python?

Guido queria criar uma linguagem que fosse:

1. **Fácil de Ler** - O código deveria parecer com inglês (ou português)
2. **Fácil de Aprender** - Iniciantes deveriam conseguir programar rapidamente
3. **Poderosa** - Capaz de fazer coisas complexas de forma simples
4. **Divertida** - Programar deveria ser prazeroso, não frustrante

### A Filosofia do Python: The Zen of Python

Em 1999, Tim Peters escreveu 19 princípios que guiam a programação em Python. Você pode vê-los digitando:

```python
import this
```

**Os mais importantes para iniciantes:**

> **Bonito é melhor que feio**
> O código deve ser agradável de ler

> **Simples é melhor que complexo**
> Sempre busque a solução mais simples

> **Legibilidade conta**
> Outras pessoas precisam entender seu código

> **Erros nunca devem passar silenciosamente**
> É melhor saber quando algo dá errado

**Exemplo prático:**

```python
# Forma Pythônica (boa)
nome = "Maria"
idade = 20
print(f"{nome} tem {idade} anos")

# Forma complicada (ruim)
n="Maria";i=20;print(n+" tem "+str(i)+" anos")
```

### Linha do Tempo do Python

```
1989  - Guido começa a trabalhar no Python
1991  - Python 0.9.0 lançado (primeira versão)
1994  - Python 1.0 lançado
2000  - Python 2.0 lançado
2008  - Python 3.0 lançado (grande mudança!)
2020  - Python 2 é descontinuado
2024  - Python 3.12 (versão atual)
2025  - Python continua crescendo!
```

### Python 2 vs Python 3

**Python 2** (não usamos mais):
```python
print "Olá"  # sem parênteses
```

**Python 3** (o que vamos aprender):
```python
print("Olá")  # com parênteses
```

**Outras diferenças importantes:**

```python
# Python 2
5 / 2    # resultado: 2

# Python 3
5 / 2    # resultado: 2.5
5 // 2   # resultado: 2 (divisão inteira)
```

### Por que Python é Tão Popular?

Python se tornou uma das linguagens mais populares do mundo. Veja por quê:

#### 1. Fácil de Aprender

```python
# Isso é tudo que você precisa para começar!
print("Olá, Mundo!")
```

#### 2. Versátil

Python pode fazer quase tudo:

**Sites e Aplicações Web:**
- Instagram (mais de 2 bilhões de usuários)
- Spotify (serviço de música)
- YouTube (maior site de vídeos)
- Pinterest (rede social de imagens)

**Ciência de Dados e Análise:**
- Analisar dados de vendas
- Prever tendências
- Criar gráficos e visualizações

**Inteligência Artificial:**
- ChatGPT
- Reconhecimento facial
- Carros autônomos
- Recomendações da Netflix

**Automação:**
- Organizar arquivos automaticamente
- Enviar emails em massa
- Processar planilhas

**Jogos:**
- Pygame para criar jogos 2D
- Scripts para Minecraft

#### 3. Grande Comunidade

- Milhões de programadores ao redor do mundo
- Muitos tutoriais e cursos gratuitos
- Fácil encontrar ajuda quando tiver dúvidas

#### 4. Bibliotecas Poderosas

Python tem "ferramentas prontas" para quase tudo:

| Biblioteca | Para que serve |
|------------|----------------|
| **NumPy** | Cálculos matemáticos |
| **Pandas** | Análise de dados |
| **Matplotlib** | Criar gráficos |
| **Django** | Criar websites |
| **TensorFlow** | Inteligência Artificial |
| **Pygame** | Criar jogos |

### Python no Mercado de Trabalho

**Estatísticas interessantes:**

- Python é a **3ª linguagem mais usada** no mundo
- É a **número 1** em Data Science e IA
- Vagas cresceram **40%** nos últimos 3 anos

**Salários no Brasil (2024):**
- Iniciante: R$ 3.000 - R$ 5.000
- Intermediário: R$ 6.000 - R$ 10.000
- Avançado: R$ 12.000 - R$ 20.000+

### Empresas que Usam Python

**Gigantes da Tecnologia:**
- Google (buscador)
- Netflix (streaming)
- NASA (exploração espacial)
- Uber (transporte)
- Dropbox (armazenamento)
- Reddit (rede social)

---

## 3. Conceito de Pseudocódigo e Algoritmos

### O que é um Algoritmo?

Um algoritmo é uma sequência de passos para resolver um problema ou realizar uma tarefa.

**Você já usa algoritmos no dia a dia!**

#### Algoritmo 1: Escovar os Dentes

```
1. Pegar a escova de dentes
2. Pegar o creme dental
3. Abrir o creme dental
4. Colocar creme dental na escova
5. Fechar o creme dental
6. Abrir a torneira
7. Molhar a escova
8. Escovar os dentes (2 minutos)
9. Enxaguar a boca
10. Lavar a escova
11. Fechar a torneira
```

Isso é um algoritmo! Uma sequência clara de passos.

#### Algoritmo 2: Fazer um Sanduíche

```
1. Pegar duas fatias de pão
2. Pegar a manteiga
3. Passar manteiga em uma fatia
4. Pegar o queijo
5. Colocar queijo em cima da manteiga
6. Pegar o presunto
7. Colocar presunto em cima do queijo
8. Cobrir com a outra fatia de pão
9. Sanduíche pronto!
```

### Características de um Bom Algoritmo

Um algoritmo deve ser:

1. **Finito** - Deve terminar em algum momento
2. **Claro** - Cada passo deve ser bem definido
3. **Com Entrada** - Recebe informações (pode ser zero)
4. **Com Saída** - Produz um resultado
5. **Efetivo** - Cada passo deve ser possível de executar

### Algoritmos na Programação

Vamos ver um algoritmo computacional simples:

#### Exemplo: Calcular a Média de Duas Notas

**Em português:**
```
1. Perguntar a primeira nota
2. Guardar a resposta
3. Perguntar a segunda nota
4. Guardar a resposta
5. Somar as duas notas
6. Dividir o resultado por 2
7. Mostrar a média
```

### O que é Pseudocódigo?

Pseudocódigo é uma forma de escrever algoritmos que está entre a linguagem natural (português) e a linguagem de programação.

**Por que usar pseudocódigo?**
- Foca na lógica, não na sintaxe
- Mais fácil de entender
- Facilita planejar antes de programar
- Funciona para qualquer linguagem

### Estrutura Básica do Pseudocódigo

#### Entrada e Saída

```
LEIA variável
ESCREVA "mensagem"
ESCREVA variável
```

**Exemplo:**
```
ESCREVA "Qual é o seu nome?"
LEIA nome
ESCREVA "Olá, ", nome
```

#### Variáveis (Guardar Informações)

```
nome ← "João"
idade ← 15
altura ← 1.65
```

O símbolo `←` significa "recebe" ou "guarda"

#### Operações Matemáticas

```
soma ← 10 + 5        // resultado: 15
diferenca ← 10 - 5   // resultado: 5
produto ← 10 * 5     // resultado: 50
divisao ← 10 / 5     // resultado: 2
```

### Algoritmos Simples em Pseudocódigo

#### Exemplo 1: Somar Dois Números

```
Algoritmo: SomarDoisNumeros
Entrada: numero1, numero2
Saída: soma

Início
    ESCREVA "Digite o primeiro número:"
    LEIA numero1
    
    ESCREVA "Digite o segundo número:"
    LEIA numero2
    
    soma ← numero1 + numero2
    
    ESCREVA "A soma é:", soma
Fim
```

#### Exemplo 2: Verificar se é Maior de Idade

```
Algoritmo: VerificarIdade
Entrada: idade
Saída: mensagem

Início
    ESCREVA "Digite sua idade:"
    LEIA idade
    
    SE idade >= 18 ENTÃO
        ESCREVA "Você é maior de idade"
    SENÃO
        ESCREVA "Você é menor de idade"
    FIM SE
Fim
```

#### Exemplo 3: Calcular Área de um Retângulo

```
Algoritmo: CalcularAreaRetangulo
Entrada: base, altura
Saída: area

Início
    ESCREVA "Digite a base do retângulo:"
    LEIA base
    
    ESCREVA "Digite a altura do retângulo:"
    LEIA altura
    
    area ← base * altura
    
    ESCREVA "A área do retângulo é:", area
Fim
```

### Do Pseudocódigo para Python

Agora vamos transformar nossos pseudocódigos em Python!

#### Exemplo 1: Somar Dois Números

**Pseudocódigo:**
```
ESCREVA "Digite o primeiro número:"
LEIA numero1
ESCREVA "Digite o segundo número:"
LEIA numero2
soma ← numero1 + numero2
ESCREVA "A soma é:", soma
```

**Python:**
```python
# Somar dois números
print("Digite o primeiro número:")
numero1 = int(input())

print("Digite o segundo número:")
numero2 = int(input())

soma = numero1 + numero2

print("A soma é:", soma)
```

#### Exemplo 2: Verificar Idade

**Pseudocódigo:**
```
LEIA idade
SE idade >= 18 ENTÃO
    ESCREVA "Maior de idade"
SENÃO
    ESCREVA "Menor de idade"
FIM SE
```

**Python:**
```python
# Verificar se é maior de idade
idade = int(input("Digite sua idade: "))

if idade >= 18:
    print("Maior de idade")
else:
    print("Menor de idade")
```

#### Exemplo 3: Calcular Área

**Pseudocódigo:**
```
LEIA base
LEIA altura
area ← base * altura
ESCREVA area
```

**Python:**
```python
# Calcular área do retângulo
base = float(input("Digite a base: "))
altura = float(input("Digite a altura: "))

area = base * altura

print(f"A área é: {area}")
```

### Tabela de Conversão: Pseudocódigo → Python

| Pseudocódigo | Python |
|--------------|--------|
| `LEIA variável` | `variavel = input()` |
| `ESCREVA "texto"` | `print("texto")` |
| `variavel ← valor` | `variavel = valor` |
| `SE condição ENTÃO` | `if condição:` |
| `SENÃO` | `else:` |
| `FIM SE` | (indentação) |
| `//` comentário | `#` comentário |

---

## 4. Atividades Práticas

### Atividade 1: Criar Algoritmos do Cotidiano

**Objetivo:** Entender como funcionam os algoritmos

**Tarefa:** Escolha uma das atividades abaixo e escreva um algoritmo detalhado:

1. Fazer um café
2. Trocar uma lâmpada
3. Preparar macarrão instantâneo
4. Enviar uma mensagem no WhatsApp

**Exemplo de resposta:**

```
Algoritmo: PrepararMacarraoInstantaneo

1. Pegar uma panela
2. Colocar 600ml de água na panela
3. Colocar a panela no fogão
4. Acender o fogo
5. Esperar a água ferver
6. Abrir o pacote de macarrão
7. Colocar o macarrão na água fervente
8. Mexer o macarrão
9. Esperar 3 minutos
10. Desligar o fogo
11. Colocar o tempero
12. Mexer bem
13. Servir em um prato
14. Macarrão pronto!
```

### Atividade 2: Pseudocódigo

**Objetivo:** Praticar a escrita de pseudocódigo

**Tarefa:** Escreva um algoritmo em pseudocódigo para:

**Problema:** Calcular se uma pessoa pode dirigir (precisa ter 18 anos ou mais)

**Solução:**
```
Algoritmo: VerificarPodeDigirir
Entrada: idade
Saída: mensagem

Início
    ESCREVA "Digite sua idade:"
    LEIA idade
    
    SE idade >= 18 ENTÃO
        ESCREVA "Você pode dirigir!"
    SENÃO
        anos_faltando ← 18 - idade
        ESCREVA "Você não pode dirigir ainda."
        ESCREVA "Faltam", anos_faltando, "anos"
    FIM SE
Fim
```

### Atividade 3: Identificar Erros

**Objetivo:** Desenvolver atenção aos detalhes

**Tarefa:** O algoritmo abaixo tem erros. Encontre e corrija:

```
Algoritmo: CalcularMedia
Entrada: nota1, nota2

Início
    ESCREVA "Digite a primeira nota"
    LEIA nota1
    
    LEIA nota2
    
    media = nota1 + nota2 / 2
    
    IMPRIMIR media
```

**Erros encontrados:**
1. Falta mensagem antes de ler nota2
2. Ordem de operação errada (deveria ser `(nota1 + nota2) / 2`)
3. Usa `IMPRIMIR` em vez de `ESCREVA`

**Versão corrigida:**
```
Algoritmo: CalcularMedia
Entrada: nota1, nota2
Saída: media

Início
    ESCREVA "Digite a primeira nota:"
    LEIA nota1
    
    ESCREVA "Digite a segunda nota:"
    LEIA nota2
    
    media ← (nota1 + nota2) / 2
    
    ESCREVA "A média é:", media
Fim
```

### Atividade 4: Desafio de Lógica

**Objetivo:** Pensar de forma algorítmica

**Problema:** Três pessoas (Ana, Bruno e Carlos) estão em uma fila. Ana não é a primeira. Bruno está entre Ana e Carlos. Em que ordem eles estão?

**Resposta:**
```
1. Bruno não pode ser o primeiro (pois está entre os outros dois)
2. Ana não é a primeira (dado do problema)
3. Logo, Carlos é o primeiro
4. Bruno está entre Carlos e Ana
5. Ordem: Carlos, Bruno, Ana
```

### Atividade 5: Para Casa

Crie algoritmos em pseudocódigo para:

1. **Calcular o dobro de um número**
   - Ler um número
   - Multiplicar por 2
   - Mostrar o resultado

2. **Verificar se um número é positivo ou negativo**
   - Ler um número
   - Verificar se é maior, menor ou igual a zero
   - Mostrar a resposta

3. **Converter temperatura de Celsius para Fahrenheit**
   - Ler temperatura em Celsius
   - Aplicar fórmula: F = C × 1.8 + 32
   - Mostrar temperatura em Fahrenheit

---

## Recapitulando

Nesta aula você aprendeu:

### Sobre Programação
- O que é uma linguagem de programação
- Diferença entre linguagens de baixo e alto nível
- Por que programação é importante
- Onde a programação é usada

### Sobre Python
- História de Guido van Rossum
- Por que Python é fácil de aprender
- Filosofia do Python (The Zen)
- Empresas que usam Python
- Oportunidades no mercado

### Sobre Algoritmos
- O que é um algoritmo
- Características de um bom algoritmo
- Como escrever pseudocódigo
- Como converter pseudocódigo para Python

---

## Dicas para Estudar em Casa

1. **Pratique escrever algoritmos** para tarefas do seu dia a dia
2. **Assista vídeos** sobre Python no YouTube
3. **Leia artigos** sobre programação para iniciantes
4. **Converse** com seus colegas sobre o que aprendeu
5. **Não tenha medo de errar** - erro faz parte do aprendizado!

---

## Recursos Úteis

### Sites para Aprender Mais

- **Python.org** - Site oficial do Python
- **Python Brasil** - Comunidade brasileira
- **W3Schools** - Tutoriais interativos
- **Codecademy** - Curso online gratuito

### Canais no YouTube

- Curso em Vídeo (Gustavo Guanabara)
- Programação Dinâmica
- Eduardo Mendes
- Hashtag Programação

---

## Pensamento Final

> "O primeiro passo é sempre o mais difícil. Mas também é o mais importante. Você deu esse passo hoje!"

Parabéns por começar sua jornada na programação! Python é uma linguagem incrível, e você está no caminho certo para aprender algo que pode mudar sua vida profissional.

Lembre-se: todo programador profissional já foi um iniciante um dia. A diferença está na persistência e na prática constante.

**Vamos juntos nessa jornada!**

---

*Material elaborado para o Curso de Qualificação Profissional em Linguagem de Programação Python - CETAM 2025*
