IC 74LS85 is a four-bit magnitude comparator that compares Binary Numbers. It checks whether a 4-bit binary number A<sub>3 </sub>A<sub>2 </sub>A<sub>1 </sub>A<sub>0</sub> is greater than, less than or equal to another 4-bit number B<sub>3 </sub>B<sub>2 </sub>B<sub>1 </sub>B<sub>0</sub>. The IC has two sets of four bit inputs to be compared and also has three cascade inputs A &gt; B, A = B and A &lt; B and produces three outputs A &gt; B, A = B and A &lt; B. These devices are fully expandable to any number of bits without external gates.<br/>

<b>Diagram:</b><br/>
<center>
<img src="./images/image001.png">
<br/><br/>
<img src="./images/image002.png">
<br/><br/>
<img src="./images/image003.jpg">
<br/><br/>
<br/>
<img src="./images/image004.png">
<br/><br/>
</center>

#### Numerical:
<p>The Comparator compare the number bit by bit from MSB to LSB.<br />
The function table of 4-bit comparator is:</p>

<table border="1" cellspacing="0" class="MsoTableGrid">
	<thead>
		<tr>
			<th colspan="4" rowspan="1" scope="col">Comparing Input</th>
			<th colspan="3" rowspan="1" scope="col">Output</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<th>A<sub>3</sub>, B<sub>3</sub></th>
			<th>A<sub>2</sub>, B<sub>2</sub></th>
			<th>A<sub>1</sub>, B<sub>1</sub></th>
			<th>A<sub>0</sub>, B<sub>0</sub></th>
			<th>A &gt; B</th>
			<th>A = B</th>
			<th>A &lt; B</th>
		</tr>
		<tr>
			<td>A<sub>3</sub> &gt; B<sub>3</sub></td>
			<td>X</td>
			<td>X</td>
			<td>X</td>
			<td>1</td>
			<td>0</td>
			<td>0</td>
		</tr>
		<tr>
			<td>A<sub>3</sub> &lt; B<sub>3</sub></td>
			<td>X</td>
			<td>X</td>
			<td>X</td>
			<td>0</td>
			<td>0</td>
			<td>1</td>
		</tr>
		<tr>
			<td>A<sub>3</sub> = B<sub>3</sub></td>
			<td>A<sub>2</sub> &gt; B<sub>2</sub></td>
			<td>X</td>
			<td>X</td>
			<td>1</td>
			<td>0</td>
			<td>0</td>
		</tr>
		<tr>
			<td>A<sub>3</sub> = B<sub>3</sub></td>
			<td>A<sub>2</sub> &lt; B<sub>2</sub></td>
			<td>X</td>
			<td>X</td>
			<td>0</td>
			<td>0</td>
			<td>1</td>
		</tr>
		<tr>
			<td>A<sub>3</sub> = B<sub>3</sub></td>
			<td>A<sub>2</sub> = B<sub>2</sub></td>
			<td>A<sub>1</sub> &gt; B<sub>1</sub></td>
			<td>X</td>
			<td>1</td>
			<td>0</td>
			<td>0</td>
		</tr>
		<tr>
			<td>A<sub>3</sub> = B<sub>3</sub></td>
			<td>A<sub>2</sub> = B<sub>2</sub></td>
			<td>A<sub>1</sub> &lt; B<sub>1</sub></td>
			<td>X</td>
			<td>0</td>
			<td>0</td>
			<td>1</td>
		</tr>
		<tr>
			<td>A<sub>3</sub> = B<sub>3</sub></td>
			<td>A<sub>2</sub> = B<sub>2</sub></td>
			<td>A<sub>1</sub> = B<sub>1</sub></td>
			<td>A<sub>0</sub> &gt; B<sub>0</sub></td>
			<td>1</td>
			<td>0</td>
			<td>0</td>
		</tr>
		<tr>
			<td>A<sub>3</sub> = B<sub>3</sub></td>
			<td>A<sub>2</sub> = B<sub>2</sub></td>
			<td>A<sub>1</sub> = B<sub>1</sub></td>
			<td>A<sub>0</sub> &lt; B<sub>0</sub></td>
			<td>0</td>
			<td>0</td>
			<td>1</td>
		</tr>
		<tr>
			<td>A<sub>3</sub> = B<sub>3</sub></td>
			<td>A<sub>2</sub> = B<sub>2</sub></td>
			<td>A<sub>1</sub> = B<sub>1</sub></td>
			<td>A<sub>0</sub> = B<sub>0</sub></td>
			<td>0</td>
			<td>1</td>
			<td>0</td>
		</tr>
	</tbody>
</table>

<br />
<br />

Example:<br />
<ol>
<li>
A = 0, B = 0<br />
&nbsp;&nbsp;&nbsp;A = 0 (Decimal)&nbsp;&nbsp;&nbsp; 0000 (Binary)<br />
&nbsp;&nbsp;&nbsp;B = 0 (Decimal)&nbsp;&nbsp;&nbsp; 0000 (Binary)<br />
  Ans:<br />
  	<table border="1" cellspacing="0" class="MsoTableGrid">
		<tr>
			<th>A&gt;B</th>
			<th>A=B</th>
			<th>A&lt;B</th>
		</tr>
		<tr>
			<td>Low</td>
			<td>High</td>
			<td>Low</td>
		</tr>
	</table>
	<br />
	<br />
</li>
<li>
A = 0, B = 2<br />
&nbsp;&nbsp;&nbsp;A = 0 (Decimal)&nbsp;&nbsp;&nbsp; 0000 (Binary)<br />
&nbsp;&nbsp;&nbsp;B = 2 (Decimal)&nbsp;&nbsp;&nbsp; 0010 (Binary)<br />
  Ans:<br />
  	<table border="1" cellspacing="0" class="MsoTableGrid">
		<tr>
			<th>A&gt;B</th>
			<th>A=B</th>
			<th>A&lt;B</th>
		</tr>
		<tr>
			<td>Low</td>
			<td>Low</td>
			<td>High</td>
		</tr>
	</table>
	<br />
	<br />
</li>
<li>
A = 4, B = 2<br />
&nbsp;&nbsp;&nbsp;A = 4 (Decimal)&nbsp;&nbsp;&nbsp; 0100 (Binary)<br />
&nbsp;&nbsp;&nbsp;B = 2 (Decimal)&nbsp;&nbsp;&nbsp; 0010 (Binary)<br />
  Ans:<br />
  	<table border="1" cellspacing="0" class="MsoTableGrid">
		<tr>
			<th>A&gt;B</th>
			<th>A=B</th>
			<th>A&lt;B</th>
		</tr>
		<tr>
			<td>High</td>
			<td>Low</td>
			<td>Low</td>
		</tr>
	</table>
</li>
</ol><script type="text/javascript" id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"> </script>