---
title: Pilar P1
layout: default
grand_parent: Exemplo I
parent: Projeto pilares
nav_order: 1
has_children: false
has_toc: false
---

<!--Don't delete this script-->
<script src = "https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id = "MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
<!--Don't delete this script-->

<p align = "justify">
A seguir são apresentados os dados do pilar P1.
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
    <td align = "left">Altura na direção x (h<sub>x</sub>)</td>
    <td>aqui</td>
    <td>m</td>
  </tr>
  <tr>
    <td align = "left">Altura na direção y (h<sub>y</sub>)</td>
    <td>aqui</td>
    <td>m</td>
  </tr>
  <tr>
    <td align = "left">Altura Útil Complementar (d')</td>
    <td>0,04</td>
    <td>m</td>
  </tr>
  <tr>
    <td align = "left">Carga compressão externa (N<sub>gext</sub>)</td>
    <td>aqui</td>
    <td>kNm</td>
  </tr>
  <tr>
    <td align = "left">Carga compressão p.p. (N<sub>gpp</sub>)</td>
    <td>aqui</td>
    <td>kNm</td>
  </tr>
  <tr>
    <td align = "left">Momento característico máximo devido cargas permanentes (M<sub>max,gk</sub>)</td>
    <td>9,1</td>
    <td>kNm</td>
  </tr>
  <tr>
    <td align = "left">Momento característico mínimo devido cargas permanentes (M<sub>min,gk</sub>)</td>
    <td>5,1</td>
    <td>kNm</td>
  </tr>
  <tr>
    <td align = "left">Momento característico máximo devido cargas variáveis (M<sub>max,qk</sub>)</td>
    <td>2,4</td>
    <td>kNm</td>
  </tr>
  <tr>
    <td align = "left">Momento característico mínimo devido cargas variáveis (M<sub>min,qk</sub>)</td>
    <td>1,4</td>
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
O primeiro passo é a determinação dos esforços mínimos para cada direção do pilar. Logo será aplicada a equação de momento mínimo:
</p>

<table style = "width:100%">
  <tr>
    <td align = "center">\[M_{dmin} = N_{d} \cdot \gamma_{g} + M_{qk} \cdot \gamma_{q}\]</td>
  </tr>
  <tr>
    <td align = "center">\[M_{Sd,max} = 9,1 \cdot 1,4 + 2,4 \cdot 1,4 = 16,1 \; \text{kN.m}\]</td>
  </tr>
  <tr>
    <td align = "center">\[M_{Sd,min} = 5,1 \cdot 1,4 + 1,4 \cdot 1,4 = 9,1 \; \text{kN.m}\]</td>
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
    <td align = "center">\[M_{Rd,lim} = 0,14 \cdot 0,396^2 \cdot 0,8 \cdot 0,45 \cdot 0,85 \cdot 25000 \left 1,4 \cdot( 1 - 0,50 \cdot 0,8 \cdot 0,45 \right) = 98,37 \]</td>
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
      <th>ξ</th>
      <th>x<sub>III</sub> (m)</th>
      <th>z (m)</th>
      <th>A<sub>s</sub> (m²)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>16,1</td>
      <td>\[\epsilon = \frac{16,1}{0,14 \cdot 0,85 \cdot \frac{25000}{0,85}}\]</td>
      <td>\[x_{III} = \frac{0,396 - \sqrt{( 0,396^{2} - ( 2 \cdot 0,0075 ) )}}{0,8}\]</td>
      <td>\[z = 0,396 - (0,5 \cdot 0,8 \cdot 0,02)\]</td>
      <td>\[A_s = {\frac{16,1}{0,39 \cdot \frac{500000}{1,15}}\]</td>
    </tr>
    <tr>
      <td>9,1</td>
      <td>\[\epsilon = \frac{9,1}{0,14 \cdot 0,85 \cdot \frac{25000}{0,85}}\]</td>
      <td>\[x_{III} = \frac{0,396 - \sqrt{( 0,396^{2} - ( 2 \cdot 0,0075 ) )}}{0,8}\]</td>
      <td>\[z = 0,396 - (0,5 \cdot 0,8 \cdot 0,02)\]</td>
      <td>\[A_s = {\frac{9,1}{0,39 \cdot \frac{500000}{1,15}}\]</td>
    </tr>
  </tbody>
</table>

<p align = "justify">
Após a verificação de flexão pura deve-se verificar a viga para cisalhamento:
</p>

<table>
  <tr>
    <td align = "center">\[V_{Sd} = 13,6 \cdot 1,4 + 3,6 \cdot 1,4 = 24,08 \; \text{kN.m}\]</td>
  </tr>
  <tr>
    <td align = "center">\[ V_{Rd2} = 0,27 \cdot (1-(25000/250000) \cdot (25000/1,4) \cdot 0,14 \cdot 0,396 \]</td>
  </tr>
  <tr>
    <td align = "center">\[ V_{Rd2} = 240,57 \]</td>
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
