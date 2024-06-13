---
title: Esforços
layout: default
parent: Exemplo I
nav_order: 3
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
<li>Carga permanente: Peso próprio da estrutura, fechamento em vidro, fechamento em alvenaria e impermeabilização da cobertura;</li>
<li>Carga variável da cobertura.</li>
</ul>

<h1>Carga na laje</h1> 

<p align = "justify">
A carga que atua na laje LC1 será divida entre carregamento permanente e variável. O peso próprio da laje é obtido através da multiplicação do peso específico do concreto e a altura da laje, a qual tem o valor de 10 cm. Logo o valor deste carregamento é \(g_{pp}=0,10 \cdot 25 = 2,50\)kN/m².
<br><br>
Consultando a tabela 4 da ABNT NBR 6120 adotou-se como carga permanente o valor de carga para a manta de 10 cm com carga de 1,80 kN/m² \(\left(g_{ext}\right)\).<br><br>
Logo a carga total é dada por:
</p>

<table border = "0" style = "width:100%">
    <tr>
        <td style="width: 90%;">\[ g = g_{pp} + g_{ext} = 2,50+1,80=4,30\;kN/m²\]</td>
        <td style="width: 10%;"><p align = "right" id = "eq1">(1)</p></td>
    </tr>
</table>

<p align = "justify">
A carga variável selecionada para esse projeto é de 1,5 kN/m² considerando a possibilidade de instalação de placas fotovoltaicas.
</p>

<h1>Carga nas vigas do pavimento superior</h1> 

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
    <td><center><img src = "assets/images/figura1.jpeg" width = "100%"></center></td>
  </tr>
  <tr>
    <td><center><p align = "justify" id = "fig1"><b>Figura 1.</b> Proposta de arquitetura.</p></center></td>
  </tr>
</table>

<!-- <h3>Carregamento nas vigas do térreo</h3>
que nestede 11,5 cm de espessura e reboco e 0,50 cm em cada face totalizando 1,70 kN/m² conforme tabela 2 da ABNT NBR 6120. Além disso uma das faces da arquitetura exige um fechamento em vidro com espessura de 10 mm (Peso específico aparente de 22 kN/m³). -->