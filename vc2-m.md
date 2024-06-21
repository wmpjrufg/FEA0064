---
title: projeto viga vc2 momento
layout: default
parent: Exemplo I
nav_order: 400
has_children: false
has_toc: false
---

<!--Don't delete this script-->
<script src = "https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id = "MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
<!--Don't delete this script-->

<h1>Etapas para verificação da viga em flexão pura</h1>  

<p aligin = "justify">
A seguir, estão os passos gerais envolvidos no projeto de flexão pura para uma viga de concreto armado: 
</p>

<ol>
  <li>Determinação dos esforços da viga (cargas permanentes e variáveis)</li>
  <li>Determinação do momento Resistente de Cálculo</li>
  <li>Determinação da altura da linha neutra</li>
  <li>Armadura final</li>
</ol>

<h2>Dados da viga de referência</h2>  
<p aligin = "justify">
A seguir são apresentados os dados da viga V1. 
</p>

<table>
<thead align="center">
  <tr>
    <th>Variável</th>
    <th>Valor</th>
    <th>Unidade</th>
  </tr>
</thead>
<tbody align="center">
  <tr>
    <td align = "left">Largura da seção transversal (\(bw\))</td>
    <td>0,14</td>
    <td>\(m\)</td>
  </tr>
  <tr>
    <td align = "left">Altura (\(h\))</td>
    <td>0,3</td>
    <td>\(m\)</td>
  </tr>
  <tr>
    <td align = "left">Altura Útil (\(d\))</td>
    <td>0,250</td>
    <td>\(m\)</td>
  </tr>
  <tr>
    <td align = "left">Momento característico devido cargas permanentes (\(M_{gk}\))</td>
    <td>0,414</td>
    <td>\(kN.m\)</td>
  </tr>
  <tr>
    <td align = "left">Momento característico devido cargas variáveis (\(M_{qk}\))</td>
    <td>0,112</td>
    <td>\(kN.m\)</td>
  </tr>
  <tr>
    <td align = "left">Resistência característica do concreto (\(f_{ck}\))</td>
    <td>25</td>
    <td>\(MPa\)</td>
  </tr>
  <tr>
    <td align = "left">Resistência característica do aço CA-50 (\(f_{ywk}\))</td>
    <td>500</td>
    <td>\(MPa\)</td>
  </tr>
  <tr>
    <td align = "left">Coeficiente de ponderação para carga permanente (\(\gamma_{g}\))</td>
    <td>1,4</td>
    <td>\(-\)</td>
  </tr>
  <tr>
    <td align = "left">Coeficiente de ponderação para carga variável (\(\gamma_{q}\))</td>
    <td>1,4</td>
    <td>\(-\)</td>
  </tr>
  <tr>
    <td align = "left">Coeficiente de minoração para resistência do concreto (\(\gamma_{c}\))</td>
    <td>1,4</td>
    <td>\(-\)</td>
  </tr>
  <tr>
    <td align = "left">Coeficiente de minoração para resistência do aço (\(\gamma_{s}\))</td>
    <td>1,15</td>
    <td>\(-\)</td>
  </tr>
</tbody>
</table>

<p aligin = "justify">
Diagrama de momento devido cargas permanentes (FTOOL):
<br>
<img src="https://i.imgur.com/1nK2O9A.jpg" alt="Diagrama de momento devido cargas permanentes">
<br>
Diagrama de momento devido cargas variáveis (FTOOL):
<br>
<img src="https://i.imgur.com/G67w7wo.jpg" alt="Diagrama de momento devido cargas variáveis (FTOOL)">
</p>

<h2>1. Determinação dos esforços da viga (cargas permanentes e variáveis)</h2>  

<p aligin = "justify">
O primeiro passo, é a determinação dos esforços da viga (cargas permanentese e variáveis) e com o auxílio da ferramenta Ftool a determinação dos Momento Característico (Msk) e posteriormente o Momento de Cálculo (Msd), tanto devido a cargas variáveis quanto permanentes. A equação <a href="#eq1">(1)</a> apresenta o valor do momento de cáclulo:
</p>

<table>
  <tr>
    <td align = "left">\[M_{sd} = M_{gk} \cdot \gamma_{g} + M_{qk} \cdot \gamma_{q}\]</td>
    <td><p align = "right" id = "eq1">(1)</p></td>
  </tr>
</table>

<p aligin = "justify">
Portanto, tem-se que:
</p>

<p>
\[M_{sd} = 4,295 \cdot 1,4 + 1,536 \cdot 1,4 = 8,163 \, \text{kN.m}\]
</p>

<h2>2. Determinação do momento Resistente de Cálculo</h2>

