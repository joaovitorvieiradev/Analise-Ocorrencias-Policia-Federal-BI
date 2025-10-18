# 📊 Análise de Ocorrências com Armas de Fogo no Brasil (Polícia Federal)

<p align="center">
  <img src="assets/images/print geral.png" alt="Visão Geral do Dashboard" width="850"/>
</p>

<p align="center">
  <i>Dashboard interativo de Business Intelligence desenvolvido no Microsoft Power BI para análise de dados públicos de ocorrências da P.F.</i>
</p>

---

## 🎯 Sobre o Projeto

Este projeto consiste em um dashboard de BI que analisa um conjunto de dados públicos de ocorrências com armas de fogo registradas pela Polícia Federal no Brasil. O objetivo foi transformar um grande volume de dados brutos (distribuídos em múltiplos arquivos CSV) em um painel interativo e visual, capaz de gerar *insights* rápidos e apoiar a tomada de decisão.

A análise foca em identificar padrões-chave, respondendo a perguntas como:
* Qual o volume total de ocorrências ao longo dos anos?
* Existe sazonalidade? (Quais meses têm mais ocorrências?)
* Quais os principais tipos de ocorrência (Ex: Furto, Apreensão, Apostilamento)?
* Quais as marcas de armas mais recorrentes nesses eventos?
* Qual a distribuição geográfica (por UF) das ocorrências no território nacional?

---

## 🛠️ Ferramentas e Tecnologias

* **Microsoft Power BI:** Ferramenta principal para visualização e criação do dashboard.
* **Power Query (Editor M):** Utilizado para o processo de **ETL (Extract, Transform, Load)**. Foi aqui que os três arquivos CSV (`...ate_2023.csv`, `_2024.csv`, `_2025.csv`) foram conectados, limpos, transformados e combinados em uma única tabela-fato.
* **DAX (Data Analysis Expressions):** Linguagem usada para criar as medidas e colunas calculadas necessárias para a análise (ex: `Total de ocorrências`, `LocalizacaoCompleta` para corrigir o mapa, etc.).

---

## 📈 Análises e Destaques do Painel

O dashboard é composto por múltiplos visuais que interagem entre si, permitindo uma análise *drill-down* (do macro para o micro).

### Visões Adicionais (Filtros Aplicados)

Além da visão geral, o painel permite filtros detalhados. Abaixo, dois exemplos de filtros aplicados:

<table align="center">
  <tr align="center">
    <td><b>Análise de Sazonalidade (Filtro: Mês 10 de 2024)</b></td>
    <td><b>Análise Geográfica (Filtro: Estado de Minas Gerais)</b></td>
  </tr>
  <tr>
    <td><img src="assets/images/print mes 10 2024.png" alt="Dashboard filtrado por Mês 10 2024" width="450"/></td>
    <td><img src="assets/images/print MG.png" alt="Dashboard filtrado por MG" width="450"/></td>
  </tr>
</table>

---

## 💾 Fontes de Dados

Os dados utilizados neste projeto são públicos e foram obtidos de fontes abertas. Eles estão divididos nos seguintes arquivos neste repositório:

```
* OCORRENCIAS_ate_2023.csv
* OCORRENCIAS_2024.csv
* OCORRENCIAS_2025 (1).csv
```

---

## 🚀 Como Explorar o Projeto

Como as licenças gratuitas do Power BI não permitem a publicação de links públicos interativos, você pode explorar o projeto da seguinte forma:

```
1.  Baixe o arquivo .pbix:
    Faça o download do arquivo Analis_ocorrencias_P.F.pbix que está neste repositório.

2.  Abra no Power BI Desktop:
    Você precisa ter o [Microsoft Power BI Desktop](https://powerbi.microsoft.com/pt-br/desktop/) (aplicativo 100% gratuito para Windows) instalado em sua máquina.
    Abra o arquivo .pbix nele.

3.  Interaja!
    Pronto! Agora você tem acesso ao dashboard completo e 100% interativo, podendo aplicar filtros, analisar os dados e ver todo o trabalho de modelagem.
```

---

*Projeto de portfólio desenvolvido por João Vitor.*