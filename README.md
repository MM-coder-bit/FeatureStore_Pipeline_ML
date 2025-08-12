# Engenharia de Atributos, Feature Store e Pipeline de Machine Learning

Este guia oferece um passo a passo para construir um pipeline de Machine Learning, com foco em **Engenharia de Atributos** e na criação de uma **Feature Store**.

## Introdução

O pipeline é responsável por todo o fluxo de trabalho, desde a extração dos dados até a disponibilização do modelo. Nele, a **Engenharia de Atributos** é a etapa de transformar dados brutos em variáveis úteis para o modelo. A **Feature Store**, por sua vez, é um repositório centralizado que gerencia, armazena e serve esses atributos, garantindo consistência e reuso em diferentes projetos.

---

## Execução do Projeto

Siga os comandos abaixo no terminal para configurar e executar o pipeline.

### Passo a Passo

1.  **Crie um ambiente virtual** para isolar as dependências do projeto. Isso garante que o projeto não interfira em outras configurações do seu sistema.
    ```bash
    python3 -m venv meu_pipeline_ml
    ```

2.  **Ative o ambiente virtual** para começar a trabalhar nele.
    ```bash
    source meu_pipeline_ml/bin/activate
    ```

3.  **Instale as dependências** do projeto a partir do arquivo `requirements.txt`.
    ```bash
    pip install -r requirements.txt
    ```

4.  **Instale o pacote localmente no modo editável**. Este comando é crucial para que o ambiente virtual reconheça e atualize as alterações no código-fonte do seu projeto em tempo real.
    ```bash
    pip install -e .
    ```

5.  **Reative o ambiente virtual**. Este passo garante que todas as variáveis de ambiente e caminhos de execução estejam configurados corretamente após a instalação do pacote local.
    ```bash
    source meu_pipeline_ml/bin/activate
    ```

6.  **Execute o script principal** do seu pipeline.
    ```bash
    python src/main.py
    ```

7.  **Desative o ambiente virtual** ao finalizar o trabalho, retornando ao ambiente global do seu sistema.
    ```bash
    deactivate
    ```