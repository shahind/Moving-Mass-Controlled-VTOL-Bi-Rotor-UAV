# MMC_VTOL_BI-ROTOR_UAV | 6DOF Simulink Model
This folder contains the 6DOF simulink model of a Moving Mass Controlled VTOL Bi-Rotor UAV which is developed in the following paper.


This repository contains the 6DoF MATLAB Symulink model, CAD files of prototype and 1DoF testbed of a novel moving mass controlled bi-rotor VTOL UAV,
for more information about the UAV and mathematical modeling, please read the paper:
https://www.sciencedirect.com/science/article/abs/pii/S1270963820309202?dgcid=author

please cite the project as :

**S. Darvishpoor, J. Roshanian, and M. Tayefi, “A novel concept of VTOL bi-rotor UAV based on moving mass control,” Aerospace Science and Technology, vol. 107, p. 106238, Dec. 2020, doi: 10.1016/j.ast.2020.106238.**

https://user-images.githubusercontent.com/10776307/134034052-e9379b01-2e93-4758-a07f-4f362ee92938.mp4

**note:  
You can change the initial values from init callback (InitFcn) of the "MMC Bi-Rotor UAV" block:  
```
%Initial Parameters
M_m          %MM mass
M_b          %Body mass
I_b_bar      %Inertia of the body around its CG
I_m_1_bar =  %Inertia of the MM1 around their CG
I_m_2_bar =  %Inertia of the MM2 around their CG
I_m_3_bar =  %Inertia of the MM3 around their CG
I_m_4_bar =  %Inertia of the MM4 around their CG
M            %Total mass
mu           %mass ratio of the m to M
Z_b_0        %z_cg body in R0
Z_m_0        %z_cg MM in R0
Z_cg_0       %z_cg total in R0
l            %max dicplacement of the moving mass
b            %Propeller thrust constant
d            %Propeller drag constant
g            %Gravity
init_X       %Initial position in inertial axes
init_V       %Initial velocity in body axes (u v w)
init_O       %Initial Euler oriantation (phi theta say)
init_R       %Initial body rotation rates (p q r)
```
In order to access callbacks: right click on the block and select propertise then choose Callbacks tab and find InitFcn.
