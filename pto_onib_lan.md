---
title: Fôrma estrutural
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
As Figuras <a href="#fig1">1</a> e <a href="#fig1">2</a> apresentam a plantas de interferência estrutural dos pilares e vigas na arquitetura do edifício.
</p>

<table border = "0" style = "width:100%">
  <tr>
    <td><center><img src = "assets/images/interferencia_terreo.png" width = "100%"></center></td>
  </tr>
  <tr>
    <td><center><p align = "justify" id = "fig1"><b>Figura 1.</b> Interferência de pilares e vigas no térreo.</p></center></td>
  </tr>
  <tr>
    <td><center><img src = "assets/images/interferencia_cobertura.png" width = "100%"></center></td>
  </tr>
  <tr>
    <td><center><p align = "justify" id = "fig2"><b>Figura 2.</b> Interferência de pilares e vigas na cobertura.</p></center></td>
  </tr>
</table>

<h1>Pré-dimensionamento</h1>  

<p align = "justify">
A etapa de pré-dimensionamento pode ser realizada por qualquer grupo de elementos estruturais e isso irá depender da forma a qual você está mais acostumado. Primeiramente será estabelecida as dimensões das vigas, depois lajes e pilares.
</p>

<h3>Pré-dimensionamento das vigas</h3>  

<p align = "justify">
Realizaremos o pré-dimensionamento das vigas do térreo VT1 a VT4 e VC1 a VC3. A largura das vigas será especificada em 14 cm para que seja possível fazer o fechamento da alvenaria sem nenhum tipo de requadro. A excessão será a viga VC1 que terá esforços de torção então será estabelecida com largura de 20 cm.<br><br>
Apenas para critério de verificação será aplicado a relação \(l_0/50\) para verificar a largura mínima (\(b_{w,min}\)) conforme o item 15.10 da ABNT NBR 6118. No caso \(b_{w,min}=4,50/50=0,09\;m=9\;cm\)
<br><br>
Considerando que todas as peças serão biapoiadas a altura das vigas é dada conforme Tabela <a href="#tab1">1</a>.
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
        <td>VT3=VT4=VC2</td>
        <td>1,50</td>
        <td>\(h = 1,50/10 = 0,15\)</td>
        <td>0,45</td>
    </tr>
    <tr>
        <td>VC1</td>
        <td>4,50</td>
        <td>\(h = 4,50/10 = 0,45\)</td>
        <td>0,45</td>
    </tr>
    <tr>
        <td>VC3</td>
        <td>1,50</td>
        <td>\(h = 1,50/5 = 0,30\)</td>
        <td>0,45</td>
    </tr>
</table>

<p align = "justify">
As vigas VT3, VT4 e VC3 poderiam ter altura de 0,30 m (ou 30 cm) porém para manter o padrão das vigas vamos empregar a altura total de 0,45 m (ou 45 cm) para todas as vigas.
</p>

<h3>Pré-dimensionamento da laje</h3>  

<p align = "justify">
A determinação da espessura da laje é influenciada por suas dimensões em planta e seu carregamento. Para laje LC1 será considerada inicialmente o vão \(l_y=4,50\;m\) e \(l_x=1,50\;m\). No caso desta laje a relação entre vão é de 3,00 (\(\lambda=l_y/l_x\)).
</p>

<p align = "justify">
A espessura mínima segundo a ABNT NBR 6118 será de 0,10 m para a laje LC1 que é uma laje com um dos lados em balanço.<br><br>
A laje em balanço apresentará a seguinte altura \(h = 0,04 \cdot 1,50 = 0,06\;m\). No entanto a altura mínima exigida é de 0,10 m. Portanto será adotada a altura de 0,10 m para a laje em questão.
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

<p align = "justify">
Para iniciar o pré-dimensionamento de pilares deve-se atentar primeiramente em seguir as dimensões mínimas definidas pela ABNT NBR 6118, que estabelece no item 13.2.3, onde a seção transversal de pilares não deve ter dimensões menores que 19 cm, a menos que sejam casos especiais, preservando um valor mínimo de 14 cm para a menor dimensão da seção. Outra importante medida é a área mínima da seção transversal de um pilar que deve ser superior a 360 cm².
<br><br>
Além disso é necessário classificar os pilares deste projeto que neste caso são os pilares de canto P1, P2 e P3 (\( \alpha=2,50 \) para pré-dimensionamento).
</p>

