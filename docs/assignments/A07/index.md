# A7 – [Topic]

## Objective

### Objective

This week we were tasked with using Finite Element Analysis (FEA) in SolidWorks to analyze and improve our bracket design from the previous assignments. We were supposed to apply the correct material, forces, and fixtures to our model and run a static study to determine the stress, displacement, and factor of safety. We also had to refine our mesh to check that our results were accurate. After analyzing our original design, we were tasked with making changes to the bracket's geometry to improve its strength and stiffness while reducing its mass. We had to analyze at least three different designs and compare the results to determine which design performed the best.

## Analyze
At first I had to make sure all of my parameters were right, there essentially wasn't a lot of analyzing to do in this assignment until the test were actually ran. I started first by making sure the correct material was assigned to my model, I applied A36 steel to my model as depicted in the screenshot below. 





After that I had to decide what I wanted my constrains to be. 


## Decide

At first I input fixed geometry to the inner T-shaped opening. I assumed that although the bracket has sufficient clearance to be installed onto the T-beam with a sliding fit, it remains stationary during operation. This fixture represents a simplified rigid connection between the bracket and the supporting beam.

<img width="1267" height="742" alt="image" src="https://github.com/user-attachments/assets/5e0c12e2-c96f-49ac-81ad-74f9f65666e1" />

After I fixed the geometry I input the load the distributed strap load of 800ibf on my feature A. At first this load went around the entire circle instead of just acting on the top half as depicted below. 

<img width="558" height="365" alt="image" src="https://github.com/user-attachments/assets/dd55df23-3d77-4704-a3e3-5ed69d4d26cb" />

I realized I need to add a split plan so the load would only be placed on the top portion of the feature that comes directly in contact with the strap. 

<img width="1266" height="735" alt="image" src="https://github.com/user-attachments/assets/01726190-51dc-4771-a37b-b6f39fa7fb90" />


After I needed to input the mesh on my design, for my first study I decided to run the it using the default mesh. 
<img width="1164" height="722" alt="image" src="https://github.com/user-attachments/assets/05f931e3-da2a-421b-88cf-be7015fc0580" />


## Communicate

