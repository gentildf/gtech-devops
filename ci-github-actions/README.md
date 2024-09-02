
# Desafio de Integração Contínua com GitHub Actions

Este repositório contém um projeto simples em [Python/Node.js] com um pipeline de Integração Contínua (CI) configurado usando GitHub Actions. O pipeline inclui etapas de linting, testes automatizados, e uma build opcional.

## Estrutura do Projeto

- **src/**: Código-fonte do projeto.
- **tests/**: Testes automatizados.
- **.github/workflows/**: Configuração do pipeline CI.
- **requirements.txt / package.json**: Arquivo de dependências.

## Como Usar

Para rodar os testes localmente:

- **Python**:
    ```bash
    pip install -r requirements.txt
    pytest
    ```

- **Node.js**:
    ```bash
    npm install
    npm test
    ```

## Pipeline CI

O pipeline de Integração Contínua (CI) é automaticamente executado em cada push ou pull request. Ele realiza as seguintes etapas:

1. **Linting**: Verifica o código em busca de problemas de formatação ou erros.
2. **Testes Automatizados**: Executa os testes para garantir que o código esteja funcionando corretamente.
3. **Build (opcional)**: Gera uma build do projeto, se aplicável.

## Objetivo

Este desafio visa demonstrar conhecimento básico de CI/CD, GitHub Actions, e como integrar testes automatizados em um pipeline.
