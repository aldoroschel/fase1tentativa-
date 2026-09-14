# Relatório Operacional de Pré-Decolagem

## Descrição do Projeto
Este trabalho apresenta uma análise detalhada dos procedimentos e verificações críticas para a fase de pré-decolagem de uma missão espacial. O projeto abrange a telemetria dos sistemas vitais, um algoritmo de verificação Go/No-Go, uma análise energética, uma análise assistida por IA para identificação de anomalias e mitigação, e uma reflexão crítica sobre aspectos éticos, sociais e sustentáveis da exploração espacial.

## Autores
- Kelven Carlos Luiz de Souza (Rm_575105)
- Aldo Roschel (Rm_575601)
- Larissa Bressanini Lehn (Rm_575921)
- Nicole Luiza Mascarenhas Zerbato (Rm_575981)

## Pré-requisitos
- Python 3.x
- Ambiente Google Colaboratory (para execução do notebook)

## Como Usar
1. Faça o download do arquivo `.ipynb` do notebook,
 https://github.com/aldoroschel/fase1tentativa-.git
2. Abra o arquivo no Google Colaboratory.
3. Execute as células do notebook sequencialmente. O script Python na seção `1.3 Script em Python` solicitará entradas interativas para simular os dados de telemetria.


Digite a temperatura interna em °C: 20

Digite a temperatura externa em °C: 20

Digite a pressão do tanque em psi: 3100

Digite o nível de energia em %: 85

Digite se a estrutura está íntegra (1) ou não(0): 1

Digite se o módulo de propulsão está ativo (1) ou não(0): 1

Digite se o módulo de vida está ativo (1) ou não(0): 1

Digite se o módulo de comunicação está ativo (1) ou não(0): 1

Digite se o módulo de navegação está ativo (1) ou não(0): 1

==================================================

               LEITURA DA VARIÁVEIS               

==================================================

Temperatura interna OK

Temperatura externa OK

Pressão dos tanques OK

Nível de Energia OK

Estrutura OK

Módulo de propulsão OK

Módulo de vida OK

Módulo de comunicação OK

Módulo de navegação OK


==================================================

               DECOLAGEM PERMITIDA                

==================================================

## Principais Seções e Análises

### 1.1 Organização e Descrição da Telemetria
Detalha os parâmetros vitais coletados por sensores da espaçonave, incluindo temperatura interna e externa, integridade estrutural, níveis de energia, pressão dos tanques e status dos módulos críticos. As faixas de segurança são referenciadas por normas da NASA, ECSS e ANSI/AIAA.

### 1.2 Algoritmo de Verificação (Pseudocódigo)
Apresenta a lógica do algoritmo de decisão Go/No-Go para a decolagem, baseado nos parâmetros de telemetria.

### 1.3 Script em Python
Um script interativo em Python que simula a leitura dos dados de telemetria, executa as validações condicionais e exibe o resultado do checklist de pré-lançamento (Decolagem Permitida ou Não Permitida).

### 2. Análise Energética
Calcula a energia disponível para a fase pós-decolagem, considerando a capacidade total da bateria, carga atual, consumo estimado na decolagem e perdas energéticas. A conclusão indica que o veículo mantém 66.08% de sua capacidade energética total disponível, atendendo às margens operacionais de segurança. **Nota:** Os valores de Capacidade Total da Bateria, Carga Atual, Consumo Estimado na Decolagem e Perda Energética são hipotéticos/ilustrativos para demonstrar os cálculos.

### 3. Análise Assistida por IA
Classifica os dados de telemetria em nominais e críticos, identifica possíveis anomalias (Risco Alfa: flutuação de pressão; Risco Beta: desbalanceamento no consumo de bateria) e sugere estratégias de risco e mitigação (Monitoramento Ativo de Tendência e Redundância Energética).

### 4. Reflexão Crítica
Aborda aspectos como Ética e Responsabilidade na automação de sistemas críticos, o Impacto Social da Exploração Espacial e a Sustentabilidade Tecnológica, discutindo a necessidade de gerenciamento de lixo espacial e design de veículos reutilizáveis.

## 5. Referências Bibliográficas
- NATIONAL AERONAUTICS AND SPACE ADMINISTRATION (NASA). NASA-STD-7001B: Payload Environmental Verification Requirements. Washington, D.C.: NASA, 2019.
- NATIONAL AERONAUTICS AND SPACE ADMINISTRATION (NASA). GSFC-STD-7000B: General Environmental Verification Standard (GEVS) for GSFC Flight Programs and Projects. Greenbelt: Goddard Space Flight Center, 2021.
- EUROPEAN COOPERATION FOR SPACE STANDARDIZATION (ECSS). ECSS-E-ST-31C: Space engineering - Thermal control. Noordwijk: ECSS Secretariat, ESA-ESTEC, 2008.
- NASA-STD-4003: Electrical Power System Design Requirements for Spacecraft.
- AIAA S-122: Electrical Power Systems for Unmanned Spacecraft.
- ISO 17770: Space systems — Spacecraft electrical power system design.
