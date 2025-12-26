# Simulador-de-Investimentos-Excel-DIO

Planilha de Investimentos – Excel 

Este projeto consiste em uma planilha de investimentos desenvolvida em Excel, com o objetivo de auxiliar no planejamento financeiro pessoal, projeção de patrimônio e definição de estratégias de alocação de investimentos de acordo com diferentes perfis de investidor. 

1. Área de Configurações  

Na primeira seção da planilha, o usuário informa: 

-Salário mensal 

-Rendimento da carteira 

Com base nesses dados, a planilha apresenta automaticamente uma sugestão de valor para investimento, considerando 30% do salário informado. 

2. Investimento Mensal 

Nesta etapa, o usuário pode definir: 

-Valor a ser investido mensalmente 

-Período de investimento (em anos) 

-Taxa de rendimento mensal 

A partir dessas informações, a planilha calcula: 

-Patrimônio acumulado ao final do período 

-Valor estimado de dividendos mensais 

3. Análise de Cenários 

A planilha apresenta uma análise comparativa de longo prazo, projetando: 

Patrimônio acumulado 

Dividendos mensais 

Para os seguintes horizontes de tempo: 

-2 anos 

-5 anos 

-10 anos 

-20 anos 

-30 anos 

Essa seção permite ao usuário visualizar o impacto do tempo e da disciplina de investimentos nos resultados financeiros. 

4. Sugestão de Alocação de Investimentos 

Nesta seção, o usuário pode selecionar o perfil de investidor, sendo: 

-Conservador 

-Moderado 

-Agressivo 

Com base no perfil escolhido e no valor total a ser investido, a planilha apresenta: 

-Tipos de Fundos Imobiliários (FIIs) 

-Percentuais sugeridos de alocação 

-Valores correspondentes para cada tipo de FII, ajustados conforme o perfil selecionado 

5. Gráfico Dinâmico 

A planilha conta ainda com um gráfico interativo, que: 

Atualiza automaticamente os percentuais de alocação 

Reflete visualmente as mudanças de acordo com o perfil de investidor selecionado 

 

Essa planilha foi desenvolvida para oferecer uma visão clara, prática e estratégica sobre investimentos, facilitando a tomada de decisões financeiras de curto, médio e longo prazo. 

 

Detalhamento Técnico das Funcionalidades 

1. Configurações  

Na seção de configurações, a sugestão de valor para investimento é calculada de forma automática a partir do salário informado pelo usuário. 
Para isso, a planilha utiliza uma fórmula simples que multiplica o valor do salário por 0,3, indicando como recomendação o investimento de 30% da renda mensal. 

2. Investimento Mensal 

Na área destinada ao investimento mensal, são realizados os seguintes cálculos: 

Patrimônio Acumulado 
O valor acumulado ao final do período é calculado por meio da fórmula de Valor Futuro (VF) do Excel. 
Essa fórmula considera: 

Taxa de rendimento mensal 

Número de períodos (convertido para meses, multiplicando o número de anos por 12) 

Valor investido mensalmente (pgto.) 

Dividendos Mensais 
O valor estimado dos dividendos mensais é obtido multiplicando o patrimônio acumulado pelo rendimento da carteira informado pelo usuário nas configurações iniciais. 

3. Análise de Cenários 

Na seção de cenários, é utilizada a mesma fórmula de Valor Futuro (VF) aplicada no investimento mensal. 
A única variável alterada é o prazo de investimento, permitindo a projeção do patrimônio acumulado e dos dividendos mensais para diferentes horizontes de tempo (2, 5, 10, 20 e 30 anos). 

4. Perfil de Investidor 

Para a seleção do perfil de investidor (Conservador, Moderado ou Agressivo), foi utilizada a funcionalidade de Validação de Dados do Excel. 
Isso garante que o usuário possa escolher apenas entre as opções previamente definidas, evitando erros de preenchimento e assegurando a integridade dos cálculos subsequentes. 

5. Percentual de Alocação por Tipo de FII 

O cálculo dos percentuais de alocação para cada tipo de Fundo Imobiliário (FII) foi estruturado a partir de uma tabela auxiliar, que contém: 

Uma chave única para cada combinação de perfil de investidor e tipo de FII 

O percentual correspondente de alocação para cada perfil 

A partir dessa tabela, foi utilizada a função PROCV, que localiza a chave correspondente (por exemplo, Perfil Moderado + FII de Papel) e retorna automaticamente o percentual de alocação adequado ao perfil selecionado pelo usuário. 

 

Esse conjunto de fórmulas e validações permite que a planilha seja dinâmica, confiável e facilmente ajustável, oferecendo uma experiência mais robusta para o planejamento e a simulação de estratégias de investimento. 

 

 

 

 

 

 

Na parte das configurações, a sugestão de investimentos pega a célula do salário e multiplica por 0,3, assim indicando uma sugestão de que se deve investir 30% do salário. 

Na parte do investimento mensal, na parte de valor acumulado, usamos a fórmula de Valor Final (VF), que utiliza a taxa mensal, número de períodos (a fórmula considera o número de períodos em mês, então, multiplicamos o número de períodos por 12) e o quanto queremos investir por mês (pgto.). Já na parte dos dividendos mensais, multiplicamos o patrimônio acumulado pelo rendimento da carteira informado pelo usuário. 

Na parte dos cenários utilizamos a mesma fórmula de valor final apenas alterando os anos. 

Na parte de perfil, utilizamos a Validação de Dados para que o usuário possa escolher o tipo de perfil de investimento. 

Já no percentual de cada tipo de FII, tive que usar uma outra tabela com uma chave única para cada perfil e cada tipo de FII, depois utilizei o PROCV para procurar o tipo de chave (perfil moderado e FII de papel por exemplo) e mostrar a porcentagem de acordo com cada perfil. 

 
---


### 🔗 Link / Versão Web

**[📂 ACESSAR VERSÃO WEB](https://federalitajuba-my.sharepoint.com/:x:/g/personal/d2024004742_unifei_edu_br/IQAcxUFfGsHHRbHbB564M5S5AczH5PJNZd5Q6hYwGfDBVq0?e=ZU8A6Y)**
 

 
