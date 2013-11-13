TenVis (Tensor Visualization tool)
====== 
TenVis can help you analyze tensors or 3x3 matrices using ellipsoids.
Different color mappings are given.
This project was created as part of my Computer Science thesis work and is mostly aimed on Diffusion Tensor Imaging visualization.

Version
-

0.1

Tech
-----------

TenVis uses javascript, HTML5, WebGL and the amazing [Three.js] library. 

Installation
--------------

No installation needed, it's all javascript! Just click the `TenVis.html` file and it works automagically. Things should work on any WebGL enabled browser, which means no IE support for the time being.

How to use
-

Drag and drop a file containing:

  - Tensors coordinates in space
  - Tensors eigenvectors ( for orientation )
  - Tensors eigenvalues

Example:
-
 
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

Snapshots
-
![alt text](https://dl.dropboxusercontent.com/u/1056837/TenVis/imgs/5.PNG "Brain1")
![alt text](https://dl.dropboxusercontent.com/u/1056837/TenVis/imgs/6.PNG "Brain2")
![alt text](https://dl.dropboxusercontent.com/u/1056837/TenVis/imgs/compositecolor-Karcher.PNG "3 tensors interpolation")
![alt text](https://dl.dropboxusercontent.com/u/1056837/TenVis/imgs/detLpY.PNG "Brain DTI slice 1")
![alt text](https://dl.dropboxusercontent.com/u/1056837/TenVis/imgs/LPSGeoAVERA.PNG "Brain DTI slice 2")

Acknowledgements
-
I would like to thank Professor [Bruno Iannazzo] from UNIPG who helped testing and debugging TenVis, and [Gabriele di Bari] whose WebGL expertise 
saved me from some weird situations.

License
-

MIT


  [Three.js]: http://threejs.org/
  [Gabriele di Bari]:https://github.com/Gabriele91
  [Bruno Iannazzo]:http://poisson.phc.unipi.it/~maxreen/bruno/   
