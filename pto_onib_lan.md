---
title: Lançamento estrutural
layout: default
parent: Exemplo I
nav_order: 1
has_children: false
has_toc: false
---


<!--Don't delete this script-->
<script src = "https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id = "MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
<!--Don't delete this script-->

<h1>Lançamento de lajes, vigas e pilares</h1> 

<p align = "justify">
O lançamento estrutural seguirá as diretrizes para peças de concreto armado em geral. A seguir serão apresentados os passos para determinação da geometria inicial de cada um dos elementos.<br><br>
A Figura <a href="#fig1">(1)</a> apresenta a planta de interferência estrutural dos pilares na arquitetura do edifício. Já as Figuras <a href="#fig2">(2)</a> e <a href="#fig3">(3)</a> apresentam as interferências do restantes dos elementos estruturas que compõem o edfício.
</p>

<table border = "0" style = "width:100%">
  <tr>
    <td><center><img src = "assets/images/figura1.jpeg" width = "100%"></center></td>
  </tr>
  <tr>
    <td><center><p align = "justify" id = "fig1"><b>Figura 1.</b> Interferência de pilares.</p></center></td>
  </tr>
  <tr>
    <td><center><img src = "assets/images/figura2.jpeg" width = "150%"></center></td>
  </tr>
  <tr>
    <td><center><p align = "justify" id = "fig2"><b>Figura 2.</b> Pavimento térreo.</p></center></td>
  </tr>
  <tr>
    <td><center><img src = "assets/images/figura3.jpeg" width = "150%"></center></td>
  </tr>
  <tr>
    <td><center><p align = "justify" id = "fig3"><b>Figura 3.</b> Pavimento superior.</p></center></td>
  </tr>
</table>

<h1>Pré-dimensionamento</h1>  

<p align = "justify">
A etapa de pré-dimensionamento pode ser realizada por qualquer grupo de elementos estruturais e isso irá depender da forma a qual você está mais acostumado. Primeiramente será estabelecida as dimensões das vigas, depois lajes e pilares.
</p>

<h3>Pré-dimensionamento das vigas</h3>  

<p align = "justify">
Realizaremos o pré-dimensionamento das vigas do térreo VT1 a VT4 e VS1 a VS3. A largura das vigas será especificada em 14 cm para que seja possível fazer o fechamento da alvenaria sem nenhum tipo de requadro. A excessão será a viga VS1 que terá esforços de torção então será estabelecida com largura de 20 cm.<br><br>
Apenas para critério de verificação será aplicado a relação \(l_0/50\) para verificar a largura mínima (\(b_{w,min}\)) conforme o item 15.10 da ABNT NBR 6118. No caso \(b_{w,min}=4,50/50=0,09\;m=9\;cm\)
<br><br>
Considerando que todas as peças serão biapoiadas a altura das vigas é dada conforme Tabela <a href="#tab1">(1)</a>.
</p>

<p align = "justify" id = "tab1"><b>Tabela 1.</b> Pré-dimensionamento das vigas.</p>

<table border="0" style = "width:100%">
    <tr>
        <th>Viga</th>
        <th>Vão (m)</th>
        <th>\(h_{min}\) (m)</th>
        <th>\(h_{adot}\) (m)</th>
    </tr>
    <tr>
        <td>VT1=VT2</td>
        <td>4,50</td>
        <td>\(h = 4,50/10 = 0,45\)</td>
        <td>0,45</td>
    </tr>
    <tr>
        <td>VT3=VT4</td>
        <td>1,50</td>
        <td>\(h = 1,50/10 = 0,15\)</td>
        <td>0,45</td>
    </tr>
    <tr>
        <td>VS1</td>
        <td>4,50</td>
        <td>\(h = 4,50/10 = 0,45\)</td>
        <td>0,45</td>
    </tr>
    <tr>
        <td>VS2</td>
        <td>1,50</td>
        <td>\(h = 1,50/10 = 0,30\)</td>
        <td>0,45</td>
    </tr>
</table>

<p align = "justify">
As vigas VT3, VT4 e VS2 poderiam ter altura de 0,30 m (ou 30 cm) porém para manter o padrão das vigas vamos empregar a altura total de 0,45 m (ou 45 cm) para todas as vigas.
</p>

<h3>Pré-dimensionamento da laje</h3>  

<p align = "justify">
A determinação da espessura da laje é influenciada por suas dimensões em planta e seu carregamento. Para laje LS1 será considerada inicialmente o vão \(l_y=4,50\;m\) e \(l_x=1,50\;m\). No caso desta laje a relação entre vão é de 3,00 (\(\lambda=l_y/l_x\)).
</p>

<p align = "justify">
A espessura mínima segundo a ABNT NBR 6118 será de 0,10 m para a laje LS1 que é uma laje com um dos lados em balanço.<br><br>
A laje em balanço apresentará a seguinte altura \(h = 0,04 \cdot 1,50 = 0,06\;m\). No entanto a altura mínima exigida é de 10 cm. Portanto será adotada a altura de 0,10 m para a laje em questão.
</p>
<!-- 
<ul>
  <li><p align = "justify">7 cm para lajes de cobertura que não possuam balanço.</p></li>
  <li><p align = "justify">8 cm para lajes de piso que não possuam balanço.</p></li>
  <li><p align = "justify">10 cm para lajes que apresentam balanço, seja para cobertura ou piso.</p></li>
  <li><p align = "justify">12 cm para lajes sujeitas ao tráfego de veículos com peso de até três toneladas.</p></li>
  <li><p align = "justify">15 cm para lajes sujeitas ao tráfego de veículos com peso superior a três toneladas.</p></li>
