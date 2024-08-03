---
title: Pilar P2
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
A seguir são apresentados os dados do pilar P2.
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
    <td>0,30</td>
    <td> m </td>
  </tr>
  <tr>
    <td align = "left">Altura na direção y (h<sub>y</sub>)</td>
    <td>0,14</td>
    <td> m </td>
  </tr>
  <tr>
    <td align = "left">Altura Útil Complementar (d')</td>
    <td>0,04</td>
    <td> m </td>
  </tr>
  <tr>
    <td align = "left">Carga de compressão característica devido carga permanente externa (N<sub>gext</sub>)</td>
    <td>-13,4</td>
    <td>kN</td>
  </tr>
  <tr>
    <td align = "left">Carga de compressão característica devido peso próprio (N<sub>gpp</sub>)</td>
    <td>-2,2</td>
    <td>kN</td>
  </tr>
  <tr>
    <td align = "left">Carga de compressão característica devida sobrecarga (N<sub>q</sub>)</td>
    <td>-3,5</td>
    <td>kN </td>
  </tr>
  <tr>
    <td align = "left">Momento fletor devido carga permanente externa na direção h<sub>x</sub> (M<sub>gext,x</sub>)</td>
    <td>5,0</td>
    <td>kNm</td>
  </tr>
  <tr>
    <td align = "left">Momento fletor devida sobrecarga na direção h<sub>x</sub> (M<sub>q,x</sub>)</td>
    <td>1,3</td>
    <td>kNm</td>
  </tr>
  <tr>
    <td align = "left">Momento fletor devido carga permanente externa na direção h<sub>y</sub> (M<sub>gext,y</sub>)</td>
    <td>0,102</td>
    <td>kNm</td>
  </tr>
  <tr>
    <td align = "left">Momento fletor devida sobrecarga na direção h<sub>y</sub> (M<sub>q,y</sub>)</td>
    <td>0,018</td>
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
    <td align = "center">\[M_{dmin} = N_{d} \cdot \left( 0,015 + 0,03 \cdot h \right) \]</td>
  </tr>
  <tr>
    <td align = "center">\[M_{dmin,x} = 10,03 \cdot \left( 0,015 + 0,03 \cdot 0,30 \right) = 15,13 kN.m \]</td>
  </tr>
  <tr>
    <td align = "center">\[M_{dmin,y} = 10,03 \cdot \left( 0,015 + 0,03 \cdot 0,14 \right) = 15,09 kN.m \]</td>
  </tr>
</table>


<p align = "justify">
Após a determinação do momento mínimo é necessário verificar o momento total de cálculo para o pilar. Para isso é necessário verificar três tipos de esforços. A carga de compressão total que atua no pilar N<sub>d</sub>. Deve-se salientar que para avaliar a carga de compressão é necessário avaliar as vigas que descarregam em cada um dos pilares e então efetuar a combinação corretamente.No pilar P2 atuam as reações de apoio das vigas <b>VC1</b> e <b>VC3</b>, prortantanto tem-se.
</p>

<table style = "width:100%">
  <tr>
    <td align = "center">\[ N_d = \left[ \left( 3,7 + 1,0 \right) + \left( 0,048 + 0,264 \right) + 2,152 \right] \cdot 1,4 = 10,03 kN.m \]</td>
  </tr>
  <tr>
    <td align = "center">\[ \text M_{dmin,x} = 15,13 kN.m \]</td>
  </tr>
  <tr>
    <td align = "center">\[ \text M_{dmin,y} = 15,09 kN.m \]</td>
  </tr>
</table>

<p align = "justify">
Os momentos de 1ª ordem serão os maiores entre o momentos inicias combinados (M_d) e os momentos mínimos (M_{dmin}). Dados os momentos de 1º ordem é necessário verificar a intensidade dos esforços de 2º que atuam no pilar de canto em questão. Porém para verificar os esforços de segunda ordem é necessário verificar as propriedades geométricas do pilar em cada direção.  
</p>

<table style = "width:100%">
  <tr>
    <td align = "center">\[ i_x = \sqrt{\frac{0,0000686}{0,042}} = 0,0404 \]</td>
  </tr>
  <tr>
    <td align = "center">\[ \lambda_x = \frac{4,16}{0,0404} = 102,93 \]</td>
  </tr>
  <tr>
    <td align = "center">\[ i_y = \sqrt{\frac{0,000315}{0,042}} = 0,0866\]</td>
  </tr>
  <tr>
    <td align = "center">\[ \lambda_y = \frac{4,16}{0,0866} = 48,03\]</td>
  </tr>
</table>

<p align = "justify">
A esbeltez limite é dada por:
</p>

<table>
  <tr>
    <td align = "center">\[ \lambda_ 1 = \frac{25 + 12,5 \cdot (e_1/h)}{\alpha _b} \]</td>
  </tr>
</table>

<p align = "justify" id = "tab2"><b>Tabela 1.</b> Valores de área de aço da viga.</p>

<p align = "justify">
No caso o valor de α<sub>b</sub> = 1,00 para peça biapoiadas sem carga transversal. Logo o valor de λ<sub>1</sub> é dado por:
</p>

<table>
  <tr>
    <td align = "center">\[ \lambda_ 1x = \frac{25 + 12,5 \cdot (1,51/0,3)}{1,0} = 219,68 \]</td>
  </tr>
  <tr>
    <td align = "center">\[ \lambda_ 1y = \frac{25 + 12,5 \cdot (1,50/0,14)}{1,0} = 159,30 \]</td>
  </tr>
</table>

<p align = "justify">
Após a determinação de quais peças terão esforços de segunda ordem é possível verificar o momento total de segunda ordem em cada direção. Para este exemplo será empregado o método da rigidez/curvatura equivalente. Neste caso, como os valores de lambda de comparação são maiores que os lambdas reais, tanto em x como em y, os momentos de segunda ordem não são consideerados:
</p>

<table>
  <tr>
    <td align = "center">\[ M_{2d,x} = 0,57 kN.m\]</td>
  </tr>
  <tr>
    <td align = "center">\[ M_{2d,y} = 1,23 kN.m\]</td>
  </tr>
</table>

<p align = "justify">
Determinados os momento de segunda ordem é possível determinar os momento totais em cada uma das direções do pilar, considerando que não há necessidade de contabilizar os efeitos de segunda ordem, os momentos totais são os de 1ª ordem.
</p>

<table>
  <tr>
    <td align = "center">\[ M_{dtot,x} = 15,73 kN.m\]</td>
  </tr>
  <tr>
    <td align = "center">\[ M_{dtot,y} = 16,34 kN.m\]</td>
  </tr>
</table>

<p align = "justify">
Determinado os esforços totais em cada uma das direções é possível determinar a área de aço total utilizando o conceito de ábacos. Para isso é necessário calcular a taxa de armadura total em cada direção:
</p>

<table>
  <tr>
    <td align = "center">\[ \mu_i = \frac{M_{dtot,i}}{h_i \cdot A_c \cdot f_cd}\]</td>
  </tr>
  <tr>
    <td align = "center">\[ \mu_x = 0,069\]</td>
  </tr>
   <tr>
    <td align = "center">\[ \mu_y = 0,15\]</td>
  </tr>
</table>

<p align = "justify">
Determinada a maior taxa de armadura é necessário verificar a área de aço total conforme cálculo abaixo:
</p>

<table>
  <tr>
    <td align = "center">\[ A_s = \frac{\omega \cdot A_c \cdot f_cd}{f_{\gamma d}}\]</td>
  </tr>
  <tr>
    <td align = "center">\[ A_s = 3,45 cm²\]</td>
  </tr>
</table>

<p align = "justify">
Determinada armadura total é possível estabelecer a armadura mínima do pilar conforme equação dada abaixo:
</p>

<table>
  <tr>
    <td align = "center">\[ A_{s,min} = 0,15 \cdot \frac{N_d}{f_{\gamma d}} \geq 0,004 \cdot A_c\]</td>
  </tr>
  <tr>
    <td align = "center">\[ A_{s,min} = 0,0346 cm²\]</td>
  </tr>
</table>

<p align = "justify">
Com o valor de área total de 3,45 cm² é possível detalhar a seção com 5 barras de 10 mm.
</p>
