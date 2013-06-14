TenVis
======
A tensor viewer.  
TenVis can help you analyze 3x3 matrices properties using ellipsoids.  
Different color mappings are given.

Version
-

0.1

Tech
-----------

TenVis uses WebGL and mostly the amazing [Three.js] library. 

Installation
--------------

No installation needed. Just click the `TenVis.html` file and it works automagically. Things should work on any WebGL enabled browser, wich means no IE support for the time being.

How to use
===

Drag and drop a file containing:

  - Tensors coordinates in space
  - Tensors eigenvectors ( for orientation )
  - Tensors eigenvalues

Example:  
57,94,23  
1,0,0  
0,1,0  
0,0,1  
10,3,3  
77,94,23  
0,1,0  
0,0,1  
1,0,0  
10,3,3  
97,94,23  
0,1,0  
1,0,0  
0,0,1  
10,3,3   
  

A .txt file containing the above data (15 text lines + 1 white line in this case) should display 3 ellipsoids aligned with the x, y and z axis.  
For each tensor, the first line contains the coordinates. The next three lines contain the rotation matrix   
 XX, XY, XZ  
 YX, YY, YZ  
 ZX, ZY, ZZ  
while the last line contains the eigenvalues of the matrix.

Acknowledgements
-
I would like to thank Professor [Bruno Iannazzo] from UNIPG who helped designing and testing TenVis, and [Gabriele di Bari] whose WebGL expertise 
saved me from some weird situations.

License
-

MIT

*Free Software, Fuck Yeah!*
  [Three.js]: http://threejs.org/
  [Gabriele di Bari]:https://github.com/Gabriele91
  [Bruno Iannazzo]:http://poisson.phc.unipi.it/~maxreen/bruno/   