This is the README file of the open source MATLAB toolbox: Reduced-order model (ROM) for linear elastic dynamics.
--------------------------------------------------------------------

Please first go to the folder cfiles to run the script compile.m, because some C codes are used in this toolbox to improve the efficiency of the procedure. So a C/C++ compiler is required. 
!!! If you couldn't compile it successfully, don't worry, we can take a detour!

First of all, add the KPOD folder to the path. Right-click on the KPOD folder and select "Add to Path" -> "Selected Folders and Subfolders". 

The detailed contents of the folders in ROM are listed below:
------------------------------------------------------------
1. cfiles
This folder includes the C codes for calculating the two and three dimensional basis functions and derivatives, which will be widely used in other functions. Please run the compile.m file first to generate the mex files which provide an interface between MATLAB and C/C++ codes.

IMPORTANT: If the C codes can't be compiled successfully, please use the functions provided in "nurbs-1.3.12" for calculating derivatives rather than the C codes. The detailed instructions can be found in the function "nurbs_derivatives", which is located in the folder "functions".

------------------------------------------------------------
2. elasticity
This folder includes two examples in the paper.

------------------------------------------------------------
3. functions
The main functions of NLIGA are given in this folder, including the mesh generation, integration, connectivity, constitutive relations, visualization mesh generation, and plot functions.

------------------------------------------------------------
5. geometries
The plate_with_hole and 3D bent pipe geometries are provided in the folder.

------------------------------------------------------------
8. nurbs-1.3.12
This is an excellent opensource toolbox for the creation, manipulation of NURBS. More information can be found on the website, https://octave.sourceforge.io/nurbs/index.html 
The representation of the NURBS and p, k refinement algorithms used in NLIGA are employed from this toolbox.

------------------------------------------------------------
6. subcode
This folder includes some functions of POD and Newmark algorithm.

------------------------------------------------------------
Thanks:
The completion of this work needs to thank Du Xiaoxiao for his help and his work: NLIGA. The IGA modeling and drawing in this article are based on his work.
Du, Xiaoxiao, Gang Zhao, Wei Wang, Mayi Guo, Ran Zhang, and Jiaming Yang. "NLIGA: a MATLAB framework for nonlinear isogeometric analysis." Computer Aided Geometric Design 80 (2020): 101869.
Xiaoxiao Du (Beihang Univeristy, duxxhf@gmail.com or duxiaoxiao@buaa.edu.cn. )
------------------------------------------------------------

Xiaofei Liu
Hunan University
ryuxiaofei@hnu.edu.cn





