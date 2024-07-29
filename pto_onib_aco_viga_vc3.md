---
title: Viga VC3
layout: default
grand_parent: Exemplo I
parent: Projeto vigas
nav_order: 7
has_children: false
has_toc: false
---

<!--Don't delete this script-->
<script src = "https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id = "MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
<!--Don't delete this script-->

<p align = "justify">
A seguir são apresentados os dados da viga VC3. 
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
    <td>14</td>
    <td>cm</td>
  </tr>
  <tr>
    <td align = "left">Altura (h)</td>
    <td>45</td>
    <td>cm</td>
  </tr>
  <tr>
    <td align = "left">Altura Útil (d)</td>
    <td>39,6</td>
    <td>cm</td>
  </tr>
  <tr>
    <td align = "left">Momento característico máximo devido cargas permanentes (M<sub>max,gk</sub>)</td>
    <td>0</td>
    <td>kNm</td>
  </tr>
  <tr>
    <td align = "left">Momento característico mínimo devido cargas permanentes (M<sub>min,gk</sub>)</td>
    <td>-3,379</td>
    <td>kNm</td>
  </tr>
  <tr>
    <td align = "left">Momento característico máximo devido cargas variáveis (M<sub>max,qk</sub>)</td>
    <td>0</td>
    <td>kNm</td>
  </tr>
  <tr>
    <td align = "left">Momento característico mínimo devido cargas variáveis (M<sub>min,qk</sub>)</td>
    <td>-0,614</td>
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
    <td align = "center">Msd = Mgk . 1,4 + Mqk . 1,4</td>
  </tr>
  <tr>
    <td align = "center">Msd,max = 0  . 1,4 + 0 . 1,4 = 0 kN.m</td>
  </tr>
  <tr>
    <td align = "center">Msd,min = -3,379 . 1,4 + -0,614 . 1,4 = -5,5902 kN.m</td>
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
    <td align = "center">\[M_{Rd,lim} = 0,14\cdot 0,396^2 \cdot 0,8 \0,8 \cdot 0,85 \ 0,01644\cdot \0,85\cdot 17,857 \left( 1 - 0,50 \cdot \0,8 \cdot \0,01644\right) = 5,55 kN.m]</td>
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
    <td align = "center">\[x_{III} = \frac{0.369 - \sqrt{( 0.369^{2} - ( 2 \cdot \0.00263) )}}{\0,8}\]</td>
  </tr>
  <tr>
    <td align = "center">\[\ = \frac{-5,5902}{0,14\cdot \0,85 \cdot \frac{25000}{\1,4}}\]</td>
  </tr>
  <tr>
    <td align = "center">\[z = 0,9996 - (0,5 \cdot \0,8 \cdot 0,991)\]</td>
  </tr>
  <tr>
    <td align = "center">\[A_s = {\frac{-5,502}{0,03316 \cdot \frac{50000}{\1,15}}}\]</td>
  </tr>
</table>

<p align = "justify" id = "tab2"><b>Tabela 1.</b> Valores de área de aço da viga.</p>

<table style = "width:100%">
  <thead>
    <tr>
      <th>M<sub>Sd</sub> (kNm)</th>
      <th>ξ</th>
      <th>x<sub>III</sub> (m)</th>
      <th>z (m)</th>
      <th>A<sub>s</sub> (m²)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>aqui aqui</td>
      <td>\[\epsilon = \frac{M_{sd}}{bw \cdot \alpha_{c} \cdot \frac{f_{ck}}{\gamma_{c}}}\]</td>
      <td>\[x_{III} = \frac{d - \sqrt{( d^{2} - ( 2 \cdot \epsilon ) )}}{\lambda}\]</td>
      <td>\[z = d - (0,5 \cdot \lambda \cdot x_{III})\]</td>
      <td>\[A_s = {\frac{M_{Sd}}{z \cdot \frac{fyk}{\gamma s}}}\]</td>
    </tr>
    <tr>
      <td>aqui aqui</td>
      <td>\[\epsilon = \frac{M_{sd}}{bw \cdot \alpha_{c} \cdot \frac{f_{ck}}{\gamma_{c}}}\]</td>
      <td>\[x_{III} = \frac{d - \sqrt{( d^{2} - ( 2 \cdot \epsilon ) )}}{\lambda}\]</td>
      <td>\[z = d - (0,5 \cdot \lambda \cdot x_{III})\]</td>
      <td>\[A_s = {\frac{M_{Sd}}{z \cdot \frac{fyk}{\gamma s}}}\]</td>
    </tr>
  </tbody>
</table>

<p align = "justify">
Após a verificação de flexão pura deve-se verificar a viga para cisalhamento:
</p>

<table>
  <tr>
    <td align = "center">\[V_{Sd} = 4,295 \cdot 1,4 + 1,536 \cdot 1,4 = 8,163 \; \text{kN.m}\]</td>
  </tr>
  <tr>
    <td align = "center">\[ V_{Rd2} = 0,27 \cdot \alpha_{v2} \cdot f_{cd} \cdot b_{w} \cdot d \cdot (1+\cot(\alpha)) \]</td>
  </tr>
  <tr>
    <td align = "center">\[ V_{Rd2} = 0,27 \cdot \alpha_{v2} \cdot f_{cd} \cdot b_{w} \cdot d \cdot (1+\cot(\alpha)) \]</td>
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
    <td align = "center">\[ \frac{A_{sw,\alpha}}{s} = \frac{V_{sw}}{0,9 \cdot d \cdot f_{ywd}\cdot(\sin(\alpha) + \cos(\alpha))} \]</td>
  </tr>
</table>
