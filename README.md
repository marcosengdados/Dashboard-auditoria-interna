# 📊 Dashboard SGA · ISO 14001:2015 — InnovElectro

> Sistema de Gestão Ambiental — Análise de Conformidade e Ações Corretivas  
> Desenvolvido em **Power BI** com base em dados reais de auditorias internas.

---

## 🗂️ Sobre o Projeto

Dashboard interativo para monitoramento do SGA de uma indústria do setor eletroeletrônico, cobrindo **conformidade geral, consumo energético, não conformidades, ações corretivas e investimento CAPEX** — tudo alinhado à estrutura da ISO 14001:2015 (cláusulas 6.1, 6.2, 9.1, 9.2 e 10.2).

---

## 📌 Roteiro de Visualizações

### 1 · KPIs Estratégicos (Painel Lateral)

Quatro cartões de indicadores consolidados no topo da visão principal:

- **Média de Energia** — 0,92 kWh/Un (meta: 0,85) → status **Atenção**
- **Conformidade Geral** — 87,39% (meta: 85%) → **Atingida** ✅
- **Investimento Total** — R$ 1,5 Mi com 16 ações de prioridade
- **Emissão de CO₂** — 0,334 kg/Un (meta: 0,40) → **Atingida** ✅

> Leitura rápida do estado geral do SGA sem necessidade de drill-down.

---

### 2 · Consumo de Energia — Gráfico de Barras Mensal

Acompanhamento mês a mês do consumo real versus meta (linha tracejada em 0,85 kWh/Un).

- **Vermelho** → Abaixo da meta (Jan–Mar): pico de 0,97 no início do ciclo
- **Laranja** → Próximo da meta (Abr–Jun): fase de ajuste operacional
- **Verde** → Acima da meta (Jul–Dez): eficiência consolidada no segundo semestre

> Tendência de melhora contínua ao longo do ano evidencia o resultado das ações corretivas de Eficiência Energética.

---

### 3 · Ações por Área · Investimento (Gráfico de Barras Horizontais — Página 1)

Comparativo entre volume de ações corretivas e investimento alocado por área auditada.

- **Eficiência Energética** concentra o maior CAPEX (~R$ 1,5 Mi) — dominância esperada dado o perfil industrial
- Demais áreas (Produto, Cadeia de Fornecedores, Emissões, Resíduos) com investimentos menores e distribuídos
- Permite identificar onde o orçamento está concentrado frente à criticidade de cada área

---

### 4 · Status das Ações Corretivas — Gráfico de Rosca

Distribuição das 16 ações corretivas abertas por status de andamento:

| Status | Qtd | % |
|---|---|---|
| Concluída | 6 | 37,5% |
| Em andamento | 6 | 37,5% |
| Planejada | 3 | 18,75% |
| Concluída com atraso | 1 | 6,25% |

> Mais de 75% das ações já estão concluídas ou em execução ativa — demonstra maturidade de gestão no ciclo PDCA.

---

### 5 · Tabela de Ações Corretivas · ISO 14001:2015 (Página 1)

Listagem detalhada com: Área Auditada, Ação Corretiva, Responsável e Status.

Destaques:
- Ações de **Eficiência Energética** com maior expressão financeira (VRF Inverter R$180k, submedidores R$48k)
- Ações de **Documentação e Treinamento** com rápida execução e status **Fechada**
- Rastreabilidade completa de responsáveis (TI + Manutenção, Eng. Infraestrutura, Coord. SGA, RH + SSMA)

---

### 6 · KPIs de Auditoria (Painel Lateral — Página 2)

Indicadores complementares focados no ciclo de auditoria:

- **Não Conformidades Ativas** — 10 registros, classificação **Crítica**
- **Custo Total de Auditorias** — R$ 123,50 Mil
- **CAPEX Realizado** — R$ 602,35 Mil
- **Índice Médio de Auditoria** — 83,33% (classificação **Crítica**)

---

### 7 · Não Conformidades por Área · Gravidade (Gráfico de Barras Agrupadas)

Volume de NCs por área auditada, segmentado por gravidade (cláusula 10.2):

- **Eficiência Energética** — maior concentração de NCs (≥3), com gravidades Leve e Moderada
- **Cadeia de Suprimentos** e **Documentação** — NCs Graves registradas
- Demais áreas (Efluentes, Emissões, Resíduos, Produção, Treinamento) com NCs Moderadas distribuídas

> Leitura por gravidade orienta a priorização das próximas auditorias internas.

---

### 8 · CAPEX Aprovado vs. Realizado por Área (Gráfico de Barras Horizontais — Página 2)

Comparativo entre orçamento aprovado e efetivamente executado:

- **Eficiência Energética** — maior gap entre aprovado e realizado, indicando ações ainda em andamento
- **Gestão de Resíduos** e **Produto** — execução mais próxima do aprovado
- Áreas menores (GHG/Carbono, Cadeia, Treinamento, Emissões) com CAPEX compacto e bem executado

---

### 9 · Tabela Expandida de Ações Corretivas (Página 2)

Detalhamento com colunas adicionais: **Custo R$, Prazo em Dias, Gravidade e Cláusulas ISO**.

- Ações de Eficiência Energética (submedidores): R$ 48.000 · 120 dias · Leve → cláusulas 6.1.2 / 8.4 / 9.1
- VRF Inverter: R$ 180.000 · 180 dias · Moderada → em tratamento
- Checklist de fim de turno: R$ 1.800 · 15 dias · Leve → Fechada
- POP-REEE-BAT-001 (Resíduos): R$ 4.500 · 30 dias · Moderada → Fechada

> Visão que conecta custo, prazo e conformidade normativa em uma única tabela — útil para relatórios de revisão pela direção (cláusula 9.3).

---

## 🛠️ Stack Técnica

| Ferramenta | Uso |
|---|---|
| Power BI Desktop | Modelagem, visualizações e publicação |
| Excel / `.xlsx` | Fonte de dados (SGA_InnovElectro_DadosProj) |
| DAX | Medidas calculadas (conformidade, médias, CAPEX) |
| ISO 14001:2015 | Framework normativo das análises |

---

## 📁 Estrutura do Repositório

```
📂 sga-iso14001-powerbi/
├── 📄 README.md
├── 📊 Dashboard_ISO14001.pbix
├── 📂 data/
│   └── SGA_InnovElectro_DadosProj.xlsx
└── 📂 assets/
    ├── dashboard_pagina1.png
    └── dashboard_pagina2.png
```

---

## 👤 Autor

**Marcos Vinicius S. Lima**  
Engenheiro Ambiental · Análise de Dados · Geoprocessamento  
[linkedin.com/in/marcosdados](https://linkedin.com/in/marcosdados) · [github.com/marcosengdados](https://github.com/marcosengdados)
