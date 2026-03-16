# 📑 Torre de Controle Logístico - Dashboard de Performance
 Análise de nível de serviço (OTIF), volumetria e faturamento utilizando Microsoft Excel.

🎯 Objetivo do Projeto

Este projeto foi desenvolvido para centralizar a gestão de transportes, permitindo o acompanhamento em tempo real da eficiência das entregas (On Time e In Full) e o impacto financeiro das operações por região e transportadora."

🛠️ Estrutura dos Dados e Modelagem 

Fato (fNotasFiscais): tabela principal com os registros de operações, onde apliquei lógica condicional (SE) para calcular os indicadores de status das entregas.

Dimensões (dTransportadoras e dClientes): tabelas de cadastro que permitem a segmentação e filtros avançados no dashboard.

<img width="943" height="413" alt="Captura de tela 2026-03-16 164020" src="https://github.com/user-attachments/assets/143b006a-ab1d-435d-843e-0b92c4cb00be" />

⚙️ Processamento e ETL (Transformação de Dados)

Lógica de Negócio: implementação de cálculos de conformidade para determinar o OTIF (On-Time In-Full). Utilizei a fórmula =SE() para cruzar a data de entrega real com a data prometida e verificar a ocorrência de avarias/extravios.

Agregação: criação de tabelas dinâmicas para consolidar os KPIs de Peso Bruto, Faturamento e Volume por trimestre e região.

<img width="434" height="319" alt="Captura de tela 2026-03-16 165634" src="https://github.com/user-attachments/assets/e59e6304-9d9b-4b54-8aa9-c0953431427f" />

📊 Dashboard e Inteligência de Dados

O painel foi estruturado em uma Torre de Controle Logístico, segmentada para oferecer desde uma visão macroexecutiva até o detalhamento operacional:

Visão Executiva (High-Level): monitoramento em tempo real dos indicadores de Faturamento, Peso Bruto e Volume Expedido, permitindo que a gestão visualize a escala da operação de forma imediata.

Gestão de Nível de Serviço (SLA): análise aprofundada de OTIF (On-Time In-Full). O dashboard permite identificar quais transportadoras possuem gargalos de entrega (On-Time) ou problemas de qualidade/avarias (In-Full), direcionando renegociações de contratos e ajustes operacionais.

Análise de Sazonalidade e Tendências: gráficos temporais que demonstram a variação da demanda e da performance de entrega ao longo dos trimestres, facilitando o planejamento de capacidade para períodos de pico.

Inteligência Geográfica: mapa interativo que destaca a capilaridade das vendas por estado, permitindo identificar regiões com alta volumetria mas baixo nível de serviço, auxiliando na redistribuição estratégica de cargas.


<img width="596" height="331" alt="Dashboard controle de transporte" src="https://github.com/user-attachments/assets/607d6cf8-e85f-430a-b7aa-a3c632caf60e" />


### 🛠️ Tecnologias e Competências
* **Microsoft Excel:** Procv/Índice e Corresp, Lógica Condicional, Tabelas Dinâmicas e Power Pivot.
* **Logística & Supply Chain:** Gestão de indicadores de performance (OTIF), análise de fretes e volumetria.
* **Data Visualization:** Design de Dashboards, Storytelling e análise geográfica.
