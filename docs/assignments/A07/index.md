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

Inner loop 1

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

After I reran an got my results from the fine mesh. I then realized my results were not converging at all they were increasing, so I analyzed on the feature where the max stress was occurring so I could see what was potentially happening. On each test it was occurring here. 

<img width="330" height="329" alt="image" src="https://github.com/user-attachments/assets/c7ce54f0-c458-4fee-8ed4-04ed8ce00a12" />

I realized I might be able to take out the sharp edge and make it a fillet to help with the loading. So I took it out of the inner loop 1 now and kicked it out to the outer loop to fix its geometry. Since I had reached max inner loop tests I was able to kick it out. 


Outer Loop 1

For my geometric changes of my first outer loop I decided to make a fillet on the features of B and A. on the straight vertical edges along feature B I made a fillet of 0.10 inches. Then I changed the back edge on feature A to a fillet of 0.05 inches. 
<img width="1250" height="730" alt="image" src="https://github.com/user-attachments/assets/9ce92d49-0e0a-47a4-b368-90f82335a6ec" />

After this geometry change was applied I went back into the inner loop to run the FEA study again with the different mesh sizes. 

Inner Loop 2 
I first ran my new part with coarse mesh. 

<img width="1270" height="761" alt="image" src="https://github.com/user-attachments/assets/1d89a50b-b565-486d-b2dd-028c79415929" />

These were the results: 

First I noticed on the stress test that the maximum stress decreased in the area it was before it doesn't reach as high of a stress value. 
<img width="856" height="637" alt="image" src="https://github.com/user-attachments/assets/eece6d3b-b568-4beb-ab2a-37068d50edef" />

The next images were each test result:

<img width="1236" height="734" alt="image" src="https://github.com/user-attachments/assets/1fe9aa7f-4993-4b66-b187-8bdc4c958ee5" />

<img width="1271" height="758" alt="image" src="https://github.com/user-attachments/assets/1fb17b2e-f689-4e19-81ce-aee7ef647e0a" />

<img width="1268" height="755" alt="image" src="https://github.com/user-attachments/assets/1e9b0750-e690-4dc4-8a11-62ce9019a687" />

After I reran the FEA using the medium mesh and these were my results:

<img width="1278" height="777" alt="image" src="https://github.com/user-attachments/assets/3ecff46e-bea8-4915-9f54-80f3e5cebb91" />

<img width="1215" height="752" alt="image" src="https://github.com/user-attachments/assets/56b6e103-e6e3-4ba6-b4ac-e10788fcda2c" />

<img width="1274" height="766" alt="image" src="https://github.com/user-attachments/assets/70c01505-eddb-4e5f-8820-af9d9a815824" />

Since there was not a sign of stress convergence but displacement was approaching convergence I ran it with the fine mesh and these were the results. 

<img width="883" height="638" alt="image" src="https://github.com/user-attachments/assets/4acd22bc-531e-4360-998e-540341e30f12" />

<img width="1182" height="735" alt="image" src="https://github.com/user-attachments/assets/3ad983c0-ea40-4e8e-8a86-96d04983e7cb" />

<img width="1195" height="729" alt="image" src="https://github.com/user-attachments/assets/bb6191eb-1fe8-4431-af83-c9a439d90d33" />


Since it showed with the fine mesh that it was actually converging but not fully converged of 7%, it was specifcally 0.69% off of 7%, I wanted to make some last geometric changes so I kicked in out of the inner loop and went to the second outer loop where I would create my last design for the assignment. 

Outer loop 2
I wanted to thicken feature B a little bit to try to reduce the max stresses where feature A and feature B connect as shown in the image previously. I also wanted to make the bracket a lot lighter when considering is mass so I also removed some unneeded material. I essentially removed material that was all blue because there was little to no stress in these areas on the design. 



















## Communicate

