# Projeto de Tradução de Textos com API da Microsoft

Este projeto é uma aplicação em Python que realiza a tradução de textos em inglês para um idioma alvo especificado, utilizando a API **Microsoft Translator**. A aplicação permite que desenvolvedores integrem traduções automáticas em seus próprios projetos, facilitando a criação de soluções multilíngues.

## Funcionalidades

- **Tradução Automática**: Traduz textos em inglês para o idioma alvo especificado.
- **API da Microsoft Translator**: Integração com o Microsoft Translator usando a API do Azure.
- **Tratamento de Erros**: Verificação de erros de requisição e formato de resposta para garantir uma execução segura e estável.

## Tecnologias

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)

![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)

![Azure](https://img.shields.io/badge/azure-%230072C6.svg?style=for-the-badge&logo=microsoftazure&logoColor=white)

![ChatGPT](https://img.shields.io/badge/chatGPT-74aa9c?style=for-the-badge&logo=openai&logoColor=white)

## Requisitos

Antes de começar, certifique-se de ter instalado:

- Python 3.6 ou superior
- As bibliotecas Python listadas no arquivo `requirements.txt` (ou instale diretamente com `pip install requests python-docx`).

Além disso, você precisará de uma **chave de assinatura válida** e do **endpoint** da API do Microsoft Translator. Esses dados podem ser obtidos ao configurar o recurso no [Azure Portal](https://portal.azure.com/).

## Instalação

1. Clone o repositório para sua máquina local:

   ```bash
   git clone https://github.com/seuusuario/seu-repositorio.git

   cd seu-repositorio

2. Instale as dependências do projeto:

    ```bash
    pip install -r requirements.


3. Configure sua chave de assinatura da API, região e endpoint no código

    ```bash
    subscription_key = "sua_chave_de_assinatura"
    endpoint = "https://api.cognitive.microsofttranslator.com/"
    location = "sua_regiao"

## Uso

A função principal do projeto é `translator_text`, que recebe um texto em inglês e o idioma de destino e retorna a tradução. Veja abaixo um exemplo de uso:

    ```python
    from seu_script import translator_text

    text_to_translate = "I know you're somewhere out there, somewhere far away"
    target_language = "pt-br"  # Português

    translation = translator_text(text_to_translate, target_language)
    print("Tradução:", translation)

## Exemplo de Saída

![imagem](./src/image/text-traslater.png)

## Tratamento de Erros

O projeto verifica o status das respostas da API e lida com possíveis erros de formato. Em caso de erro, uma mensagem detalhada será exibida no console.

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir uma issue ou enviar um pull request.

## Licença

Este projeto é licenciado sob a MIT License.

Esse README.md fornece uma visão geral clara e orientações para instalação e uso, facilitan
