# Dashbord de Vendas Xbox by DIO

## 🧩 BASE ESTRUTURAL

## 🎮 — 1. Sobre o Projeto

Este projeto foi desenvolvido como um dashboard interativo voltado para a análise de vendas do Xbox Game Pass, permitindo aos usuários transformar dados brutos em informações visuais claras e úteis. A proposta central envolve o uso de gráficos dinâmicos e métricas essenciais para aprimorar a visualização do faturamento total, impacto da auto renovação e vendas de passes adicionais. Além disso, o dashboard conta com um sistema integrado de filtros e segmentação, possibilitando a análise detalhada por período, tipo de assinatura e comportamento do consumidor. Com a inclusão de indicadores de desempenho, os usuários podem acompanhar tendências de vendas em tempo real, facilitando a tomada de decisões estratégicas e proporcionando maior clareza na gestão dos resultados do Xbox Game Pass.

## 🎭 — 2. Qual a estrutura da planilha?


### 2.1. Amostra de dados (Perfil Conservador):

| Cenários           | Patrimônio Acumulado | Rendimento  |
|--------------------|----------------------|-------------|
| Quanto em 1 ano?   | R$ 12.633,23         | R$ 117,49   |
| Quanto em 2 anos?  | R$ 26.750,73         | R$ 247,78   |
| Quanto em 5 anos?  | R$ 79.857,52         | R$ 742,67   |
| Quanto em 15 anos? | R$ 461.543,83        | R$ 4.292,36 |
| Quanto em 20 anos? | R$ 884.178,41        | R$ 8.222,86 |

### 2.2. Perfil de Investimento Mensal

O Investimento Mensal acima mostrado se refere a um valor fixo de R$ 1.000,00, ao qual anexei ao perfil **"Conservador"**. No entanto, existe na planilha valores que são alusivos a outros dois perfis que igualmente são analisados, sendo, o perfil **"Moderado"** com valor fixo de R$ 2.000,00 e, o perfil **"Agressivo"** com valor fixo de R$ 2.500,00.
Ambos os perfis refletem de forma interativa na tabela, refletindo os ganhos finais mensais e o acumulado, assim como no patrimônio e rendimentos anuais de cada valor que é investido.

---

## 🎱 CONTEXTO FOCAL

## ♟️ — 3. Perfis de Investidor (nas células mescladas `D32` & `D33`):

- **Investidor Conservador** – faixa de valores entre R$ 1.000,00 e R$ 1.999,99, priorizando segurança e estabilidade;
- **Investidor Moderado** – valores variando de R$ 2.000,00 a R$ 2.499,99, equilibrando risco e retorno de forma estratégica;
- **Investidor Agressivo** – montantes a partir de R$ 2.500,00, focando em alto potencial de valorização e maior exposição ao risco.

### 3.1. Construção do Modelo:

As células `D32` e `D33` analisam a quantidade do valor investido com base no perfil do investidor, usando a fórmula:

```excel
==SE(D32="Conservador"; 1000;
 SE(D32="Moderado"; 2000;
 SE(D32="Agressivo"; 2500; 0)))
```

Esse retorno beneficia a transparência dos Tipos de FII, que são o ponto focal da análise, trazendo o percentual de maneira demonstrativa, representando a quantidade investida. 
No mais, o investimento mensal, anteriormente proposto, demonstra as informações de dividendos e patrimônio com base na taxa percentual do período, ao qual vinculei a 0,93% pelo período de 120 meses (10 anos).

---

## 🎲 CONCLUSÃO

## 🕹️ — 4. Proposta da Planilha



## ✖️ — 5. Construção

- Microsoft Excel;
- Sistema Interativo e Dinâmico de Menus;
- Sistema de Assinaturas clara e transparente com segmentação dos Dados;
- Validação de Dados por marcadores de valores em gráficos;
  
## 🎰e — 6. Anexo do Arquivo
[Clique aqui para baixar](https://github.com/EdBerriel/Dashbord-Vendas-Xbox/blob/main/Dashboard%20Xbox.xlsx)
