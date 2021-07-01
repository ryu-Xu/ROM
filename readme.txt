This is the README file of the open source MATLAB toolbox: Reduced-order model (ROM) for linear elastic dynamics.
--------------------------------------------------------------------
The detailed contents of the folders in ROM are listed below:
--------------------------------------------------------------------
1. data
This folder includes the data of two cases and Each of them includes stiffness matrix, 
mass matrix, damping matrix, boundary conditions, and loads. Among them, the variable "kk" 
means the stiffness matrix, "mm" the mass matrix, "cc" the damping matrix  "bcdof" the 
boundary condition which is a vector whose length is the degree of freedom of the system. Its value is 0, 
except for the value of the constrained degree of freedom is 1. The variable "fd" is the load.
--------------------------------------------------------------------

2. subcode
This folder contains some code for imposing boundary conditions,  Newmark method
and its reduced-order model, and updating the POD basis function.
--------------------------------------------------------------------

3. main_calculation.m
This file could be used to quickly calculate the dynamics responses with ROM. In this case, 
the response is displacement. 
--------------------------------------------------------------------

4. model-FEM
The file includes two models,  plate_with_hole.m and bentpipe.m, 
which are written in FEM and can be run directly.
--------------------------------------------------------------------

5. model-IGA
The file includes two models,  plate_with_hole.m and bentpipe.m, 
which are written in IGA and can be run directly.
--------------------------------------------------------------------

*** If you have any comments or suggestions, please feel free to contact us! 
- Xiaofei Liu, 
- Hunan Univeristy,
- ryuxiaofei@hnu.edu.cn. 

*** If you feel it is helpful for your work, please cite our work.

