<h1 align="center">🚗 Vehicle Rental Management</h1>

<p align="center">
  <strong>Dashboard de gestão em Power BI</strong> — controle de locação de veículos, faturamento e previsão preditiva de vendas
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Power_BI-F2C811?style=flat&logo=powerbi&logoColor=black">
  <img src="https://img.shields.io/badge/DAX-107C10?style=flat">
  <img src="https://img.shields.io/badge/Power_Query-217346?style=flat">
</p>

---
## 🎯 Objetivo
Centralizar indicadores operacionais e financeiros de uma locadora — faturamento, ticket médio, quilometragem e qualidade cadastral da base de clientes — além de projetar tendências futuras de faturamento.

## 📊 Fonte de dados
Dados fictícios da plataforma Kaggle criados para prática, simulando uma locadora de veículos (Yto Car) com operação em múltiplas cidades entre 2014 e 2019.

## 🛠️ Ferramentas utilizadas
Power BI Desktop · DAX · Power Query (M) · Modelagem relacional (Inner Join, Left Join, Left Anti Join)

## 🖼️ Preview
### Capa
<p align="center">
  <img src="imagens/CarRentalAgency1.png" width="700"><br>
<em>Tela de abertura dashboard, apresentando  o projeto "Controle de Locação de Veículos" e os três eixos principais de análise: controle de clientes, controle de modelo / faturamento e monitoramento de quilometragem / previsão de vendas.</em>
</p>

### Locação de Veiculos
<p align="center">
  <img src="imagens/mainpanel.png" width="700"><br>
<em>Visão geral operacional: total de clientes, quilometragem média e faturamento consolidado, com filtros por situação, ano, modelo e dia. Traz também a distribuição de faturamento por ano e por dia da semana, além de uma tabela de consumos com busca dinâmica por placa do veículo.</em>
</p>

### Clientes
<p align="center">
  <img src="imagens/Clients.png" width="700"><br>
<em>Painel focado na qualidade da base de clientes da Yto Car: proporção de veículos por categoria (Luxo, Light, não registrada), situação cadastral (cadastrado vs. não cadastrado) e o faturamento associado a cada grupo. Duas tabelas lado a lado permitem cruzar rapidamente clientes com e sem cadastro completo.</em>
</p>

### Previsão
<p align="center">
  <img src="imagens/Forecast.png" width="700"><br>
<em>Módulo preditivo: evolução histórica do faturamento (2014–2019) para clientes ativos, com projeção de tendência e banda de incerteza para 2020, além de indicadores de ticket médio e quantidade de clientes no período filtrado.</em>
</p>

### Modelo de Dados e Medidas
<table>
<tr>
<td width="50%">
<p align="center">
  <strong>Modelo de dados</strong><br>
  <img src="imagens/ModelDisplay.png" width="450"><br>
  <em>Modelagem relacional com Inner Join, Left Join e Left Anti Join entre as tabelas de clientes (tb_cli) e quilometragem (tb_km), isolando clientes cadastrados, não cadastrados e cruzamentos completos.</em>
</p>
</td>
<td width="50%">
<p align="center">
  <strong>Tabela de medidas</strong><br>
  <img src="imagens/Measures.png" width="110"><br>
  <em>Medidas DAX centralizadas — Faturamento, Média KM, Ticket Médio, Total de Clientes e Total de Cidades — organizadas numa tabela dedicada, reutilizável em todo o relatório.</em>
</p>
</td>
</tr>
</table>

## 🔗 Dashboard Interativo
[▶️ Clique aqui para explorar o dashboard ao vivo](https://app.powerbi.com/view?r=eyJrIjoiYzNjNTA1ZDctODRkNy00YzM3LThkOGItYWM1ODgyYTkzYWZjIiwidCI6IjY1NWFhNjFkLTVkY2ItNDE4Mi05N2YxLTJmNTQ5MTlkZTBjZiJ9)

## 🧩 Destaques técnicos
- **Modelagem relacional avançada**: uso combinado de Inner Join, Left Join e Left Anti Join entre as tabelas de clientes (`tb_cli`) e quilometragem (`tb_km`), isolando clientes cadastrados, não cadastrados e cruzamentos completos.
- **Tratamento de dados no Power Query**: padronização de inconsistências textuais (`Table.ReplaceValue`), como registros de marca/modelo não identificados, tratados como "MODELO NÃO REGISTRADO".
- **Tabela de medidas centralizada (DAX)**: KPIs reutilizáveis como Faturamento, Média KM, Ticket Médio, Total de Clientes e Total de Cidades, organizados numa tabela dedicada de medidas.
- **Busca dinâmica por placa**: campo de consulta interativo para localizar veículos específicos direto no dashboard.
- **Página preditiva**: projeção de tendência (forecast) sobre a série histórica de faturamento, com banda de incerteza visual.

## 💡 Principais insights
- Base de 30 clientes, com faturamento total de R$ 81,43 mil no período analisado
- 2015 foi o ano de pico, concentrando 42,82% de todo o faturamento (R$ 35 mil)
- Queda acentuada em 2017 (apenas 4,07% do faturamento), com recuperação parcial em 2019 (24,58%)
- Terça-feira é o dia de maior faturamento (R$ 34 mil), com queda progressiva ao longo da semana até quarta-feira (R$ 1 mil)
- 73,99% do faturamento (R$ 57,38 mil) vem de clientes com cadastro completo, indicando espaço para regularizar a base pendente (26,01%)
- Módulo preditivo aponta tendência de queda no faturamento entre 2019 e 2020 para o segmento de clientes ativos

## 📁 Estrutura
- Dashboard - LOCADORA DE VEICULO.pbix
- imagens/imagens
- Dashboard interativo
- Destaques técnicos
- README.md

## 📬 Contato
[GitHub](https://github.com/RPessotti) · [LinkedIn](https://linkedin.com/in/rafael-pessotti-563240323)
