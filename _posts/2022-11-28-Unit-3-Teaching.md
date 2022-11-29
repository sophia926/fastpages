---
keywords: fastai
title: Title
nb_path: _notebooks/2022-11-28-Unit-3-Teaching.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2022-11-28-Unit-3-Teaching.ipynb
-->

<div class="container" id="notebook-container">
        
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">albums</span> <span class="o">=</span> <span class="p">[</span>
    <span class="p">(</span><span class="s2">&quot;Welcome to my Nightmare&quot;</span><span class="p">,</span> <span class="s2">&quot;Alice Cooper&quot;</span><span class="p">,</span> <span class="mi">1975</span><span class="p">,</span>   <span class="c1"># First album list</span>
     <span class="p">[</span>
         <span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="s2">&quot;Welcome to my Nightmare&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="mi">2</span><span class="p">,</span> <span class="s2">&quot;Devil&#39;s Food&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="mi">3</span><span class="p">,</span> <span class="s2">&quot;The Black Widow&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="mi">4</span><span class="p">,</span> <span class="s2">&quot;Some Folks&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="mi">5</span><span class="p">,</span> <span class="s2">&quot;Only Women Bleed&quot;</span><span class="p">),</span>
     <span class="p">]</span>
     <span class="p">),</span>
    <span class="p">(</span><span class="s2">&quot;Bad Company&quot;</span><span class="p">,</span> <span class="s2">&quot;Bad Company&quot;</span><span class="p">,</span> <span class="mi">1974</span><span class="p">,</span>   <span class="c1"># Second album list</span>
     <span class="p">[</span>
         <span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="s2">&quot;Can&#39;t Get Enough&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="mi">2</span><span class="p">,</span> <span class="s2">&quot;Rock Steady&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="mi">3</span><span class="p">,</span> <span class="s2">&quot;Ready for Love&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="mi">4</span><span class="p">,</span> <span class="s2">&quot;Don&#39;t Let Me Down&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="mi">5</span><span class="p">,</span> <span class="s2">&quot;Bad Company&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="mi">6</span><span class="p">,</span> <span class="s2">&quot;The Way I Choose&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="mi">7</span><span class="p">,</span> <span class="s2">&quot;Movin&#39; On&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="mi">8</span><span class="p">,</span> <span class="s2">&quot;Seagull&quot;</span><span class="p">),</span>
     <span class="p">]</span>
     <span class="p">),</span>
    <span class="p">(</span><span class="s2">&quot;Nightflight&quot;</span><span class="p">,</span> <span class="s2">&quot;Budgie&quot;</span><span class="p">,</span> <span class="mi">1981</span><span class="p">,</span>
     <span class="p">[</span>
         <span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="s2">&quot;I Turned to Stone&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="mi">2</span><span class="p">,</span> <span class="s2">&quot;Keeping a Rendezvous&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="mi">3</span><span class="p">,</span> <span class="s2">&quot;Reaper of the Glory&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="mi">4</span><span class="p">,</span> <span class="s2">&quot;She Used Me Up&quot;</span><span class="p">),</span>
     <span class="p">]</span>
     <span class="p">),</span>
    <span class="p">(</span><span class="s2">&quot;More Mayhem&quot;</span><span class="p">,</span> <span class="s2">&quot;Imelda May&quot;</span><span class="p">,</span> <span class="mi">2011</span><span class="p">,</span>
     <span class="p">[</span>
         <span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="s2">&quot;Pulling the Rug&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="mi">2</span><span class="p">,</span> <span class="s2">&quot;Psycho&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="mi">3</span><span class="p">,</span> <span class="s2">&quot;Mayhem&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="mi">4</span><span class="p">,</span> <span class="s2">&quot;Kentish Town Waltz&quot;</span><span class="p">),</span>
     <span class="p">]</span>
     <span class="p">),</span>
<span class="p">]</span>

<span class="n">album</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter a number between 1 and 4: &quot;</span><span class="p">)</span>
<span class="n">song</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter a number to choose the song: &quot;</span><span class="p">)</span>
<span class="n">output</span> <span class="o">=</span> <span class="n">albums</span><span class="p">[</span><span class="nb">int</span><span class="p">(</span><span class="n">album</span><span class="p">)</span><span class="o">-</span><span class="mi">1</span><span class="p">][</span><span class="mi">3</span><span class="p">][</span><span class="nb">int</span><span class="p">(</span><span class="n">song</span><span class="p">)</span><span class="o">-</span><span class="mi">1</span><span class="p">][</span><span class="mi">1</span><span class="p">]</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;Playing &quot;&#39;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">output</span><span class="p">)</span> <span class="o">+</span> <span class="s1">&#39;&quot;&#39;</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Playing &#34;Rock Steady&#34;
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">data</span> <span class="o">=</span> <span class="p">[</span><span class="mi">104</span><span class="p">,</span> <span class="mi">101</span><span class="p">,</span> <span class="mi">4</span><span class="p">,</span> <span class="mi">105</span><span class="p">,</span> <span class="mi">308</span><span class="p">,</span> <span class="mi">103</span><span class="p">,</span> <span class="mi">5</span><span class="p">,</span> <span class="mi">107</span><span class="p">,</span>
        <span class="mi">100</span><span class="p">,</span> <span class="mi">306</span><span class="p">,</span> <span class="mi">106</span><span class="p">,</span> <span class="mi">102</span><span class="p">,</span> <span class="mi">108</span><span class="p">]</span>    <span class="c1"># list of the different numerical values</span>
<span class="n">min_valid</span> <span class="o">=</span> <span class="mi">100</span>  <span class="c1"># minimum value</span>
<span class="n">max_valid</span> <span class="o">=</span> <span class="mi">200</span>  <span class="c1"># maximum value</span>

<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;These are the indexes and values from the list that do not fit the range of 100-200&quot;</span><span class="p">)</span>
<span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">reversed</span><span class="p">(</span><span class="nb">range</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="mi">13</span><span class="p">)):</span>
    <span class="k">if</span> <span class="p">(</span><span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">]</span> <span class="o">&gt;=</span> <span class="n">min_valid</span> <span class="ow">and</span> <span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">]</span> <span class="o">&lt;=</span> <span class="n">max_valid</span><span class="p">):</span>
        <span class="k">continue</span>
    <span class="k">else</span><span class="p">:</span>
        <span class="nb">print</span><span class="p">(</span><span class="n">i</span><span class="p">,</span> <span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">])</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>These are the indexes and values from the list that do not fit the range of 100-200
9 306
6 5
4 308
2 4
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

</div>
 
