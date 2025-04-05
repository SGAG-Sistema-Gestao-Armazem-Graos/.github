# 🌾 SGAG | Sistema de Gestão de Armazém de Grãos

Projeto desenvolvido em Python com foco na **automação do controle de entrada e saída de grãos em armazéns**, utilizando **visão computacional (OCR)** e **integração com sensores de peso** para garantir precisão, rastreabilidade e segurança nas operações logísticas.

---

## 📌 Objetivo Geral

Desenvolver um sistema para registrar, controlar e acompanhar o escoamento de grãos em um armazém, com foco nas operações de **entrada e saída**, garantindo precisão nos registros por meio de sensores e câmeras.

---

## 🎯 Objetivos Específicos

- Registrar entradas e saídas de grãos com base em sensores e câmeras.
- Capturar automaticamente a placa dos caminhões via visão computacional.
- Integrar com balança rodoviária para registrar peso bruto, líquido e tara.
- Controlar os níveis de estoque em tempo real por tipo de grão.
- Armazenar histórico de movimentações para futuras análises.
- Evitar erros ou fraudes no processo logístico.

---

## 🔍 Escopo Inicial

O sistema será baseado em Python com interface via **terminal**, e conterá os seguintes módulos:

- 📷 Visão computacional para leitura da placa do caminhão (`OpenCV` + `Tesseract OCR`)
- ⚖️ Integração com balança rodoviária (porta serial ou leitura de arquivo)
- 💾 Armazenamento em memória com exportação futura para CSV/TXT

---

## 📦 Entidades e Atributos

### 🚚 Caminhão

### 🧺 Grão
- Tipo (ex: soja, milho, arroz)
- Unidade de medida

### 🔁 Movimentação
- Tipo: entrada ou saída
- Quantidade
- Data
- Placa do caminhão
- Peso bruto, tara, peso líquido
- Origem/destino
- Observações

### 📊 Estoque
- Quantidade disponível por tipo de grão
- Atualização automática após movimentações

---

## ✅ Funcionalidades Principais

- Captura da **placa do caminhão via OCR**
- Leitura automática do **peso bruto, líquido e tara**
- Registro de entrada e saída com preenchimento automático de dados
- Atualização de **estoque em tempo real**
- Histórico completo de todas as movimentações
- Validação de estoque para evitar saídas indevidas

---

## 🧠 Tecnologias Utilizadas

- **Python 3.x**
- **OpenCV** e **Tesseract OCR** (Visão Computacional)
- **Pandas** (manipulação de dados)
- **PySerial** ou leitura de arquivos para integração com balança
- Armazenamento em memória (com exportação futura para CSV)

---

## 🧑‍🌾 Público-Alvo

Pequenas e médias **cooperativas**, **armazéns rurais** e **produtores** com operação logística relevante e que buscam automação e rastreabilidade.

---

## 🧾 Justificativa

A automatização no controle de grãos é essencial para **aumentar a produtividade**, evitar perdas e fraudes. Ao integrar **tecnologia de visão computacional** com **leitura automatizada de peso**, o sistema entrega uma solução acessível, segura e eficiente, mesmo para armazéns com infraestrutura simples.

---

## 🗂️ Estrutura Sugerida

