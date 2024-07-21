---
title: Esforços
layout: default
parent: Exemplo I
nav_order: 3
has_children: True
has_toc: True
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
    <td><center><img src = "assets/images/vistas.png" width = "100%"></center></td>
  </tr>
  <tr>
    <td><center><p align = "justify" id = "fig1"><b>Figura 1.</b> Indicação de vistas para determinar os pórticos.</p></center></td>
  </tr>
</table>

<p align = "justify">
Os pórticos no Ftool podem ser baixados a seguir:
</p>

<ul>
  <li><a target="_blank" rel="noopener" href="https://github.com/wmpjrufg/FEA0064/blob/gh-pages/portico_p1_vt1_p2_vc1.ftl">Pórtico vista P1-VT1-P2-VC1</a>;</li>
  <li><a target="_blank" rel="noopener" href="https://github.com/wmpjrufg/FEA0064/blob/gh-pages/portico_p3_vt3_p1_vc2.ftl">Pórtico vista P3-VT3-P1-VC2</a>;</li>
  <li><a target="_blank" rel="noopener" href="https://github.com/wmpjrufg/FEA0064/blob/gh-pages/portico_p3_vt2.ftl">Pórtico vista P3-VT2</a>;</li>
  <li><a target="_blank" rel="noopener" href="https://github.com/wmpjrufg/FEA0064/blob/gh-pages/portico_vt4_p2_vc3.ftl">Pórtico vista VT4-P2-VC3</a>.</li>
</ul>

<p align = "justify">
O módulo de elasticidade será considerado para o concreto classe 25 (f<sub>ck</sub> = 25 MPa) e com um agregado de granito com dimensão máxima de 19 mm.
</p>

<table border = "0" style = "width:100%">
    <tr>
        <td>\[ E_{ci} = 5600 \cdot \sqrt{25} = 28000 \; MPa = 28 \cdot 10^6 \; kPa \]</td>
    </tr>
    <tr>
        <td>\[ \alpha_i = 0,80 + 0,20 \cdot + \frac{25}{80} = 0,86 \]</td>
    </tr>
    <tr>
        <td>\[ E_{cs} = 0,86 \cdot 28 \cdot 10^6 = 24,08 \cdot 10^6 \; kPa \]</td>
    </tr>
</table>

<p align = "justify">
A seguir são listadas as tabelas de esforços em cada uma das vistas para que seja possível efetuar o dimensionamento da estrutura por completo.
</p>