<h4><i>Área de influência e verificação da área necessária</i></h4>  

<p align = "justify">
A Figura <a href="#fig4">4</a> apresenta a divisão do carregamento do painel de laje em função dos pilares (áreas de influência). Para isso usou-se a distribuição de carga em função do tipo de pilar.
</p>

<table border = "0" style = "width:100%">
  <tr>
    <td><center><img src = "assets/images/area_influencia.png" width = "150%"></center></td>
  </tr>
  <tr>
    <td><center><p align = "justify" id = "fig3"><b>Figura 4.</b> Distribuição do carregamento do painel nos pilares (áreas de influência).</p></center></td>
  </tr>
</table>

<p aligin = "justify">
O carregamento estimado para essa cobertura será de \( q=6\;kN/m² \). Com isso, é possível encontrar a força normal de cálculo para pré-dimensionamento. A Tabela <a href="#tab2">2</a> apresenta a força \( N_{sd}^{*} \).
  
<p align = "justify" id = "tab2"><b>Tabela 2.</b> Estimativa do carregamento nos pilares.</p>

<table style = "width:100%">
  <thead>
    <tr>
      <th>Pilar</th>
      <th>Área de influência (m²)</th>
      <th>\(N_{sd}^{*}\) (kN)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>P1</td>
      <td>1,52</td>
      <td>\(2,50 \cdot 1,52 \cdot 6 = 22,80\)</td>
    </tr>
    <tr>
      <td>P2</td>
      <td>3,37</td>
      <td>\(2,50 \cdot 3,37 \cdot 6 = 50,55\)</td>
    </tr>
    <tr>
      <td>P3</td>
      <td>1,86</td>
      <td>\(2,50 \cdot 1,86 \cdot 6 = 27,90\)</td>
    </tr>
  </tbody>
</table>

<p align = "justify">
Para este projeto será considerado um \(f_{ck}\) de 25 MPa (25.000 kPa) para as peças de concreto. Isso leva a um valor de \(f_{cd} = 25000/1,40=17857,14 kPa\).
<br><br>
Além disso vamos considerar que a tensão no aço para pré-dimensionamento será para um encurtamento de 0,2% nas armaduras sendo este valor igual a 420 MPa. Para a quantidade de armadura será adotado o valor de taxa mecânica de armadura igual a 2%.
<br><br>
Após a determinação da área de influência e a estimativa de carregamento no pavimento deve-se obter a área estimada de um pilar de concreto conforme a Tabela <a href="#tab3">3</a>.
</p>

<p align = "justify" id = "tab3"><b>Tabela 3.</b> Área de concreto necessária e dimensões finais.</p>

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
      <td>\[A_{c}=\frac{22,80}{0,85 \cdot 17857,14 + 0,02 \cdot 420000}=0,000967\]</td>
      <td>0,14</td>
      <td>\[h=0,000967/0,14=0,0069\]</td>
      <td>0,30</td>
      <td>\[0,042\;m²>0,036\;m²\]</td>
    </tr>
    <tr>
      <td>P2</td>
      <td>\[A_{c}=\frac{50,55}{0,85 \cdot 17857,14 + 0,02 \cdot 420000}=0,002144\]</td>
      <td>0,14</td>
      <td>\[h=0,002144/0,14=0,0153\]</td>
      <td>0,30</td>
      <td>\[0,042\;m²>0,036\;m²\]</td>
    </tr>
    <tr>
      <td>P3</td>
      <td>\[A_{c}=\frac{27,90}{0,85 \cdot 17857,14 + 0,02 \cdot 420000}=0,001183\]</td>
      <td>0,14</td>
      <td>\[h=0,001183/0,14=0,0085\]</td>
      <td>0,30</td>
      <td>\[0,042\;m²>0,036\;m²\]</td>
    </tr>
  </tbody>
</table>

<h1>Projeto executivo de fôrma</h1> 

<p align = "justify">
Definida a forma estrutural é necessário determinar os vãos efetivos de cada um dos elementos. No caso será aplicada a proposição das seções 14.6.2.4 e 15.6 da ABNT NBR 6118. 
</p>

<h3>Elemento isolado: laje</h3> 

