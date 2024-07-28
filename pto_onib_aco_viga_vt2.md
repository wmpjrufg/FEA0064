---
title: Viga VT2
layout: default
grand_parent: Exemplo I
parent: Projeto vigas
nav_order: 2
has_children: false
has_toc: false
---

<!--Don't delete this script-->
<script src = "https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id = "MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
<!--Don't delete this script-->

<p align = "justify">
A seguir são apresentados os dados da viga VT2. 
</p>

<table style = "width:100%">
<thead align="center">
  <tr>
    <th>Variável</th>
    <th>Valor</th>
    <th>Unidade</th>
  </tr>
</thead>
<tbody align="center">
  <tr>
    <td align = "left">Largura da seção transversal (b<sub>w</sub>)</td>
    <td>0,14</td>
    <td>m</td>
  </tr>
  <tr>
    <td align = "left">Altura (h)</td>
    <td>0,45</td>
    <td>m</td>
  </tr>
  <tr>
    <td align = "left">Altura Útil (d)</td>
    <td>0,396</td>
    <td>m</td>
  </tr>
  <tr>
    <td align = "left">Momento característico máximo devido cargas permanentes (M<sub>max,gk</sub>)</td>
    <td>1,9</td>
    <td>kNm</td>
  </tr>
  <tr>
    <td align = "left">Momento característico mínimo devido cargas permanentes (M<sub>min,gk</sub>)</td>
    <td>3,4</td>
    <td>kNm</td>
  </tr>
  <tr>
    <td align = "left">Momento característico máximo devido cargas variáveis (M<sub>max,qk</sub>)</td>
    <td>0</td>
    <td>kNm</td>
  </tr>
  <tr>
    <td align = "left">Momento característico mínimo devido cargas variáveis (M<sub>min,qk</sub>)</td>
    <td>0</td>
    <td>kNm</td>
  </tr>
  <tr>
    <td align = "left">Resistência característica do concreto (f<sub>ck</sub>)</td>
    <td>25</td>
    <td>MPa</td>
  </tr>
  <tr>
    <td align = "left">Resistência característica do aço CA-50 (f<sub>yk</sub>)</td>
    <td>500,00</td>
    <td>MPa</td>
  </tr>
  <tr>
    <td align = "left">Coeficiente de ponderação para carga permanente (γ<sub>g</sub>)</td>
    <td>1,40</td>
    <td>-</td>
  </tr>
  <tr>
    <td align = "left">Coeficiente de ponderação para carga variável (γ<sub>q</sub>)</td>
    <td>1,40</td>
    <td>-</td>
  </tr>
  <tr>
    <td align = "left">Coeficiente de minoração para resistência do concreto (γ<sub>c</sub>)</td>
    <td>1,40</td>
    <td>-</td>
  </tr>
  <tr>
    <td align = "left">Coeficiente de minoração para resistência do aço (γ<sub>s</sub>)</td>
    <td>1,15</td>
    <td>-</td>
  </tr>
</tbody>
</table>

<p align = "justify">
O primeiro passo é a determinação dos esforços de cálculo na viga (M<sub>Sd</sub>). No caso avalia-se o momento de cálculo para o valor máximo e valor mínimo de momento fletor. Lembrando que para o momento fletor mínimo negativo efetua-se o cálculo da armadura em módulo.
</p>

<table style = "width:100%">
  <tr>
    <td align = "center">\[M_{Sd} = M_{gk} \cdot \gamma_{g} + M_{qk} \cdot \gamma_{q}\]</td>
  </tr>
  <tr>
    <td align = "center">\[M_{Sd,max} = 1,9 \cdot 1,4 + 0 \cdot 1,4 = 2,66 \; \text{kN.m}\]</td>
  </tr>
  <tr>
    <td align = "center">\[M_{Sd,min} = 3,4 \cdot 1,4 + 0 \cdot 1,4 = 4,76 \; \text{kN.m}\]</td>
  </tr>
</table>

<p align = "justify">
Após isso determina-se o momento resistente dessa seção para verificação da possibilidade de armadura dupla. No caso a armadura simples é dada por M<sub>Sd</sub> ≤ M<sub>Rd,lim</sub>.
</p>

