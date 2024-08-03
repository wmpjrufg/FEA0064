---
title: Pilar P3
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
A seguir são apresentados os dados do pilar P3.
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
    <td>m</td>
  </tr>
  <tr>
    <td align = "left">Altura na direção y (h<sub>y</sub>)</td>
    <td>0,14</td>
    <td>m</td>
  </tr>
  <tr>
    <td align = "left">Altura Útil Complementar (d')</td>
    <td>0,04</td>
    <td>m</td>
  </tr>
  <tr>
    <td align = "left">Carga de compressão característica devido carga permanente externa (N<sub>gext</sub>)</td>
    <td>-2,386</td>
    <td>kN</td>
  </tr>
  <tr>
    <td align = "left">Carga de compressão característica devido peso próprio (N<sub>gpp</sub>)</td>
    <td>-2,236</td>
    <td>kN</td>
  </tr>
  <tr>
    <td align = "left">Carga de compressão característica devida sobrecarga (N<sub>q</sub>)</td>
    <td>-0,434</td>
    <td>kN</td>
  </tr>
  <tr>
    <td align = "left">Momento fletor devido carga permanente externa na direção h<sub>x</sub> (M<sub>gext,x</sub>)</td>
    <td>0</td>
    <td>kNm</td>
  </tr>
  <tr>
    <td align = "left">Momento fletor devida sobrecarga na direção h<sub>x</sub> (M<sub>q,x</sub>)</td>
    <td>0</td>
    <td>kNm</td>
  </tr>
  <tr>
    <td align = "left">Momento fletor devido carga permanente externa na direção h<sub>y</sub> (M<sub>gext,y</sub>)</td>
    <td>	0,009</td>
    <td>kNm</td>
  </tr>
  <tr>
    <td align = "left">Momento fletor devida sobrecarga na direção h<sub>y</sub> (M<sub>q,y</sub>)</td>
    <td>0,002</td>
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
      <td align = "center">\[M_{dmin,x} = 3,4314 \cdot \left( 0,015 + 0,03 \cdot 0,30 \right) \]</td>
  </tr>
  <tr>
    <td align = "center">\[M_{dmin,x} = 0,08235 \; \text{kNm} \]</td>
  </tr>  
  <tr>
      <td align = "center">\[M_{dmin,y} = 3,4314 \cdot \left( 0,015 + 0,03 \cdot 0,14 \right) \]</td>
  </tr>
  <tr>
    <td align = "center">\[M_{dmin,y} = 0,06588 \; \text{kNm} \]</td>
  </tr>    
</table>

<p align = "justify">
Após a determinação do momento mínimo é necessário verificar o momento total de cálculo para o pilar. Para isso é necessário verificar três tipos de esforços. A carga de compressão total que atua no pilar N<sub>d</sub>. Deve-se salientar que para avaliar a carga de compressão é necessário avaliar as vigas que descarregam em cada um dos pilares e então efetuar a combinação corretamente. Por exemplo no pilar P3 atuam apenas as reações de apoio da viga <b>VC2</b>.
</p>

<table style = "width:100%">
  <tr>
    <td align = "center">\[ N_d = \left[ \left( N_{gext,vc2} + N_{q,vc2} \right) + N_{gpp} \right] \cdot \gamma_f \]</td>
  </tr>
  <tr>
    <td align = "center">\[ N_d = \left[ \left( 0,182 +0,033 \right) +2,236 \right] \cdot 1,4 \]</td>
  </tr>
  <tr>
    <td align = "center">\[ N_d = 3,4314 \; \text{kN} \]</td>
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
Os valores obtidos foram os seguintes:  
</p>

<table style = "width:100%">
  <tr>
    <td align = "center">\[ i_x = \sqrt{\frac{\frac{(0,14\cdot 0,30^{3})}{12}}{0,14\cdot 0,30}} = 0,0866 \; \text{m}  \]</td>
  </tr>
  <tr>
    <td align = "center">\[ \lambda_x = \frac{2,13}{0,0866} = 24,595 \]</td>
  </tr>
  <tr>
    <td align = "center">\[ i_y = \sqrt{\frac{\frac{(0,30\cdot 0,14^{3})}{12}}{0,14\cdot 0,30}} = 0,0404 \; \text{m} \]</td>
  </tr>
  <tr>
    <td align = "center">\[ \lambda_y = \frac{2,13}{0,0404} = 52,7038 \]</td>
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
    <td align = "center">\[ \lambda_{1x} = \frac{25 + 12,5 \cdot ((\frac{0,08235}{3,4314})/0,30)}{1} \simeq 26 \to 35  \]</td>
  </tr>
  <tr>
    <td align = "center">\[ \lambda_{1y} = \frac{25 + 12,5 \cdot ((\frac{0,06588}{3,4314})/0,14)}{1} = 26,714 \to 35 \]</td>
  </tr>
</table>

<p align = "justify">
Após a determinação de quais peças terão esforços de segunda ordem (neste caso, apenas em y) é possível verificar o momento total de segunda ordem em cada direção. Para este exemplo será empregado o método da rigidez/curvatura equivalente. Os momentos de segunda ordem são dados a seguir:
</p>

<table>
  <tr>
    <td align = "center">\[ N_{c} = b \cdot h = 420 \; \text{cm²} \]</td>
  </tr>  
  <tr>
    <td align = "center">\[ \nu = \frac{3,4314}{420\cdot (\frac{2,5}{1,4})} = 0,004575 \]</td>
  </tr>    
  <tr>
    <td align = "center">\[ \frac{1}{r}=\frac{0,005}{14\cdot (0,004575+0,5)} = 0,0007078 \; \text{cm}^{-1} \]</td>
  </tr>    
  <tr>
    <td align = "center">\[ e_{2,y}=\frac{213^2}{10}\cdot 0,0007078 = 3,2112 \; \text{cm} \]</td>
  </tr>     
  <tr>
    <td align = "center">\[ M_{2d,y} = 3,2112 \cdot 3,4314 = 11,0189 \; \text{kNcm}\]</td>
  </tr>
</table>

<p align = "justify">
Determinados os momento de segunda ordem é possível determinar os momento totais em cada uma das direções do pilar.
</p>

<table>
  <tr>
    <td align = "center">\[ M_{d,x,total} = 8,235 \; \text{kNcm}\]</td>
  </tr>
  <tr>
    <td align = "center">\[ M_{d,y,total} = 11,0189 + 6,588 = 17,6069 \; \text{kNcm} \]</td>
  </tr>
</table>

<p align = "justify">
Determinado os esforços totais em cada uma das direções é possível determinar a área de aço total utilizando o conceito de ábacos. Para isso é necessário calcular a taxa de armadura total em cada direção:
</p>

<table>
  <tr>
    <td align = "center">\[ \mu _{i} = \frac{M_{d,total}}{h \cdot A_{c} \cdot f_{cd}} \]</td>
  </tr>
  <tr>
    <td align = "center">\[ \mu _{x} = \frac{-8,235}{30\cdot 420\cdot (\frac{2,5}{1,4})}= 0,000366 \]</td>
  </tr>  
  <tr>
    <td align = "center">\[ \mu _{y} = \frac{17,6069}{14\cdot 420\cdot (\frac{2,5}{1,4})} = 0,00167\]</td>
  </tr>
</table>

<p align = "justify">
Determinada a maior taxa de armadura é necessário verificar a área de aço total conforme cálculo abaixo:
</p>

<table>
  <tr>
    <td align = "center">\[ A_{s}=\frac{\omega \cdot A_{c}\cdot f_{cd}}{f_{\gamma d}} \]</td>
  </tr>
  <tr>
    <td align = "center">\[ A_{s}= 3,9655 \; \text{cm²} \]</td>
  </tr>
</table>

<p align = "justify">
Determinada armadura total é possível estabelecer a armadura mínima do pilar conforme equação dada abaixo:
</p>

<table>
  <tr>
    <td align = "center">\[ A _{s,min}= 0,15\cdot \frac{N_{d}}{f_{\gamma d}} \geq 0,004\cdot A_{c}\]</td>
  </tr>
  <tr>
    <td align = "center">\[ A _{s,min}= 0,15\cdot \frac{3,4314}{43,5} \geq 0,004\cdot 420 \]</td>
  </tr>
  <tr>
    <td align = "center">\[ A _{s,min}= 0,01183 \; \text{cm²} \geq 1,68 \; \text{cm²} \]</td>
  </tr>  
</table>

<p align = "justify">
Com o valor de área total de 3,9655 cm² é possível detalhar a seção com 4 barras de 12,5 mm.
  
<p align = "justify">
Observação: o valor de Nd para o P3 é muito pequeno e deu problema nos limites dos cálculo de 1/r e de As mín.
</p>
