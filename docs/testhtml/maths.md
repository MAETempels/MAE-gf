<body>
     
<h1>Mathematics</h1>

<h3>Contents</h3>
<ul>
  <li><a href="#mats-intr">Introduction</a></li>
  <li><a href="#mats-spin">Spiders formula</a></li>
  <li><a href="#mats-bigg">To big matrix</a></li>
</ul>

<h3 id="mats-intr">Introduction</h3>
<p>On this page some mathematics for those who like such. Including formula in pseudo-code.</p>

<h3 id="mats-spin">Spider formula's</h3>
<p>As shown in the <a href="https://github.com/MAETempels/MAE-gf/wiki/Spiders"><i>Spiders</i></a> article, spider-matrices can be generated. <br>
In all formula N is the number of legs on one side. The spider will thus have 4N legs. Spaces have to be ingored. The sign "&" means "concatenate": "A" & "B" => "AB". The "" are omitted.</p>  

<p>For the <b>traditional spider in a square</b>, the following code will do the trick. N>=2, tiling is set to <span class="elem">brick</span>.</p>
<pre><p class="form">
5 & (for i=1 to N: -) & 5 & (for i=1 to N: -)
-C & (for i=1 to N-2: D) & 632 & (for i=1 to N-2: A) & B
(for j=1 to N-2:
     5 & (for i=1 to N: 6) & 3 & (for i=1 to N: 2)
next j)
5 & (for i=1 to N: 6) & - & (for i=1 to N: 2)                 
</p></pre>

<h3 id="mats-bigg">To big matrix</h3>
<p><img alt="to big matrix" align="right" src="https://maetempels.github.io/MAE-gf/images/gf-sn-nott.png"> 
We wished to find the matrix-scheme for the crossed-snowflake-in-a-square. Just putting te snowflake in the square won't work, since the snowflake requires 11 "nodes", whereas the square has 9 nodes inside. So, the square has to be enlarged. The matrix in the picture follows the rules for matrices, but the tiles are too big for Groundforge to handle.</p>

<p><br><br><br><br><br><br></p>

<p><hr></p>
</body>