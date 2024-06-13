---
title: Carregamento
layout: default
parent: Exemplo I
nav_order: 2
has_children: false
has_toc: false
---

<!--Don't delete this script-->
<script src = "https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id = "MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
<!--Don't delete this script-->

<p align = "justify">
O carregamento será determinado conforme prescrição da ABNT NBR 6120. O memorial descreve que a cobertura será impermeabilizada. Portanto as cargas atuantes nessa estrutura podem ser descritas da seguinte forma:
</p>

<ul>
<li>Carga permanente: Peso próprio da estrutura, fechamento em vidro, fechamento em alvenaria, impermeabilização da cobertura;</li>
<li>Carga variável da cobertura.</li>
</ul>

<h1>Carga na laje</h1> 

<p align = "justify">
A carga que atua na laje LC1 será divida entre carregamento permanente e variável. O peso próprio da laje é obtido através da multiplicação do peso específico do concreto e a altura da laje, a qual tem o valor de 10 cm. Logo o valor deste carregamento é \( g_{pp}=0,10 \cdot 25 = 2,50 kN/m² \).
<br><br>
Consultando a tabela 4 da ABNT NBR 6120 adotou-se como carga permanente o valor de carga para a manta de 10 cm com carga de 1,80 kN/m² \(\left(g_{ext}\right)\).
<br><br>
Logo a carga total é dada por:
</p>

<table border = "0" style = "width:100%">
    <tr>
        <td style="width: 90%;">\[ g = g_{pp} + g_{ext} = 2,50+1,80=4,30 \]</td>
        <td style="width: 10%;"><p align = "right" id = "eq1">(1)</p></td>
    </tr>
</table>

<p align = "justify">
A carga variável selecionada para esse projeto é de 1,5 kN/m² considerando a possibilidade de instalação de placas fotovoltaicas.
</p>

<h1>Carga nas vigas</h1> 

<p align = "justify">
O carregamento nas vigas superiores é dependente das reações da laje LC1 nas vigas VC1, VC2 e VC3. Já as vigas do térreo suportam cargas de alvenarias de vedação rebocada e o fechamento em vidro temperado. Nesta seção serão apresentadas os carregamentos referentes das vigas do pavimento cobertura.
</p>

<h3>Reação da LC1 nas vigas da cobertura</h3> 

<p align = "justify">
Como dito anteriormente a laje LC1 suportará uma carga permanente de 4,30 kN/m² e uma carga variável de 1,50 kN/m². Para determinar as reações da laje nas vigas será necessário o uso do método de charneiras plásticas. Porém é necessário discutir o sistema de apoio das lajes nas vigas.
<br><br>
No caso deste projeto a laje LC1 fica engastada na viga VC1 visto que está é considerada uma laje unidirecional (\(\lambda>2,00\)). Portanto para evitar a formação de um mecanismo a mesma será considerada engastada em VC1. Logo a partição da carga é apresentada na Figura <a href="#fig1">1</a>.
</p>

<table border = "0" style = "width:100%">
  <tr>
    <td><center><img src = "assets/images/charneiras.png" width = "100%"></center></td>
  </tr>
  <tr>
    <td><center><p align = "justify" id = "fig1"><b>Figura 1.</b> Charneiras LC1.</p></center></td>
  </tr>
</table>

<p align = "justify">
No caso deste projeto o valor da A1 é de 4,83 m² e o valor de A2 é de 0,56 m². Logo é possível determinar a carga devido a reação da laje LC1 em todas as vigas da cobertura conforme Tabela <a href="#tab1">1.</a>
</p>

<p align = "justify" id = "tab1"><b>Tabela 1.</b> Carga nas vigas da cobertura.</p>

<table style = "width:100%">
  <thead>
    <tr>
      <th>Viga</th>
      <th>Área de influência (m²)</th>
      <th>Carga (kN/m²)</th>
      <th>Vão (m)</th>
      <th>Carga distribuída laje (kN/m)</th>
      <th>Carga distribuída p.p. (kN/m)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>VC1</td>
      <td>4,83</td>
      <td>\(g\)= 4,30</td>
      <td>4,16</td>
      <td>\[\frac{4,30 \cdot 4,83}{4,16} = 4,99\]</td>
      <td>\[\ 0,14 \cdot 0,45 \cdot 25 = 1,57\]</td>
    </tr>
    <tr>
      <td>VC1</td>
      <td>4,83</td>
      <td>\(q\)= 1,50</td>
      <td>4,16</td>
      <td>\[\frac{1,50 \cdot 4,83}{4,16} = 1,74\]</td>
      <td><center>-</center></td>
    </tr>
    <tr>
      <td>VC2=VC3</td>
      <td>0,56</td>
      <td>\(g\)= 4,30</td>
      <td>1,43</td>
      <td>\[\frac{4,30 \cdot 0,56}{1,43} = 1,68\]</td>
      <td>\[\ 0,14 \cdot 0,45 \cdot 25 = 1,57\]</td>
    </tr>
    <tr>
      <td>VC2=VC3</td>
      <td>0,56</td>
      <td>\(q\)= 1,50</td>
      <td>1,43</td>
      <td>\[\frac{1,50 \cdot 0,56}{1,43} = 0,59\]</td>
      <td><center>-</center></td>
    </tr>
  </tbody>
</table>

<h3>Carregamento nas vigas do térreo</h3>

<p align = "justify">
Considerando que a parede tem 15 cm de espessura foi selecionado neste projeto a alvenaria de vedação 11,5 cm de espessura e reboco em cada face de 2,00 cm totalizando 1,70 kN/m² (considerando 1,75 m de fechamento totaliza \(g_{alv}=2,97\;kN/m\)) conforme tabela 2 da ABNT NBR 6120. Além disso uma das faces da arquitetura exige um fechamento em vidro com espessura de 10 mm (peso específico aparente de 22 kN/m³) e altura de 1,75 m que totaliza \(g_{vidro}=22 \cdot 0,01 \cdot 1,75=0,38\;kN/m \). A Tabela <a href="#tab2">2</a> resume o carregamento nas vigas do térreo.
</p>

<p align = "justify" id = "tab2"><b>Tabela 2.</b> Carga nas vigas do térreo.</p>

<table style = "width:100%">
  <thead>
    <tr>
      <th>Viga</th>
      <th>Carga distribuída vedações (kN/m)</th>
      <th>Carga distribuída p.p. (kN/m)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>VT1=VT3</td>
      <td>2,97</td>
      <td>\[\ 0,14 \cdot 0,45 \cdot 25 = 1,57\]</td>
    </tr>
    <tr>
      <td>VT2</td>
      <td>0,00</td>
      <td>\[\ 0,14 \cdot 0,45 \cdot 25 = 1,57\]</td>
    </tr>
    <tr>
      <td>VT4</td>
      <td>0,38</td>
      <td>\[\ 0,14 \cdot 0,45 \cdot 25 = 1,57\]</td>
    </tr>
  </tbody>
</table>