<p aligin = "justify">
O segundo passo, é a verificação do Momento Resistente de Cálculo (Mrd) para determinação do tipo de armadura a ser utilizado. Tal valor pode ser encontrado por meio da equação <a href="#eq2">(2)</a>.
</p>

<table>
  <tr>
    <td align = "left">\[M_{rd, lim} = bw \cdot d^{2} \cdot \beta \cdot \alpha_{c} \cdot f_{cd} \cdot [ 1 - ( 0,5 \cdot \lambda \cdot \beta ) ]\]</td>
    <td><p align = "right" id = "eq2">(2)</p></td>
  </tr>
</table>

<p aligin = "justify">
Para o caso apresentado, tem-se que:
</p>

<table>
  <thead align="center">
    <tr>
      <th>Variável</th>
      <th>Valor</th>
      <th>Observação</th>
    </tr>
  </thead>
  <tbody align="center">
    <tr>
      <td>\(\beta\)</td>
      <td>0,45</td>
      <td>\(f_{ck} \leq f_{yk}\)</td>
    </tr>
    <tr>
      <td>\(\lambda\)</td>
      <td>0,80</td>
      <td>\(f_{ck} \leq 50 \, \text{MPa}\)</td>
    </tr>
    <tr>
      <td>\(\alpha_{c}\)</td>
      <td>0,85</td>
      <td>Para concretos até C50</td>
    </tr>
  </tbody>
  </table>

<p aligin = "justify">
  Logo, aplicando-se a equação <a href="#eq2">(2)</a>, tem-se que:
</p>

<p>
  \[M_{rd, lim} = 0,14 \cdot 0,255^{2} \cdot 0,45 \cdot 0,85 \cdot \frac{25000}{1,4} \cdot [ 1 - ( 0,5 \cdot 0,80 \cdot 0,45 ) ] = 40,79 \, \text{kN.m}\]
</p>

<p aligin = "justify">
Dessa forma constata-se que \(M_{sd} \leq M_{rd,lim}\), logo deve-se realizar uma armadura simples.
</p>

<h2>3. Determinação da altura da linha neutra</h2>

<p aligin = "justify">
O terceiro passo, é a determinação da altura linha neutra (\(X_{III}\)).
</p>

<table>
  <tr>
    <td align = "left">\[X_{III} = \frac{d - \sqrt{( d^{2} - ( 2 \cdot \epsilon ) )}}{\lambda}\]</td>
    <td><p align = "right" id = "eq3">(3)</p></td>
  </tr>
  <tr>
    <td align = "left">\[\epsilon = \frac{M_{sd}}{bw \cdot \alpha_{c} \cdot \frac{f_{ck}}{\gamma_{c}}}\]</td>
    <td><p align = "right" id = "eq4">(4)</p></td>
  </tr>
  <tr>
    <td align = "left">\[z = d - (0,5 \cdot \lambda \cdot X_{III})\]</td>
    <td><p align = "right" id = "eq5">(5)</p></td>
  </tr>
</table>

<p aligin = "justify">
  Logo, aplicando-se as equações <a href="#eq3">(3)</a> e <a href="#eq4">(4)</a> respectivamente, tem-se que:
</p>

<p>
  \[\epsilon = \frac{8,163}{0,14 \cdot 0,85 \cdot \frac{25000}{1,4}} = 0,00384\]

  \[X_{III} = \frac{0,255 - \sqrt{( 0,255^{2} - ( 2 \cdot 0,00384 ) )}}{0,80} = 0,02 \, \text{m}\]
</p>

<p aligin = "justify">
Com isso, é possível calcular a distância do ponto de aplicação da resultante das tensões normais de compressão no concreto e da resultante das tensões normais de tração do aço, o braço de alavanca \(z\) por meio da equação <a href="#eq5">(5)</a>:
</p>

<p>
\[z = 0,255 - (0,5 \cdot 0,80 \cdot 0,02) = 0,25 \, \text{m}\]
</p>

<h2>4. Armadura Final</h2>

<p aligin = "justify">
Dessa forma, com os valores do braço de alvanca \(z\) <a href="#eq5">(5)</a>: e \(Msd\) <a href="#eq1">(1)</a>:, é possível calcular a Aréa de Aço Final (As). Por meio da Equação <a href="#eq6">(6)</a>.
</p>

<table>
  <tr>
    <td align = "left">\[As = {\frac{Msd}{z*\frac{fyk}{\gamma s}}}\]</td>
    <td><p align = "right" id = "eq6">(6)</p></td>
  </tr>
  <tr>
  <table>

<p aligin = "justify">
  Logo, aplicando-se a equação <a href="#eq6">(6)</a> tem-se que armadura final para a flexão é:
</p>

<p>
\[As = {\frac{8,163}{0,25*\frac{500000}{1,15}}} = 7,59*10^-5 \, \text{m²}\]
</p>
