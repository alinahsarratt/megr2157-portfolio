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

When I went to run the study after it informed me that I had under constrained bodies so I had to fix those in order to proceed. After I saw that my feature A could slide up and down so I constrained it to feature b in the image below with fixed geometry. 

<img width="362" height="336" alt="image" src="https://github.com/user-attachments/assets/247fabc2-3628-4855-93d8-a1401840d929" />

These were the result of my first FEA study run with the medium mesh 

<img width="1241" height="715" alt="image" src="https://github.com/user-attachments/assets/6a0b65b5-5efe-48a9-9ce3-f9d9e21e3ab4" />



<img width="1242" height="727" alt="image" src="https://github.com/user-attachments/assets/e8626e2d-011a-44cd-a850-5c3d9a5315e8" />


<img width="1252" height="728" alt="image" src="https://github.com/user-attachments/assets/2ac12b34-7d5a-48bc-9c2e-2b0057b03818" />


Next I went and changed the mesh size to coarse and reran it. 

<img width="1256" height="764" alt="image" src="https://github.com/user-attachments/assets/31e0093b-18f9-4168-9862-2faf2ffba239" />

These were the results I got:

<img width="1136" height="720" alt="image" src="https://github.com/user-attachments/assets/a7542009-8cef-4272-b43b-a753dd4147cf" />

<img width="887" height="622" alt="image" src="https://github.com/user-attachments/assets/d42b5fde-835e-4d10-bdea-fc18bcc06e3d" />

<img width="1275" height="746" alt="image" src="https://github.com/user-attachments/assets/3a64e740-0c48-460b-8060-9f05d9d7bfee" />







## Communicate

