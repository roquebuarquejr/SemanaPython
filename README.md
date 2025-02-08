# 🚀 5 Dias de Python do Zero

Este repositório documenta meu desafio de **5 dias aprendendo Python do zero**, onde aplico os conceitos na leitura de uma planilha de gastos, criação de gráficos e integração com a OpenAI para análise financeira. Se você também quer aprender Python do zero, siga este guia! 🎯

📺 **Vídeo Intro:** *(Adicione o link aqui)*

---

## 📅 **Dia 1: Instalando o Ambiente de Desenvolvimento**
### 🎯 **Objetivo:** Configurar tudo para começar a programar em Python.

### 🛠 **Passo a passo:**
1. **Baixar e instalar o Python** [(site oficial)](https://www.python.org/)
2. **Instalar um editor de código:**
   - Recomendo **VS Code** ou **PyCharm**
3. **Testar a instalação:**
   ```bash
   python --version  # Verifica se o Python está instalado
   ```
4. **Criar e rodar um script simples:**
   ```python
   print("Olá, mundo! Estou começando com Python!")
   ```

### ✅ **Exercícios:**
1. Crie um script que imprime seu nome e idade.
2. Escreva um programa que exibe a data e hora atual.
3. Faça um script que recebe um número do usuário e o imprime na tela.
4. Teste rodar um programa pelo terminal (`python nome_do_arquivo.py`).
5. Descubra onde o Python está instalado no seu computador e adicione o caminho ao `PATH`.

---

## 📅 **Dia 2: Lógica de Programação em Python**
### 🎯 **Objetivo:** Aprender os conceitos fundamentais da programação.

### 🔹 **Conceitos principais:**
- **Variáveis e Tipos de Dados:** `int`, `float`, `str`, `bool`
- **Entrada e saída de dados:** `input()`, `print()`
- **Operadores Matemáticos e Lógicos:** `+`, `-`, `*`, `/`, `==`, `!=`, `>`, `<`
- **Condicionais (`if`, `else`, `elif`)**
- **Loops (`for`, `while`)**
- **Listas (`list`) e Arrays**

### ✅ **Exercícios:**
1. Crie um programa que pede ao usuário dois números e imprime a soma deles.
2. Faça um programa que recebe um número e diz se ele é par ou ímpar.
3. Crie uma lista com 5 números e imprima cada um usando um `for` loop.
4. Peça a idade do usuário e informe se ele é maior ou menor de idade.
5. Faça um contador que imprime de 1 a 10 usando `while`.

---

## 📅 **Dia 3: Lendo a Planilha de Gastos**
### 🎯 **Objetivo:** Aprender a manipular arquivos de planilha (Excel e CSV) com Python.

### 🛠 **Passo a passo:**
1. **Instalar Pandas e OpenPyXL:**
   ```bash
   pip install pandas openpyxl
   ```
2. **Ler um arquivo CSV:**
   ```python
   import pandas as pd
   df = pd.read_csv("gastos.csv")
   print(df.head())
   ```
3. **Ler um arquivo Excel (.xlsx):**
   ```python
   df = pd.read_excel("gastos.xlsx")
   print(df.head())
   ```
4. **Converter colunas em listas:**
   ```python
   categorias = df["Categoria"].tolist()
   valores = df["Valor"].tolist()
   ```
5. **Somar os gastos por categoria:**
   ```python
   total = sum(valores)
   print(f"Gasto total: R$ {total:.2f}")
   ```

### ✅ **Exercícios:**
1. Liste todas as categorias presentes na planilha.
2. Exiba o maior e o menor gasto registrado.
3. Calcule a média dos gastos.
4. Conte quantos registros existem na planilha.
5. Filtre e exiba apenas os gastos acima de R$ 500.

---

## 📅 **Dia 4: Criando Gráficos dos Dados da Planilha**
### 🎯 **Objetivo:** Visualizar os dados usando gráficos.

### 🛠 **Passo a passo:**
1. **Instalar Matplotlib e Seaborn:**
   ```bash
   pip install matplotlib seaborn
   ```
2. **Criar um gráfico de barras:**
   ```python
   import matplotlib.pyplot as plt
   plt.bar(categorias, valores)
   plt.xlabel("Categorias")
   plt.ylabel("Gastos")
   plt.title("Gastos por Categoria")
   plt.show()
   ```
3. **Criar um gráfico de pizza:**
   ```python
   plt.pie(valores, labels=categorias, autopct='%1.1f%%')
   plt.title("Distribuição dos Gastos")
   plt.show()
   ```

### ✅ **Exercícios:**
1. Crie um gráfico de linha mostrando os gastos ao longo do tempo.
2. Mude as cores e o estilo do gráfico.
3. Adicione uma legenda personalizada ao gráfico.
4. Exiba os 3 maiores gastos do mês.
5. Salve o gráfico gerado como uma imagem (`.png`).

---

## 🚀 **Conclusão**
Este projeto mostrou como iniciar com Python e aplicá-lo para análise financeira! Se gostou, ⭐ este repositório e compartilhe! 😃
