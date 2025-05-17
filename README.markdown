# CondominAI 

![CondominAI Logo](https://github.com/VictorsCodes/CondominAI/blob/main/Logo.png?raw=true)

CondominAI é uma ferramenta em Python para análise de faturas em PDF de condomínio, energia, água, cartão de crédito, telefonia, etc, hospedada no Google Colab. Utiliza a API do Google Gemini para extrair e comparar dados financeiros, oferecendo resumos e respostas a perguntas sobre as faturas.

## Funcionalidades

- **Agente 1: Coletor de Faturas** 📂: Lista PDFs na pasta do Google Drive.
- **Agente 2: Analisador de Faturas** 🔍: Extrai valores (ex.: Valor do Doc, Rateio) de PDFs.
- **Agente 3: Resumidor de Faturas** 📋: Resume dados de uma fatura ou compara múltiplas.
- **Agente 4: Pergunte ao CondominAI** 🤖: Responde perguntas sobre faturas em linguagem natural.

## Pré-requisitos

- Conta no Google Colab.
- Acesso ao Google Drive.
- Chave da API Google Gemini (`GOOGLE_API_KEY`).
- Python 3.7+ com bibliotecas:
  - `google-generativeai`
  - `PyPDF2`
  - `pandas`
  - `IPython`

## Configuração

1. **Clone o repositório**:

   ```bash
   git clone https://github.com/VictorsCodes/condominai.git
   ```

2. **Configure a API Key**:

   - Adicione sua chave `GOOGLE_API_KEY` nos segredos do Colab (Settings > Secrets).

3. **Monte o Google Drive**:

   - No Colab, execute o código para montar o Drive em `/content/drive`.

4. **Adicione faturas**:

   - Coloque PDFs das faturas em `/content/drive/MyDrive/CondominAI/Faturas de Condomínio`.

     ![Fatura_Upload](https://raw.githubusercontent.com/VictorsCodes/CondominAI/refs/heads/main/Upload_Fatura.png)

## Uso

1. Abra o notebook `condominai.ipynb` no Google Colab.
2. Execute as células para instalar dependências e rodar o script.
3. Escolha o modo:
   - **1**: Analisar uma única fatura.
   - **2**: Comparar duas ou mais faturas.
4. Siga as instruções para selecionar faturas e fazer perguntas.

### Exemplo de Saída

```
✅ Sucesso! A pasta 'Faturas de Condomínio' foi criada.
📑 Faturas disponíveis:
1. Fatura_Março_2025.pdf
2. Fatura_Abril_2025.pdf
👆 Selecione a fatura para análise:
```

## Estrutura do Projeto

- `condominai.ipynb`: Notebook principal com o código.
- `/Faturas de Condomínio/`: Pasta no Google Drive para PDFs.

## Contribuição

1. Faça um fork do repositório.
2. Crie uma branch (`git checkout -b feature/nova-funcionalidade`).
3. Envie um pull request com suas alterações.

## Licença

MIT License. Veja LICENSE para detalhes.

## Contato

Dúvidas? Abra uma issue.
