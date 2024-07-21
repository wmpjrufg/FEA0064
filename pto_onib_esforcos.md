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
Os esforços serão determinados empregando método dos deslocamentos em função dos pórticos apresentados na seção anterior. Para essa determinação foi empregado o <i>software</i> Ftool. A disposição de vistas dos pórticos de concreto é apresentada na Figura <a href="#fig1">1</a>.
</p>

<table border = "0" style = "width:100%">
  <tr>
    <td><center><img src = "assets/images/charneiras.png" width = "100%"></center></td>
  </tr>
  <tr>
    <td><center><p align = "justify" id = "fig1"><b>Figura 1.</b> Indicação de vistas para determinar os pórticos.</p></center></td>
  </tr>
</table>

<p align = "justify">
Os pórticos no Ftool podem ser baixados a seguir:
</p>

<ul>
  <li><a target="_blank" rel="noopener" href="https://www.ftool.com.br/Ftool/">Pórtico vista A</a>;</li>
  <li><a target="_blank" rel="noopener" href="https://www.ftool.com.br/Ftool/">Pórtico vista B</a>;</li>
  <li><a target="_blank" rel="noopener" href="https://www.ftool.com.br/Ftool/">Pórtico vista C</a>;</li>
  <li><a target="_blank" rel="noopener" href="https://www.ftool.com.br/Ftool/">Pórtico vista D</a>.</li>
</ul>

<p align = "justify">
O módulo de elasticidade será considerado para o concreto classe 25 (f<sub>ck</sub> = 25 MPa) e com um agregado de granito com dimensão máxima de 19 mm.
</p>

<table border = "0" style = "width:100%">
    <tr>
        <td>\[ E_ci = 5600 \cdot \sqrt{25} = 28000 MPa = 28 \cdot 10^6 kPa \]</td>
    </tr>
    <tr>
        <td>\[ \alpha_i = 0,80 + 0,20 \cdot + \frac{25}{80} = 0,86 \]</td>
    </tr>
    <tr>
        <td>\[ E_cs = 0,86 \cdot 28 \cdot 10^6 = 24,08 \cdot 10^6 kPa \]</td>
    </tr>
</table>

<h1>Pórtico vista A</h1> 

<p align = "justify">
A carga que atua na laje LC1 será divida entre carregamento permanente e variável. O peso próprio da laje é obtido através da multiplicação do peso específico do concreto e a altura da laje, a qual tem o valor de 10 cm. Logo o valor deste carregamento é \(g_{pp}=0,10 \cdot 25 = 2,50\)kN/m².
<br><br>
Consultando a tabela 4 da ABNT NBR 6120 adotou-se como carga permanente o valor de carga para a manta de 10 cm com carga de 1,80 kN/m² \(\left(g_{ext}\right)\).<br><br>
Logo a carga total é dada por:
</p>

<table border = "0" style = "width:100%">
    <tr>
        <td>\[ g = g_{pp} + g_{ext} = 2,50+1,80=4,30\;kN/m²\]</td>
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
No caso deste projeto a laje LC1 fica engastada na viga VC1 visto que está é considerada uma laje unidirecional (\(\lambda>2,00\)). Portanto para evitar a formação de um mecanismo a mesma será considerada engastada em VC1. Logo a partição da carga é apresentada na Figura 
</p>



<p align = "justify">
No caso deste projeto o valor da A1 é de 4,83 m² e o valor de A2 é de 0,56 m². 
</p>

<p align = "justify" id = "tab3"><b>Tabela 3.</b> Vão efetivo das vigas da cobertura.</p>

<table style = "width:100%">
  <thead>
    <tr>
      <th>Viga</th>
      <th>\(L_{0} (m)\)</th>
      <th>\(a_{1} (m)\)</th>
      <th>\(a_{2} (m)\)</th>
      <th>\(L_{ef} (m)\)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>VC1</td>
      <td>3,90</td>
      <td>\[min \left(0,30/2,\;0,30 \cdot 0,45 \right) = 0,13\]</td>
      <td>\[min \left(0,30/2,\;0,30 \cdot 0,45 \right) = 0,13\]</td>
      <td>\[3,90+0,13\cdot2=4,16\]</td>
    </tr>
    <tr>
      <td>VC2</td>
      <td>1,06</td>
      <td>\[min \left(0,30/2,\;0,30 \cdot 0,45 \right) = 0,13\]</td>
      <td>\[min \left(0,14/2,\;0,30 \cdot 0,45 \right) = 0,07\]</td>
      <td>\[1,06+0,13+0,07=1,26\]</td>
    </tr>
    <tr>
      <td>VC3</td>
      <td>1,36</td>
      <td>não se aplica pois não tem apoio</td>
      <td>\[min \left(0,14/2,\;0,30 \cdot 0,45 \right) = 0,07\]</td>
      <td>\[1,36+0,07=1,43¹\]</td>
    </tr>
  </tbody>
</table>


<!-- <h3>Carregamento nas vigas do térreo</h3>
que nestede 11,5 cm de espessura e reboco e 0,50 cm em cada face totalizando 1,70 kN/m² conforme tabela 2 da ABNT NBR 6120. Além disso uma das faces da arquitetura exige um fechamento em vidro com espessura de 10 mm (Peso específico aparente de 22 kN/m³). -->