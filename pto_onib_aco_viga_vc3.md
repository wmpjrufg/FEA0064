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

<p aligin = "justify">
A seguir são apresentados os dados da viga VC1. 
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
    <td>aqui</td>
    <td>m</td>
  </tr>
  <tr>
    <td align = "left">Altura (h)</td>
    <td>aqui</td>
    <td>m</td>
  </tr>
  <tr>
    <td align = "left">Altura Útil (d)</td>
    <td>aqui</td>
    <td>m</td>
  </tr>
  <tr>
    <td align = "left">Momento característico máximo devido cargas permanentes (M<sub>max,gk</sub>)</td>
    <td>aqui</td>
    <td>kNm</td>
  </tr>
  <tr>
    <td align = "left">Momento característico mínimo devido cargas permanentes (M<sub>min,gk</sub>)</td>
    <td>aqui</td>
    <td>kNm</td>
  </tr>
  <tr>
    <td align = "left">Momento característico máximo devido cargas variáveis (M<sub>max,qk</sub>)</td>
    <td>aqui</td>
    <td>kNm</td>
  </tr>
  <tr>
    <td align = "left">Momento característico mínimo devido cargas variáveis (M<sub>min,qk</sub>)</td>
    <td>aqui</td>
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

<p aligin = "justify">
O primeiro passo é a determinação dos esforços de cálculo na viga (M<sub>Sd</sub>). No caso avalia-se o momento de cálculo para o valor máximo e valor mínimo de momento fletor. Lembrando que para o momento fletor mínimo negativo efetua-se o cálculo da armadura em módulo.
</p>

<table style = "width:100%">
  <tr>
    <td align = "center">\[M_{Sd} = M_{gk} \cdot \gamma_{g} + M_{qk} \cdot \gamma_{q}\]</td>
  </tr>
  <tr>
    <td align = "center">\[M_{Sd,max} = 4,295 \cdot 1,4 + 1,536 \cdot 1,4 = 8,163 \; \text{kN.m}\]</td>
  </tr>
  <tr>
    <td align = "center">\[M_{Sd,min} = 4,295 \cdot 1,4 + 1,536 \cdot 1,4 = 8,163 \; \text{kN.m}\]</td>
  </tr>
</table>

<p aligin = "justify">
Após isso determina-se o momento resistente dessa seção para verificação da possibilidade de armadura dupla. No caso a armadura simples é dada por M<sub>Sd</sub> ≤ M<sub>Rd,lim</sub>.
</p>

<table style = "width:100%">
  <tr>
    <td align = "center">\[M_{Rd,lim} = b_{w} \cdot d^2 \cdot \lambda \cdot \beta _x \cdot \alpha _c \cdot f_{cd} \left( 1 - 0,50 \cdot \lambda \cdot \beta _x \right)\]</td>
  </tr>
  <tr>
    <td align = "center">\[M_{Rd,lim} = b_{w} \cdot d^2 \cdot \lambda \cdot \beta _x \cdot \alpha _c \cdot f_{cd} \left( 1 - 0,50 \cdot \lambda \cdot \beta _x \right)\]</td>
  </tr>
</table>

<p aligin = "justify">
No exemplo  M<sub>Rd,lim</sub> > M<sub>Sd</sub>.
</p>

<p aligin = "justify">
O terceiro passo, é a determinação da altura linha neutra x<sub>III</sub> e o braço de alavanca z para cálculo da armadura .
</p>

<table>
  <tr>
    <td align = "center">\[x_{III} = \frac{d - \sqrt{( d^{2} - ( 2 \cdot \epsilon ) )}}{\lambda}\]</td>
  </tr>
  <tr>
    <td align = "center">\[x_{III} = \frac{2,5aqui_aqui - \sqrt{( 2,5^{2} - ( 2 \cdot \epsilon ) )}}{\lambda}\]</td>
  </tr>
  <tr>
    <td align = "center">\[\epsilon = \frac{M_{sd}}{bw \cdot \alpha_{c} \cdot \frac{f_{ck}}{\gamma_{c}}}\]</td>
  </tr>
  <tr>
    <td align = "center">\[\epsilon = \frac{M_{sd}}{bw \cdot \alpha_{c} \cdot \frac{f_{ck}}{\gamma_{c}}}\]</td>
  </tr>
  <tr>
    <td align = "center">\[z = d - (0,5 \cdot \lambda \cdot x_{III})\]</td>
  </tr>
  <tr>
    <td align = "center">\[z = d - (0,5 \cdot \lambda \cdot x_{III})\]</td>
  </tr>
</table>

<p aligin = "justify">
Dessa forma, com o valor do braço de alvanca z é possível determinar a área de aço da peça:
</p>

<table>
  <tr>
    <td align = "center">\[A_s = {\frac{M_{Sd}}{z \cdot \frac{fyk}{\gamma s}}}\]</td>
  </tr>
  <tr>
    <td align = "center">\[A_s = {\frac{M_{Sd}}{z \cdot \frac{fyk}{\gamma s}}}\]</td>
  </tr>
<table>