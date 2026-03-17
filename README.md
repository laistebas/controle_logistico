# Torre de Controle Logístico - Dashboard de Performance
 Análise de nível de serviço (OTIF), volumetria e faturamento utilizando Microsoft Excel.

### Objetivo do projeto

Este projeto foi desenvolvido para centralizar a gestão de transportes, permitindo o acompanhamento da eficiência das entregas (On Time e In Full) e o impacto financeiro das operações segmentado por região e transportadora.

### Estrutura dos dados e modelagem 

Fato (fNotasFiscais): tabela principal com os registros de operações, onde apliquei lógica condicional (SE) para calcular os indicadores de status das entregas.

Dimensões (dTransportadoras e dClientes): tabelas de cadastro que permitem a segmentação e filtros no dashboard.

<img width="943" height="413" alt="Captura de tela 2026-03-16 164020" src="https://github.com/user-attachments/assets/143b006a-ab1d-435d-843e-0b92c4cb00be" />

⚙️ Processamento e ETL (Transformação de Dados)

Lógica de Negócio: implementação de cálculos de conformidade para determinar o OTIF (On-Time In-Full). Utilizei a fórmula =SE() para cruzar a data de entrega real com a data prometida e verificar a ocorrência de avarias/extravios.

Agregação: criação de tabelas dinâmicas para consolidar os KPIs de Peso Bruto, Faturamento e Volume por trimestre e região.

<img width="434" height="319" alt="Captura de tela 2026-03-16 165634" src="https://github.com/user-attachments/assets/e59e6304-9d9b-4b54-8aa9-c0953431427f" />

📊 Dashboard e Inteligência de Dados

O painel foi estruturado como uma Torre de Controle Logístico, segmentada para oferecer desde a visão macroexecutiva até o detalhamento operacional:

Visão Executiva (High-Level): monitoramento de KPIs críticos (Faturamento, Peso Bruto e Volume Expedido), permitindo que a gestão visualize a escala da operação de forma imediata.

Gestão de Nível de Serviço (SLA): análise aprofundada de OTIF. O dashboard permite identificar quais transportadoras possuem gargalos de prazo (On-Time) ou problemas de qualidade (In-Full), direcionando renegociações de contratos.

Análise de Sazonalidade e Tendências: gráficos temporais que demonstram a variação da demanda e performance ao longo dos trimestres, facilitando o planejamento de capacidade para períodos de pico.

Inteligência Geográfica: mapeamento da capilaridade de expedição por estado, identificando regiões com alta volumetria e baixo nível de serviço para auxílio na redistribuição estratégica de cargas.


<img width="707" height="395" alt="Captura de tela 2026-03-17 104226" src="https://github.com/user-attachments/assets/ce389413-efc1-42fb-a4e1-bd21b58030f5" />


### Principais insights da análise

A partir da exploração dos dados no dashboard, foram identificados pontos críticos para a tomada de decisão estratégica:

Gargalo de Pontualidade (On-Time): identificou-se que a operação possui alta maturidade em separação (In-Full médio de 90%), porém enfrenta desafios logísticos de transporte, com um On-Time médio de 63%. Transportadoras como Gaucho Transportes e RodoCarioca apresentam os menores índices de pontualidade (60%), indicando necessidade de revisão de rotas ou SLAs.

Sazonalidade Crítica (Novembro): a análise histórica de 2018 e 2019 revelou uma queda sistêmica na performance OTIF no mês de novembro (abaixo de 45%). Este insight sugere a necessidade de um planejamento de capacidade antecipado para suportar picos de demanda (como Black Friday).

Liderança de Performance: a transportadora Paulistana destacou-se com o melhor equilíbrio entre os indicadores, mantendo 93% de In-Full e 64% de On-Time, consolidando-se como o parceiro mais confiável para operações de alta prioridade.

Concentração Regional: o Sudeste concentra a maior volumetria da operação (38% do total expedido). O monitoramento constante desta região é vital, pois qualquer oscilação no nível de serviço impacta diretamente o faturamento global da companhia.