</ul> -->

<h3>Pré-dimensionamento dos pilares</h3>  

<p aligin = "justify">
Para iniciar o pré-dimensionamento de pilares deve-se atentar primeiramente em seguir as dimensões mínimas definidas pela ABNT NBR 6118, que estabelece no item 13.2.3, onde a seção transversal de pilares não deve ter dimensões menores que 19 cm, a menos que sejam casos especiais, preservando um valor mínimo de 14 cm para a menor dimensão da seção. Outra importante medida é a área mínima da seção transversal de um pilar que deve ser superior a 360 cm².
<br><br>
Além disso é necessário classificar os pilares deste projeto que neste caso são os pilares de canto P1, P2 e P3 (\(\alpha=2,50 para pré-dimensionamento\)).
</p>

<h4><i>Área de influência e verificação da área necessária</i></h4>  

<p align = "justify">
A Figura <a href="#fig4">(4)</a> apresenta a divisão do carregamento do painel de laje em função dos pilares. Para isso usou-se a distribuição de carga em função do tipo de pilar.
</p>

<table border = "0" style = "width:100%">
  <tr>
    <td><center><img src = "assets/images/figura3.jpeg" width = "150%"></center></td>
  </tr>
  <tr>
    <td><center><p align = "justify" id = "fig3"><b>Figura 4.</b> Distribuição do carregamento do painel nos pilares.</p></center></td>
  </tr>
</table>

<p aligin = "justify">
O carregamento estimado para essa cobertura será de 6 \(kN/m²\). Com isso, é possível encontrar a a força normal de cálculo para pré-dimensionamento (\(N_sd^{*}=\alpha \cdot A_i \cdot q\)). A Tabela <a href="#tab2">(2)</a>.
  
<p align = "justify" id = "tab2"><b>Tabela 2.</b> Pré-dimensionamento de pilares.</p>

<table style = "width:100%">
  <thead>
    <tr>
      <th>Pilar</th>
      <th>Área de influência (m²)</th>
      <th>N_sd^{*} (kN/m²)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>P1</td>
      <td>1,671</td>
      <td>2,50 \cdot 1,671 \cdot 6 = </td>
    </tr>
    <tr>
      <td>P1</td>
      <td>1,671</td>
      <td>2,50 \cdot 1,671 \cdot 6 = </td>
    </tr>
  </tbody>
</table>

<p aligin = "justify">
Após a determinação da área de influência e carregamento estimado no pavimento deve-se obter a área estimada de um pilar de concreto conforme a equação <a href="#eq1">(1)</a>:
</p>

<table>
  <tr>  
    <td align = "left">\[A_{c}=\frac{N_{sd}^{*}}{0,85 \cdot f{cd} + \rho _s}\]</td>
    <td><p align = "rigth" id = "eq1">(1)</p></td>
  </tr>
</table>

<p aligin = "justify">
Com isso obtemos os resultados de área de concreto necessário para cada pilar:
</p>

<table>
  <thead>
    <tr>
      <th>Pilar</th>
      <th>Área de concreto (m²)</th>
      <th>Menor dimensão-\(b\) (m)</th>
      <th>Maior dimensão-\(h\) (m)</th>
      <th>\(h_{adot}\) (m)</th>
      <th>Área total (m²)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>P1</td>
      <td>9,67 \cdot 10^{-4} </td>
      <td>P1</td>
      <td>9,67 \cdot 10^{-4} </td>
      <td>P1</td>
      <td>P1</td>
    </tr>
    <tr>
      <td>P1</td>
      <td>9,67 \cdot 10^{-4} </td>
      <td>P1</td>
      <td>9,67 \cdot 10^{-4} </td>
      <td>P1</td>
      <td>P1</td>
    </tr>
    <tr>
      <td>P1</td>
      <td>9,67 \cdot 10^{-4} </td>
      <td>P1</td>
      <td>9,67 \cdot 10^{-4} </td>
      <td>P1</td>
      <td>P1</td>
    </tr>
  </tbody>
</table>

<h2>Definição das dimensões dos pilares</h2>

<p aligin = "justify">
Como é necessário admitir uma seção mínima de 360 cm² e tentando utilizar a menor dimensão nos pilares, vai ser adotado a dimensão mínima para o menor lado de 14 \(cm\) (dimensão \(b\)) e com isso é possível achar a outra dimensão do pilar (\(h\)). Para isso, deve ser feito:
</p>

COLOCA JÁ O RESULTADO FINAL EM FORMATO DE TABELA MESMO VOU FAZER UM EXEMPLO PARA VC...

<table>
<thead>
  <tr>
    <th>Pilar</th>
    <th>Área de concreto (\(m^2\))</th>
    <th>Dimensão \(b\) (\(m\))</th>
    <th>Dimensão \(h\) (\(m\))</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>P1</td>
    <td>9,67 \cdot 10^{-4}</td>
    <th>0,14 (\(m\))</th>
    <th>\( area = 0,14 \cdot b \therefore h =  0,30 \)</th>
  </tr>
    <tr>
    <td>P2</td>
    <td>2,36 \cdot 10^{-3}</td>
    <th>0,14 (\(m\))</th>
    <th>\( area = 0,14 \cdot b \therefore h =  0,30 \)</th>
  </tr>
    <tr>
    <td>P3</td>
    <td>9,67 \cdot 10^{-4}</td>
    <th>0,14 (\(m\))</th>
    <th>\( area = 0,14 \cdot b \therefore h =  0,30 \)</th>
  </tr>
</tbody>
</table>


