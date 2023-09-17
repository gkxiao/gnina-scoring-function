<h2>Install gninatorch</h2>
<p>code:https://github.com/RMeli/gnina-torch</p>
<p>manual: https://gnina-torch.readthedocs.io/en/latest/ </p>
<h2>Run in score_only mode</h2>
<p>1. create a index file (score.index) as following:</p>
<pre line="1">
receptor_1.pdb ligand_1.sdf
receptor_1.pdb ligand_2.sdf
receptor_1.pdb ligand_3.sdf
</pre>
<p>2.rescore</p>
<pre line="1">
python -m gninatorch.gnina \
    score.index \
    --batch_size 200 \
    --cnn default
</pre>
<h2>Case study</h2>
<h3>DUD-E EGFR</h3>
<p>Blog: http://blog.molcalx.com.cn/2023/08/31/boosting-virtual-screening-enrichments-with-data-fusion.html</p>
<img style="text-align:center;" src='http://blog.molcalx.com.cn/wp-content/uploads/2023/08/2023083111293864.png' alt="CNN score use to boost the docking enrichment." width="500" height="500">
<h3>DUDE HIVPR</h3>
<p>Blog: http://blog.molcalx.com.cn/2023/09/13/beware-of-the-benchmarking-test.html</p>
<img style="text-align:center;" src='http://blog.molcalx.com.cn/wp-content/uploads/2023/09/2023091418453321.png' alt='Docking Virtual screening performane with different protein structure'  width="500" height="390">
<h2>Reference</h2>
<ol>
   <li>Sunseri, J.; Koes, D. R. Virtual Screening with Gnina 1.0. Molecules 2021, 26 (23), 7369. https://doi.org/10.3390/molecules26237369.</li>
   <li>https://github.com/RMeli/gnina-torch</li>
</ol>
