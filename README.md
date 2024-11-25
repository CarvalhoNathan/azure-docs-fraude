# 💳 Azure Fraud Detection with OCR

Este projeto utiliza os serviços **Storage Account** e **Document Intelligence** da Azure para detectar documentos fraudulentos. A solução usa OCR (Reconhecimento Óptico de Caracteres) para analisar imagens de documentos, verificando se os cartões de crédito são válidos ou inválidos, com base nas informações extraídas da imagem.

---

## 📑 Índice
- [Introdução](#-introdução)
- [Tecnologias Utilizadas](#️-tecnologias-utilizadas)
- [Funcionalidades](#-funcionalidades)
- [Como Usar](#️-como-usar)
- [Resultados](#-resultados)

---

## 📌 Introdução

Fraudes envolvendo cartões de crédito representam um grande desafio no mercado financeiro. Este projeto foi desenvolvido para verificar a validade de cartões de crédito a partir de imagens ou documentos digitalizados. Utilizando OCR com **Document Intelligence**, o sistema lê as informações do cartão de crédito e valida sua autenticidade, enquanto o **Storage Account** da Azure é utilizado para armazenamento seguro das imagens enviadas.

---

## ⚙️ Tecnologias Utilizadas

- [Azure Storage Account](https://azure.microsoft.com/en-us/products/storage/)
- [Azure Document Intelligence (OCR)](https://azure.microsoft.com/en-us/products/cognitive-services/document-intelligence/)
- Python

---

## 🚀 Funcionalidades

- **Upload de Imagens**: O usuário pode enviar uma imagem do cartão de crédito ou utilizar um dispositivo com câmera para capturar a imagem.
- **OCR (Reconhecimento de Texto)**: O serviço de OCR do **Document Intelligence** é utilizado para extrair os dados do cartão de crédito da imagem.
- **Validação do Cartão**: A autenticidade do cartão é verificada automaticamente, retornando se o cartão é **Válido** ou **Inválido**.
- **Armazenamento Seguro**: As imagens são armazenadas no **Azure Storage** de forma segura.

---

## 🛠️ Como Usar

1. **Clone este repositório**:
   ```bash
   git clone https://github.com/seu-usuario/azure-fraud-detection.git
   cd azure-fraud-detection
   ```

2. **Configure suas chaves de API da Azure**:
   - Adicione as credenciais para o **Storage Account** e **Document Intelligence** no arquivo `.env` ou diretamente no código.

3. **Execute o script de validação**:
   - Envie a imagem do cartão de crédito **(FAKE)**
   - O OCR irá processar a imagem e extrair os dados do cartão.

4. **Visualize os resultados**:
   - O sistema retornará se o cartão é **Válido** ou **Inválido** com base nos dados extraídos.

---

## 📊 Resultados

O sistema fornece uma análise precisa e rápida, determinando se o cartão de crédito é válido ou inválido com base nas informações extraídas das imagens. Exemplos de outputs incluem:

- **Cartão Válido**: "Este cartão de crédito é válido."
- **Cartão Inválido**: "Este cartão de crédito não é válido."

---

## 🤝 Contribuições

Contribuições são bem-vindas! Abra uma issue ou envie um pull request com sugestões de melhorias.

---

## 📄 Licença

Este projeto é licenciado sob a [MIT License](LICENSE).
