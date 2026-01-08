---
title: "Econometrics: Globalization, Education, and Obesity"
date: 2024-06-30
math: true
summary: "Applied panel regression models to study the relationship between social globalization, education, and obesity using cross-country panel data, with fixed-effects specifications and economic interpretation."
---

## Social Globalization, Education, and Obesity  
**Evidence from a Cross-Country Panel Study**

Global obesity has become a major public health concern. According to *The Lancet*, the global adult obesity rate has more than doubled since 1990, and by 2022 more than one billion people worldwide were affected by obesity. In response, the World Health Organization launched the *Acceleration Plan to Stop Obesity* in 2022, encouraging countries to take action before 2030.

This study examines the relationship between social globalization, education, and obesity prevalence using country-level panel data, with a particular focus on how structural and informational factors interact to shape long-run health outcomes.

---

## Research Motivation

Social globalization reflects the intensity of cross-border cultural flows and media openness, which may expose populations to foreign lifestyles, dietary patterns, and consumption norms. A growing literature has documented correlations between social globalization and obesity outcomes at both the individual and aggregate levels.

Education has also been widely studied as a determinant of human physiological and behavioral outcomes, and a substantial body of research has established systematic relationships between educational attainment and obesity. However, social globalization and education are closely connected—particularly through information diffusion and communication technologies.

Rather than examining these factors in isolation, this study analyzes their joint effects on national obesity rates, allowing for interaction effects and heterogeneous transmission channels.

![correlation between education and obesity](edu_obe_corr.png)
![correlation between social globalization and obesity](glob_obe_corr.png)
---

## Data and Empirical Strategy

The analysis is based on an unbalanced panel dataset covering **172 countries from 1990 to 2021**. Obesity is measured as the share of the adult population with a body mass index (BMI) greater than or equal to 30, following the World Health Organization definition.

Social globalization is captured using the **KOF Social Globalization Index**, which aggregates three dimensions: personal contacts, information flows, and cultural proximity. Education is measured by average years of schooling at the national level.

To account for economic development and nutritional conditions, the empirical models include GDP per capita, its squared term, and daily per-capita caloric supply as control variables. All estimations are conducted using fixed-effects panel regressions, with the choice of fixed effects supported by Hausman tests.

---

## Empirical Models

### Basic Model

The baseline specification relates obesity prevalence to aggregate social globalization and education:

$$\begin{aligned}
obe_{i,t} &= \beta_0 + {\color{blue}{\beta_1 \cdot kofsog_{i,t} + \beta_2 \cdot edu_{i,t}}} + \beta_3 \cdot \alpha_i \\\\
&+ \left( \beta_4 \cdot perkgdp_{i,t} + \beta_5 \cdot perkgdp^2_{i,t} + \beta_6 \cdot kcal_{i,t}\right) + u_{i,t}
\end{aligned}$$


where $obe_{i,t}$ denotes the obesity prevalence rate in country $i$ at time $t$, and $\alpha_i$ captures country fixed effects.

---

### KOF Subcomponent Model

To identify which dimensions of social globalization drive the observed relationship, the aggregate KOF index is decomposed into its subcomponents:

$$\begin{aligned}
obe_{i,t} &= \beta_0 + {\color{blue}{\beta_1 \cdot kofipg_{i,t} + \beta_2 \cdot kofing_{i,t} + \beta_3 \cdot kofcug_{i,t}}} + \beta_4 \cdot edu_{i,t} + \beta_5 \cdot \alpha_i \\\\
&+ \left( \beta_4 \cdot perkgdp_{i,t} + \beta_5 \cdot perkgdp^2_{i,t} + \beta_6 \cdot kcal_{i,t}\right) + u_{i,t}
\end{aligned}$$


The three components correspond to interpersonal contacts, information flows, and cultural proximity, respectively.

---

### Interaction Model

To test whether the effect of social globalization on obesity varies with educational attainment, an interaction specification is estimated:

$$\begin{aligned}
obe_{i,t} &= \beta_0 + \beta_1 \cdot kofsog_{i,t} + \beta_2 \cdot edu_{i,t} +  {\color{blue}{\beta_3 \cdot kof \times edu_{i,t}}} + \beta_4 \cdot \alpha_i \\\\
&+ \left( \beta_5 \cdot perkgdp_{i,t} + \beta_6 \cdot perkgdp^2_{i,t} + \beta_7 \cdot kcal_{i,t}\right) + u_{i,t}
\end{aligned}$$

This specification allows the marginal effect of social globalization to vary systematically with the level of education.

---
![basic model](basic.png)
![KOF subcomponent model](KOF_sep.png)
![interaction model](cross.png)




## Conclusion

Using country-level panel data, this study documents three main findings:

1. Social globalization is positively associated with national obesity rates.
2. Education is also positively associated with obesity at the country level, except in high-income countries.
3. Information flows constitute the primary channel through which social globalization relates to obesity.

These results highlight systematic differences between country-level and individual-level analyses and provide evidence on how structural and informational factors shape global obesity patterns.