<table style = "width:100%">
  <tr>
    <td align = "center">\[M_{Rd,lim} = b_{w} \cdot d^2 \cdot \lambda \cdot \beta _x \cdot \alpha _c \cdot f_{cd} \left( 1 - 0,50 \cdot \lambda \cdot \beta _x \right)\]</td>
  </tr>
  <tr>
    <td align = "center">\[M_{Rd,lim} = 0,14 \cdot 0,396^2 \cdot 0,8 \cdot 0,45 \cdot 0,85 \cdot \frac{25000}{1,4} \left( 1 - 0,50 \cdot 0,8 \cdot 0,45 \right)\]</td>
  </tr>
  <tr>
    <td align = "center">\[M_{Rd,lim} = 98,371\; \text{kN.m}\]</td>
  </tr>
</table>

<p align = "justify">
No exemplo  M<sub>Rd,lim</sub> > M<sub>Sd</sub>.
</p>

<p align = "justify">
O terceiro passo, é a determinação da altura linha neutra x<sub>III</sub>, braço de alavanca z e armadura de flexão A<sub>s</sub>. Esse processo será repetido para cada momento o máximo e o mínimo:
</p>

<table>
  <tr>
    <td align = "center">\[x_{III} = \frac{d - \sqrt{( d^{2} - ( 2 \cdot \epsilon ) )}}{\lambda}\]</td>
  </tr>
  <tr>
    <td align = "center">\[\epsilon = \frac{M_{sd}}{bw \cdot \alpha_{c} \cdot \frac{f_{ck}}{\gamma_{c}}}\]</td>
  </tr>
  <tr>
    <td align = "center">\[z = d - (0,5 \cdot \lambda \cdot x_{III})\]</td>
  </tr>
  <tr>
    <td align = "center">\[A_s = {\frac{M_{Sd}}{z \cdot \frac{fyk}{\gamma s}}}\]</td>
  </tr>
</table>

<p align = "justify" id = "tab2"><b>Tabela 1.</b> Valores de área de aço da viga.</p>

<table style = "width:100%">
  <thead>
    <tr>
      <th>M<sub>Sd</sub> (kNm)</th>
      <th>ϵ (m²)</th>
      <th>x<sub>III</sub> (m)</th>
      <th>z (m)</th>
      <th>A<sub>s</sub> (m²)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>\[2,66\]</td>
      <td>\[0,0012518\]</td>
      <td>\[0,0039672\]</td>
      <td>\[0,3944131\]</td>
      <td>\[1,5511654\cdot 10^{-5}\]</td>
    </tr>
    <tr>
      <td>\[4,76\]</td>
      <td>\[0,00224\]</td>
      <td>\[0,0071219\]</td>
      <td>\[0,3931512\]</td>
      <td>\[2,7846791\cdot 10^{-5}\]</td>
    </tr>
  </tbody>
</table>

<p align = "justify">
Após a verificação de flexão pura deve-se verificar a viga para cisalhamento:
</p>

<table>
  <tr>
    <td align = "center">\[V_{Sd} = 4,1 \cdot 1,4 + 0 \cdot 1,4 = 5,74 \; \text{kN.m}\]</td>
  </tr>
  <tr>
    <td align = "center">\[ V_{Rd2} = 0,27 \cdot \alpha_{v2} \cdot f_{cd} \cdot b_{w} \cdot d \cdot (1+\cot(\alpha)) \]</td>
  </tr>
  <tr>
    <td align = "center">\[ V_{Rd2} = 0,27 \cdot \left ( 1-\frac{25}{250} \right ) \cdot \left ( \frac{25}{1,4} \right ) \cdot 0,14 \cdot 0,396 \cdot (1+\cot(90)) \]</td>
  </tr>
  <tr>
    <td align = "center">\[ V_{Rd2} = 240,57\; \text{kN}\]</td>
  </tr>  
</table>

<p align = "justify">
No caso a viga apresenta resistência da biela de compressão. E o próximo passo é a verificação da armadura necessária para o cisalhamento:
</p>

<table>
  <tr>
    <td align = "center">\[ \frac{A_{sw,\alpha}}{s} = \frac{V_{sw}}{0,9 \cdot d \cdot f_{ywd}\cdot(\sin(\alpha) + \cos(\alpha))} \]</td>
  </tr>
  <tr>
    <td align = "center">\[ \frac{A_{sw,\alpha}}{s} = \frac{5,74+\left ( 0,6\cdot \left ( \frac{0,7\cdot 0,3\cdot 25^{\frac{2}{3}}}{1,4} \right )\cdot 0,14\cdot 0,396 \right )}{0,9 \cdot 0,396 \cdot \left ( \frac{500}{1,15} \right ) \cdot(\sin(90) + \cos(90))} \]</td>
  <tr>
    <td align = "center">\[ \frac{A_{sw,\alpha}}{s} =  0,0001562\; \text{m²/m}\]</td>
  </tr>    
  </tr>
</table>
