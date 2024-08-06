---
title: Pilar P1 com rigidez
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
    <td>0,14</td>
    <td>m</td>
  </tr>
  <tr>
    <td align = "left">Altura na direção y (h<sub>y</sub>)</td>
    <td>0,3</td>
    <td>m</td>
  </tr>
  <tr>
    <td align = "left">Altura Útil Complementar (d')</td>
    <td>0,04</td>
    <td>m</td>
  </tr>
  <tr>
    <td align = "left">Carga de compressão característica devido carga permanente externa (N<sub>gext</sub>)</td>
    <td>15,694</td>
    <td>kN</td>
  </tr>
  <tr>
    <td align = "left">Carga de compressão característica devido peso próprio (N<sub>gpp</sub>)</td>
    <td>2,153</td>
    <td>kN</td>
  </tr>
  <tr>
    <td align = "left">Carga de compressão característica devida sobrecarga (N<sub>q</sub>)</td>
    <td>3,94</td>
    <td>kN</td>
  </tr>
  <tr>
    <td align = "left">Momento fletor devido carga permanente externa na direção h<sub>x</sub> (M<sub>gext,x</sub>)</td>
    <td>0,064</td>
    <td>kNm</td>
  </tr>
  <tr>
    <td align = "left">Momento fletor devida sobrecarga na direção h<sub>x</sub> (M<sub>q,x</sub>)</td>
    <td>0,012</td>
    <td>kNm</td>
  </tr>
  <tr>
    <td align = "left">Momento fletor devido carga permanente externa na direção h<sub>y</sub> (M<sub>gext,y</sub>)</td>
    <td>5,03</td>
    <td>kNm</td>
  </tr>
  <tr>
    <td align = "left">Momento fletor devida sobrecarga na direção h<sub>y</sub> (M<sub>q,y</sub>)</td>
    <td>1,324</td>
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
    <td align = "center">\[M_{dmin} = 30,545 \cdot \left( 0,015 + 0,03 \cdot 0,14 \right) \]=0,586</td>
  </tr>
  <tr>
    <td align = "center">\[M_{dmin} = 30,545 \cdot \left( 0,015 + 0,03 \cdot 0,3 \right) \]=0,733</td>
  </tr>
</table>


<p align = "justify">
Após a determinação do momento mínimo é necessário verificar o momento total de cálculo para o pilar. Para isso é necessário verificar três tipos de esforços. A carga de compressão total que atua no pilar N<sub>d</sub>. Deve-se salientar que para avaliar a carga de compressão é necessário avaliar as vigas que descarregam em cada um dos pilares e então efetuar a combinação corretamente. Por exemplo no pilar P1 atuam as reações de apoio das vigas <b>VC1</b> e <b>VC2</b>.
</p>

<table style = "width:100%">
  <tr>
    <td align = "center">\[ N_d = \left[ \left( 13,4 + 3,5 \right) + \left( 2,34 + 0,425 \right) + 2,153 \right] \cdot \1,4 \]=30,545</td>
  </tr>
  <tr>
    <td align = "center">\[ \text(momento em x aqui) \]</td>
  </tr>
  <tr>
    <td align = "center">\[ \text(momento em y aqui) \]</td>
  </tr>
</table>

<p align = "justify">
Dados os momentos de 1º ordem é necessário verificar a intensidade dos esforços de 2º que atuam no pilar de canto em questão. Porém para verificar os esforços de segunda ordem é necessário verificar as propriedades geométricas do pilar em cada direção.  
</p>

<table style = "width:100%">
  <tr>
    <td align = "center">\[ i_x = \sqrt{\frac{I_x}{A}} \]</td>
  </tr>
  <tr>
    <td align = "center">\[ \lambda_x = \frac{l_e}{i_x} \]</td>
  </tr>
  <tr>
    <td align = "center">\[ i_y = \sqrt{\frac{I_y}{A}} \]</td>
  </tr>
  <tr>
    <td align = "center">\[ \lambda_y = \frac{l_e}{i_y} \]</td>
  </tr>
</table>

<p align = "justify">
A esbeltez limite é dada por:
</p>

<table>
  <tr>
    <td align = "center">\[ \lambda_ 1 = \frac{25 + 12,5 \cdot (e_1/h)}{\alfa_b} \]</td>
  </tr>
</table>

<p align = "justify" id = "tab2"><b>Tabela 1.</b> Valores de área de aço da viga.</p>

<p align = "justify">
No caso o valor de α<sub>b</sub> = 1,00 para peça biapoiadas sem carga transversal. Logo o valor de λ<sub>1</sub> é dado por:
</p>

<table>
  <tr>
    <td align = "center">\[ \lambda_ 1 = \frac{25 + 12,5 \cdot (0,165/0,3)}{\1} \]=31,875</td>
  </tr>
  <tr>
    <td align = "center">\[ \lambda_ 1 = \frac{25 + 12,5 \cdot (0,165/0,14)}{\1} \]=39,73</td>
  </tr>
</table>

<p align = "justify">
Após a determinação de quais peças terão esforços de segunda ordem é possível verificar o momento total de segunda ordem em cada direção. Para este exemplo será empregado o método da rigidez/curvatura equivalente. Os momentos de segunda ordem são dados a seguir:
</p>

<table>
  <tr>
    <td align = "center">\[ M_{d,x} = aqui\]</td>
  </tr>
  <tr>
    <td align = "center">\[ M_{d,x} = aqui\]</td>
  </tr>
</table>

<p align = "justify">
Determinados os momento de segunda ordem é possível determinar os momento totais em cada uma das direções do pilar.
</p>

<table>
  <tr>
    <td align = "center">\[ M_{d,x} = aqui\]</td>
  </tr>
  <tr>
    <td align = "center">\[ M_{d,x} = aqui\]</td>
  </tr>
</table>

<p align = "justify">
Determinado os esforços totais em cada uma das direções é possível determinar a área de aço total utilizando o conceito de ábacos. Para isso é necessário calcular a taxa de armadura total em cada direção:
</p>

<table>
  <tr>
    <td align = "center">\[ M_{d,x} = aqui\]</td>
  </tr>
  <tr>
    <td align = "center">\[ M_{d,x} = aqui\]</td>
  </tr>
</table>

<p align = "justify">
Determinada a maior taxa de armadura é necessário verificar a área de aço total conforme cálculo abaixo:
</p>

<table>
  <tr>
    <td align = "center">\[ M_{d,x} = aqui\]</td>
  </tr>
  <tr>
    <td align = "center">\[ M_{d,x} = aqui\]</td>
  </tr>
</table>

<p align = "justify">
Determinada armadura total é possível estabelecer a armadura mínima do pilar conforme equação dada abaixo:
</p>

<table>
  <tr>
    <td align = "center">\[ M_{d,x} = aqui\]</td>
  </tr>
  <tr>
    <td align = "center">\[ M_{d,x} = aqui\]</td>
  </tr>
</table>

<p align = "justify">
Com o valor de área total de xx cm² é possível detalhar a seção com xx barras de xx mm.
</p>
