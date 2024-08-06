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
    <td>0,14</td>
    <td>m</td>
  </tr>
  <tr>
    <td align = "left">Altura na direção y (h<sub>y</sub>)</td>
    <td>0,3</td>
    <td>m</td>
  </tr>  <tr>
    <td align = "left">Vão efetivo viga 2 (x) (l<sub>vc2</sub>)</td>
    <td>1,43</td>
    <td>m</td>
  </tr> 
  <tr>
    <td align = "left">Vão efetivo viga 1 (y) (l<sub>vc1</sub>)</td>
    <td>4,16</td>
    <td>m</td>
  </tr>
  <tr>
    <td align = "left">Altura do pilar 1 (l<sub>e</sub>)</td>
    <td>2,05</td>
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
    <td>3,940</td>
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
    <td align = "left">Coeficiente de ponderação para seção de 14cm (γ<sub>n</sub>)</td>
    <td>1,25</td>
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
    <td align = "center">\[ N_d = \left[ \left( N_{gext,vc1} + N_{q,vc1} \right) + \left( N_{gext,vc2} + N_{q,vc2} \right) + N_{gpp} \right] \cdot \gamma_f \cdot \gamma_n \]</td>
  </tr>
  <tr>
    <td align = "center">\[ N_d = \left[ \left( 13,354 + 3,515 \right) + \left( 2,340 + 0,425 \right) + 2,153 \right] \cdot 1,4 \cdot 1,25 = 38,127 kN \]</td>
  </tr>
  <tr>
    <td align = "center">\[M_{dmin} = N_d \cdot \left( 0,015 + 0,03 \cdot h \right) \]</td>
 <tr>
  <tr>
    <td align = "center">\[M_{dxmin} = 38,127 \cdot \left( 0,015 + 0,03 \cdot 0,14 \right) = 0,732 kN.m \]</td>
  </tr>
  <tr>
    <td align = "center">\[M_{dymin} = 38,127 \cdot \left( 0,015 + 0,03 \cdot 0,3 \right) = 0,915 kN.m \]</td>
  </tr>
</table>

<p align = "justify">
Após a determinação do momento mínimo é necessário verificar o momento total de cálculo para o pilar. Para isso é necessário verificar três tipos de esforços. A carga de compressão total que atua no pilar N<sub>d</sub>. Deve-se salientar que para avaliar a carga de compressão é necessário avaliar as vigas que descarregam em cada um dos pilares e então efetuar a combinação corretamente. Por exemplo no pilar P1 atuam as reações de apoio das vigas <b>VC1</b> e <b>VC2</b>.
</p>

<table style = "width:100%">
  <tr>
    <td align = "left">Rigidez do pilar </td>
  </tr>
  <tr>
    <td align = "center">\[R_p = \frac {\frac{b \cdot h ³}{12}}{l_e} \]</td>
  </tr>
  <tr>
    <td align = "center">\[R_p,x = \frac {\frac{h_y \cdot h_x ³}{12}}{l_e} = 3,35x10^-5 m³ \]</td>
  </tr>
   <tr>
    <td align = "center">\[R_p,y = \frac {\frac{h_x \cdot h_y ³}{12}}{l_e} = 1,54x10^-4 m³ \]</td>
  </tr>
  <tr>
    <td align = "left">Rigidez da viga </td>
  </tr>
  <tr>
    <td align = "center">\[R_v = \frac {\frac{b_v \cdot h_v ³}{12}}{l_vc} \]</td>
  </tr>
   <tr>
    <td align = "center">\[R_v,x = \frac {\frac{b_v \cdot h_v ³}{12}}{l_vc2} = 7,43x10^^-4 m³ \]</td>
  </tr>
  <tr>
    <td align = "center">\[R_v,y = \frac {\frac{b_v \cdot h_v ³}{12}}{l_vc1} = 2,56x10^^-4 m³ \]</td>
  </tr>
  <tr>
    <td align = "left"> Momentos de calculo </td>
  </tr>
  <tr>
    <td align = "center">\[M_k = (M_gext + M_q) \cdot 1,4 \cdot 1,25 \]</td>
  </tr>
  <tr>
    <td align = "center">\[M_{x} = (0,064 + 0,012) \cdot 1,4 \cdot 1,25 = 0,133 kN.m \]</td>
  </tr>
   <tr>
    <td align = "center">\[M_{y} = (5,03 + 1,324) \cdot 1,4 \cdot 1,25 = 11,120 kN.m \]</td>
  </tr>
  <tr>
    <td align = "left">Momentos superiores e inferiores </td>
  </tr>
   <tr>
    <td align = "center">\[M_{k,sup} = M_{k,inf} = \frac{ M_k \cdot R_p}{2 \cdot R_p + R_v} \]</td>
  </tr>
   <tr>
    <td align = "center">\[M_{kx,sup} = M_{kx,inf} = \frac{ M_{x} \cdot R_p,x}{2 \cdot R_p,x + R_v,x} = 5,49x10^-3 kN.m \]</td>
  </tr>
   <tr>
    <td align = "center">\[M_{ky,sup} = M_{ky,inf} = \frac{ M_{y} \cdot R_p,y}{2 \cdot R_p,y + R_v,y} = 3,04 kN.m \]</td>
  </tr>
  <tr>
    <td align = "left">Momentos de primeira ordem </td>
  </tr>  <tr>
    <td align = "center">\[M_{d1ªx} = M_{k,sup} + \frac{M_{k,sup}}{2} \]</td>
  </tr>
  <tr>
    <td align = "center">\[M_{d1ªx} = M_{kx,sup} + \frac{M_{kx,sup}}{2} = 0,008 kN.m \]</td>
  </tr>
  <tr>
    <td align = "center">\[M_{d1ªy} = M_{ky,sup} + \frac{M_{ky,sup}}{2} = 4,553 kN.m \]</td>
  </tr>
