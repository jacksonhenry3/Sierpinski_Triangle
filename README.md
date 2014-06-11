<p>
	First, if you don't know about fractals, read about <a href = 'http://mathworld.wolfram.com/Fractal.html'>fractals</a>, they are freaking awesome.
	<br>
	The <a href = 'http://mathworld.wolfram.com/SierpinskiSieve.html'>Sierpinski Triangle</a> is a relatively simple fractal. And, inspired by <a href = 'http://books.google.com/books/about/Chaos_and_Fractals.html?id=jVpS_u0Lg4gC'>Chaos and Fractals</a> I wrote two programs to procedurally generate it. One is based on addressing each node while the other is based on a chaotic process. If both are carried out an infinite number of times they will generate the same figure.
</p>
<br>
<h3>By Randomness</h3>
<p>
	Start with three points (the three points of the largest triangle) and label them 1, 2 and 3. Then pick another point, anywhere. Role a 3 sided die (or a random number generator), if you role a three place a point 1/2 the distance from your initial point to point number three. Then, repeat that process for the new point. If you do this infinite times you will generate the Sierpinski gasket. Each frame of the .gif is a zoomed in image of the top triangle of the previous frame.
</p>
<br>
<h3>By Binary Address</h3>
<p>
	The Sierpinski triangle can be though of as a <a href = 'http://mathworld.wolfram.com/BinaryTree.html'>binary tree</a>. You can assign a unique id to each node in a binary tree in a very simple way. To get to a node all you do is start at the base of the tree and go either left or right at each subsequent node encountered. So if we list all the turn taken to get to a node we get a unique string which describes the path to that node. eg left right left left right. Because there is only two choices we call this a binary string, it is common to let 0 mean left and 1 mean right which would make our previous example in to 01001. using this process we address an arbitrarily large number of nodes and construct the Sierpinski triangle.
</p>
<hr>
Writen in python 2.7<br>Dependancies
<ul>
  <li>
    <a href = 'http://wiki.scipy.org/PyLab'>pylab</a>
  </li>
</ul>
