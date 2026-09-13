# Sistema de Auditoria de Erros em FP&A (Finanças) com Python & Pandas

Este projeto apresenta a automatização de um sistema de auditoria e saneamento de dados financeiros para o departamento de FP&A (Planejamento e Análise Financeira). O objetivo principal é identificar inconsistências de lançamentos em Centros de Custo e realizar a conciliação automatizada de despesas operacionais (OPEX).

A combinação de habilidades de negócios em Finanças corporativas com a biblioteca Pandas permite eliminar processos manuais em planilhas, mitigar riscos de lançamentos incorretos e acelerar o fechamento mensal.

## 🛠️ Tecnologias e Conceitos Utilizados
- **Python 3** (Lógica estruturada e automação)
- **Pandas** (Tratamento de dados, Filtros Booleanos, Agrupamentos e *Partial Match*)
- **Dicionário de Negócios / FP&A:** Centro de Custo, Rateio, Auditoria de Notas e Despesas Operacionais.

## 🚀 Funcionalidades do Sistema
1. **Saneamento Massivo de Dados (Data Cleansing):** Tratamento automatizado de inconsistências de digitação (letras maiúsculas/minúsculas e espaços extras nas extremidades) usando laços de repetição eficientes (`for`).
2. **Prevenção de Erros de Tipo:** Tratamento preventivo de dados nulos ou numéricos misturados em colunas de texto com `astype(str)`.
3. **Visão Consolidada (Tabela Dinâmica):** Agrupamento (`groupby`) e sumarização de despesas por Centro de Custo em segundos.
4. **Auditoria por Correspondência Parcial (*Partial Match*):** Filtro inteligente que varre as descrições contábeis para isolar despesas específicas (ex: "Licenças"), simulando o comportamento avançado de filtros de texto corporativos.
5. **Integração com Excel:** Exportação automatizada dos relatórios de auditoria para o formato `.xlsx`.

## 📦 Como Executar o Projeto

1. Clone o repositório:
```bash
git clone https://github.com
```

2. Certifique-se de ter o Pandas instalado:
```bash
pip install pandas openpyxl
```

3. Certifique-se de que o arquivo de dados `dados_fpa_auditoria.csv` está no mesmo diretório do script.

4. Execute o script pelo terminal:
```bash
python auditoria_fpa.py
```

## 📊 Estrutura do Script de Automação

O script processa a base de dados original, limpa os campos de texto para evitar quebras em rateios e exporta um arquivo formatado para a tomada de decisão da liderança financeira.

---
*Projeto desenvolvido como parte do portfólio de transição e fortalecimento técnico na intersecção entre Finanças Corporativas e Data Analytics.*


