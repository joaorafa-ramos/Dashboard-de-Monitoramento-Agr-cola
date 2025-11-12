# FIAP - Faculdade de Informática e Administração Paulista

## Atividade 1 - IR ALÉM (Opcional 1) - Dashboard de Monitoramento Agrícola 

## Integrantes

. João Rafael Gonçalves Ramos - 567908

. Letícia Angelim Guerra - 567501

. Matheus Guimarães França - 567144

. Rivando Bezerra Cavalcanti Neto - 568235

. Tales Ferraz de Arruda Domienikan - 567483


## Descrição

Este projeto entrega um **Dashboard de Monitoramento Agrícola** desenvolvido em **Python + Streamlit**. Ele exibe em tempo real as variáveis do solo (**Umidade, pH, Nitrogênio (N), Fósforo (P), Potássio (K)**) e clima, oferecendo recomendações inteligentes de irrigação.  
Tecnologias principais: **Streamlit, Pandas, Altair**.

## Estrutura de Pastas

```
📁 ir-alem-1/
├── .venv/                  ← Ambiente virtual (criado automaticamente)
├── dashboard.py            ← Código principal (Streamlit)
├── dados_sensores.csv      ← Dataset de sensores
├── requirements.txt        ← Dependências do projeto
├── iniciar_dashboard.bat   ← Atalho para execução
├── README.md               ← Este arquivo
└── prints/                 ← Capturas de tela
    ├── print1.png
    ├── print2.png
    └── print3.png
```

## Variáveis Monitoradas

- **Umidade do Solo (%)**
- **pH do Solo**
- **Nitrogênio (N) em kg/ha**
- **Fósforo (P) em kg/ha**
- **Potássio (K) em kg/ha**
- **Temperatura (°C)**
- **Umidade do Ar (%)**
- **Status da Bomba de Irrigação**

## Como Executar no Windows

### Pré-requisitos

- Python 3.8+ e pip instalados
- Arquivo `dados_sensores.csv` na mesma pasta de `dashboard.py`

### Opção 1 – Usar o Atalho

Clique duas vezes em `iniciar_dashboard.bat`.

### Opção 2 – Terminal

```bash
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
streamlit run dashboard.py
```

O dashboard abrirá em `http://localhost:8501`.

## Capturas de Tela

### 1 - Métricas Principais
Métricas Principais (prints/print1.png)
*Exibição das últimas leituras dos sensores: Umidade, pH, Nitrogênio, Fósforo e Potássio.*

### 2 - Gráficos Interativos
Gráficos Interativos (prints/print2.png)
*Análise temporal com gráficos interativos de Umidade/pH e Nutrientes (N, P, K) com zoom e exploração.*

### 3 - Sistema de Recomendação de Irrigação
Sistema de Irrigação (prints/print3.png)
*Recomendações inteligentes baseadas em temperatura, umidade do ar e umidade do solo, com histórico da bomba.*
## Vídeo Demonstrativo

🔗 [LINK DO VÍDEO]((https://youtu.be/J9iB4t9So8U))

## Funcionalidades Implementadas

- Métricas em tempo real 
- Gráficos interativos de Umidade/pH e Nutrientes (N • P • K)
- Recomendação automática de irrigação
- Histórico de acionamento da bomba
- Cache de dados
- Tratamento de erros

## Lógica de Recomendação

O sistema recomenda irrigação baseado em:
- Umidade do Solo < 50%
- Temperatura > 28°C
- Umidade do Ar < 60%







