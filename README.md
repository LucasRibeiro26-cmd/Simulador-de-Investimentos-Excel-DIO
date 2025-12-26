# 📊 Simulador de Investimentos & Alocação de Ativos


## 📖 Sobre o Projeto

Este projeto consiste em uma ferramenta desenvolvida em **Microsoft Excel** com o objetivo de auxiliar no planejamento financeiro pessoal. A planilha realiza projeções de patrimônio baseadas em juros compostos e define estratégias automáticas de alocação em Fundos Imobiliários (FIIs) de acordo com o perfil de risco do investidor.

O foco foi criar uma interface intuitiva que transforme inputs simples (salário e aporte) em cenários complexos de longo prazo.

## 🛠️ Funcionalidades Principais

### 1. Planejamento e Configurações
* **Regra dos 30%:** Com base no salário mensal inserido, a planilha calcula automaticamente uma sugestão de aporte ideal (30% da renda).
* **Projeção de Liberdade Financeira:** Calcula o valor estimado de **Dividendos Mensais** futuros baseados no rendimento médio da carteira.

### 2. Análise de Cenários (Longo Prazo)
A ferramenta projeta automaticamente o **Patrimônio Acumulado** e a **Renda Passiva** para diferentes horizontes temporais, permitindo comparar o impacto dos juros compostos em:
* 2 anos (Curto prazo)
* 5 e 10 anos (Médio prazo)
* 20 e 30 anos (Longo prazo)

### 3. Alocação Inteligente de Ativos (FIIs)
O usuário seleciona seu perfil de investidor através de uma lista suspensa:
* 🛡️ **Conservador**
* ⚖️ **Moderado**
* 🚀 **Agressivo**

O sistema então redistribui o valor do aporte sugerido entre diferentes tipos de FIIs (Papel, Tijolo, Híbrido, etc.) com percentuais ajustados especificamente para cada perfil.

## ⚙️ Engenharia e Detalhamento Técnico

Neste projeto, apliquei lógicas avançadas de Excel para garantir a automação e integridade dos dados:

* **Fórmulas Financeiras (`VF` / `FV`):**
  Utilizada para o cálculo de Juros Compostos.
  > *Lógica aplicada:* `VF(taxa_mensal; anos*12; aporte_mensal; valor_atual)`
  
* **Busca e Referência Avançada (`PROCV` com Chave Composta):**
  Para a alocação de ativos, criei uma **Tabela Auxiliar** gerando chaves únicas (Ex: "Moderado + FII Papel"). O `PROCV` utiliza essa chave para buscar o percentual correto de alocação, permitindo dinamismo na mudança de perfis sem uso de macros complexas.

* **Validação de Dados:**
  Implementação de listas suspensas (Drop-down menus) para a seleção de perfis, evitando erros de digitação (input error) e garantindo que os cálculos funcionem corretamente.

* **Visualização de Dados:**
  Gráficos dinâmicos que se atualizam instantaneamente conforme a mudança do perfil de investidor, facilitando a tomada de decisão visual.

## 🚀 Como Acessar a Planilha

Você pode visualizar a planilha funcional ou fazer o download através do link abaixo:

### 📂 **[CLIQUE AQUI PARA ACESSAR O PROJETO](https://federalitajuba-my.sharepoint.com/:x:/g/personal/d2024004742_unifei_edu_br/IQAcxUFfGsHHRbHbB564M5S5AczH5PJNZd5Q6hYwGfDBVq0?e=sBCuoN)**

---

## 👨‍💻 Autor

**Lucas Ribeiro**
Engenharia de Energia - UNIFEI
[Seu LinkedIn](www.linkedin.com/in/lucas-ribeiro-9160082b1)