</table>

<p align = "justify">
Dados os momentos de 1º ordem é necessário verificar a intensidade dos esforços de 2º que atuam no pilar de canto em questão. Porém para verificar os esforços de segunda ordem é necessário verificar as propriedades geométricas do pilar em cada direção.  
</p>

<table style = "width:100%">
  <tr>
    <td align = "center">\[ i_x = \sqrt{\frac{\frac{0,3 \cdot 0,14³}{12}}{0,14 \cdot 0,3}} = 0,0404 m \]</td>
  </tr>
  <tr>
    <td align = "center">\[ \lambda_x = \frac{3,46 \cdot l_e}{h_x} = 50,66 \]</td>
  </tr>
  <tr>
    <td align = "center">\[ i_y = \sqrt{\frac{\frac{0,14 \cdot 0,3³}{12}}{0,14 \cdot 0,3}} = 0,0866 m \]</td>
  </tr>
  <tr>
    <td align = "center">\[ \lambda_y = \frac{3,46 \cdot l_e}{h_y} = 23,64 \]</td>
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
No caso o valor de α<sub>b</sub> = 1,00 para peça biapoiadas sem carga transversal, o valor da esbeltez deve respeitar a NBR 6118:2023 15.8.2, devemos usar um valor dentro do intervalor de 35 <= \lambda_ 1 <= 90. Logo o valor de λ<sub>1</sub> é dado por:
</p>

<table>
   <tr>
    <td align = "center">\[ e_1x = \frac{M_{d1ªx}}{N_d} = 2,16x10^-4 m \]</td>
  </tr>
  <tr>
    <td align = "center">\[ e_1y = \frac{M_{d1ªy}}{N_d} = 0,1194 m \]</td>
  </tr>
  <tr>
    <td align = "center">\[ \lambda_ 1x = \frac{25 + 12,5 \cdot (e_1x/hx)}{\alpha _b} = 25,02 \geq 35 \]</td>
  </tr>
  <tr>
    <td align = "center">\[ \lambda_ 1y = \frac{25 + 12,5 \cdot (e_1y/hy)}{\alpha _b} = 29,98 \geq 35 \]</td>
  </tr>
</table>

<p align = "justify">
Após a determinação de quais peças terão esforços de segunda ordem é possível verificar o momento total de segunda ordem em cada direção. Para este exemplo será empregado o método da curvatura equivalente. Os momentos de segunda ordem são os maiores momentos entre os minimos e o de primeira ordem já calculados:
</p>

<table>
  <tr>
    <td align = "center">\[ M_{d2ª,x} = 0,732 kN.m\]</td>
  </tr>
  <tr>
    <td align = "center">\[ M_{d2ª,y} = 4,553 kN.m \]</td>
  </tr>
</table>

<p align = "justify">
Determinados os momento de segunda ordem é possível determinar os momento totais em cada uma das direções do pilar.
</p>

<table>
   <tr>
    <td align = "center">\[ v = \frac{N_d}{A_c \cdot F_cd} = 0,051 \]</td>
  </tr>
   <tr>
    <td align = "center">\[ \frac{1}{r_x} = \frac{0,005}{h_x \cdot (v + 0,5)} = 0,065 \leq \frac{0,005}{h_x} = 0,036 \]</td>
  </tr>
   <tr>
    <td align = "center">\[ \frac{1}{r_y} = \frac{0,005}{h_y \cdot (v + 0,5)} = 0,030 \leq \frac{0,005}{h_y} = 0,017 \]</td>
  </tr>
     <tr>
    <td align = "center">\[ e_2x = \frac{1}{r_x} \cdot \frac{l_e²}{10} = 0,015 \]</td>
  </tr>
    <tr>
    <td align = "center">\[ e_2y = \frac{1}{r_y} \cdot \frac{l_e²}{10} = 0,007 \]</td>
  </tr>
  <tr>
    <td align = "center">\[ M_{dtot,x} = \alpha _b \cdot M_{d2ª,x} + N_d \cdot e_2x = 1,304 kN.m \]</td>
  </tr>
  <tr>
    <td align = "center">\[ M_{dtot,x} = \alpha _b \cdot M_{d2ª,y} + N_d \cdot e_2y = 4,820 kN.m \]</td>
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
    <td align = "center">\[ \mu_x = \frac{M_{dtot,x}}{h_x \cdot A_c \cdot f_cd} = 0,0124 \]</td>
  </tr>
   <tr>
    <td align = "center">\[ \mu_y = \frac{M_{dtot,y}}{h_y \cdot A_c \cdot f_cd} = 0,0214 \]</td>
  </tr>
</table>

<p align = "justify">
Determinada a maior taxa de armadura é necessário verificar a área de aço total conforme cálculo abaixo(ÁBACO 16-A, v=0,051, omega encontrado ω =0,2):
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
    <td align = "center">\[ A_{s,min1} = 1,68cm²\]</td>
  </tr>
</table>

<p align = "justify">
Com o valor de área total calculado de 3,45 cm² é possível detalhar a seção com 5 barras de 10 mm, essas 5 barras somam uma área de 3,93 cm².
</p>