<p align = "justify">
A definição do elemento isolado de laje será realizada conforme o equacionamento da seção 14.6.2.4 da ABNT NBR 6118. A proposição deste item é para sistema de vigas porém o mesmo pode ser aplicado para sistemas de laje.
<br><br>
Dado que todas as vigas tem largura de 14 cm ou 0,14 m a condição \(t/2\) será de 7 cm para todos os bordos. Para a condição \(0,30 \cdot h\) será empregada a altura da laje que é de 10 cm totalizando 3 cm. Logo o valor de vão efetivo é apresentado na Figura <a href="#fig5">5</a>.
</p>

<table border = "0" style = "width:100%">
  <tr>
    <td><center><img src = "assets/images/vao_ef_laje.png" width = "150%"></center></td>
  </tr>
  <tr>
    <td><center><p align = "justify" id = "fig3"><b>Figura 5.</b> Vão efetivo da laje.</p></center></td>
  </tr>
</table>

<h3>Elemento isolado: vigas</h3> 

<p align = "justify">
Para aplicar a metodologia descrita acima devemos considerar os pilares como elementos que servem de apoio para as vigas. Logo a condição \(t/2\) dependerá da direção do pilar. Como essa direção poderá variar em função da viga o valor de vão efetivo deverá ser acrescido das parcelas \(a_1\) e \(a_2\). A Tabela <a href="#tab3">3</a> apresenta estes detalhes:
</p>

<p align = "justify" id = "tab3"><b>Tabela 3.</b> Vão efetivo das vigas da cobertura.</p>

<table style = "width:100%">
  <thead>
    <tr>
      <th>Viga</th>
      <th>\(L_{0} \; (m)\)</th>
      <th>\(a_{1} \; (m)\)</th>
      <th>\(a_{2} \; (m)\)</th>
      <th>\(L_{ef} \; (m)\)</th>
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

<p align = "justify">
Como usaremos o sistema de pórtico plano para determinação dos esforços finais e então dimensionamento dos elementos faremos duas adequações para evitar imperfeições geométricas no modelo estrutural. A primeira é de que utilizaremos os vãos efetivos do pavimento superior para refletir o modelo estrutural do térreo. ¹Além disso o vão efetivo das vigas VC2 e VC3 serão igualados por critério de facilidade de determinação das dimensões do pórtico final. No caso o vão empregado será o da viga VC3.
</p>

<h3>Elemento isolado: pilares</h3> 

<p align = "justify">
Para os pilares será aplicada a condição da seção 15.6 da ABNT NBR 6118. Os resultados são apresentados na Tabela <a href="#tab4">4</a>. Vale salientar aqui que devido o pilar possuir duas "alturas" a determinação do vão efetivo deveria ser feito para as duas direções (h e b). Para este exemplo didático será determinada a altura efetiva relativa a viga VC1 e ela será a base para as outras direções. Tal condições não prejudica o cálculo estrutural neste exemplo em específico. Outra questão importante é de que apesar da altura ser determinada com essa condição de aproximação das dimensões, o comprimento de flambagem será diferente no dimensionamento dos pilares. Tal situação será abordada no detalhamento dos pilares.
<br><br>
Considerando que o pé esquerdo do projeto é de 2,20 m e que na posição da viga de cobertura a altura é de 0,45 m o vão livre \( \left( l_0 \right) \) é de 1,75 m.
</p>

<p align = "justify" id = "tab4"><b>Tabela 4.</b> Vão efetivo pilares.</p>

<table style = "width:100%">
  <thead>
    <tr>
      <th>\(l_{0} + h \; (m)\)</th>
      <th>\(l \; (m)\)</th>
      <th>\(l_{ef} \; (m)\)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>\[1,75 + 0,30 = 2,05\]</td>
      <td>\[1,75 + \frac{0,45}{2} \cdot 2 = 2,20\]</td>
      <td>\[2,05\]</td>
    </tr>
  </tbody>
</table>

<p align = "justify">
Logo podemos construir o diagrama de barras unifilares do projeto do ponto de ônibus e então fazer a determinação dos esforços e dimensionamento dos elementos estruturais. A Fgiura <a href="#fig6">6</a> apresenta o modelo determinado anteriormente.
</p>

<table border = "0" style = "width:100%">
  <tr>
    <td><center><img src = "assets/images/3d.png" width = "150%"></center></td>
  </tr>
  <tr>
    <td><center><p align = "justify" id = "fig6"><b>Figura 6.</b> Diagramas de barras unifilares que formam o pórtico 3D do projeto estrutural.</p></center></td>
  </tr>
</table>