
# Desafio de Integração Contínua com GitHub Actions

Este repositório contém um projeto simples em Python com um pipeline de Integração Contínua (CI) configurado usando GitHub Actions. O pipeline inclui etapas de linting, testes automatizados, e uma build opcional. Porém, neste caso, será utilizado apenas a parte de testes automatizados.

## Estrutura do Projeto

- **src/**: Código-fonte do projeto.
- **tests/**: Testes automatizados.
- **.github/workflows/**: Configuração do pipeline CI.
- **requirements.txt**: Arquivo de dependências.

## Requisitos do Ambiente

- Python 3.8 ou superior
- Git

## Como Configurar o Ambiente

### Instalar Python

1. Certifique-se de ter o Python instalado na sua máquina. Para verificar, execute:
   ```bash
   python --version
   ```
   - Se Python não estiver instalado, baixe e instale a versão mais recente em [python.org](https://www.python.org/downloads/).

### Criar um Ambiente Virtual

1. Crie um ambiente virtual (recomendado) para isolar as dependências do projeto:
   ```bash
   python -m venv venv
   ```

2. Ative o ambiente virtual:

   - **No Linux/MacOS**:
     ```bash
     source venv/bin/activate
     ```
   - **No Windows**:
     ```bash
     .\venv\Scripts\activate
     ```

### Instalar Dependências

1. Instale as dependências necessárias para rodar o projeto, incluindo `pytest`:
   ```bash
   pip install -r requirements.txt
   ```

   Certifique-se de que o arquivo `requirements.txt` inclua a linha:
   ```plaintext
   pytest
   ```

## Como Usar

### Executar os Testes

1. Certifique-se de estar no ambiente virtual (veja a seção "Como Configurar o Ambiente").
2. Execute os testes:
   ```bash
   pytest tests/
   ```

## Pipeline CI

O pipeline de Integração Contínua (CI) é automaticamente executado em cada push ou pull request. Ele realiza a seguinte etapa:

1. **Testes Automatizados**: Executa os testes para garantir que o código esteja funcionando corretamente.

Observação: As etapas de build ou verificação de código não foram incluídas para simplificar o exercício.

## Objetivo

Este desafio visa demonstrar conhecimento básico de CI/CD, GitHub Actions, e como integrar testes automatizados em um pipeline.
