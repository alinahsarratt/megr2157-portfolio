# A7 – [Topic]



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





Next I went and changed the mesh size to coarse and reran it. 

<img width="1256" height="764" alt="image" src="https://github.com/user-attachments/assets/31e0093b-18f9-4168-9862-2faf2ffba239" />

These were the results I got:

<img width="1136" height="720" alt="image" src="https://github.com/user-attachments/assets/a7542009-8cef-4272-b43b-a753dd4147cf" />

<img width="887" height="622" alt="image" src="https://github.com/user-attachments/assets/d42b5fde-835e-4d10-bdea-fc18bcc06e3d" />



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



After I reran the FEA using the medium mesh and these were my results:


<img width="1278" height="777" alt="image" src="https://github.com/user-attachments/assets/3ecff46e-bea8-4915-9f54-80f3e5cebb91" />

<img width="1215" height="752" alt="image" src="https://github.com/user-attachments/assets/56b6e103-e6e3-4ba6-b4ac-e10788fcda2c" />



Since there was not a sign of stress convergence but displacement was approaching convergence I ran it with the fine mesh and these were the results. 

<img width="883" height="638" alt="image" src="https://github.com/user-attachments/assets/4acd22bc-531e-4360-998e-540341e30f12" />

<img width="1182" height="735" alt="image" src="https://github.com/user-attachments/assets/3ad983c0-ea40-4e8e-8a86-96d04983e7cb" />




Since it showed with the fine mesh that it was actually converging but not fully converged of 7%, it was specifcally 0.69% off of 7%, I wanted to make some last geometric changes so I kicked in out of the inner loop and went to the second outer loop where I would create my last design for the assignment. 

Outer loop 2

I wanted to thicken feature B a little bit to try to reduce the max stresses where feature A and feature B connect as shown in the image previously. I also wanted to make the bracket a lot lighter when considering is mass so I also removed some unneeded material. I essentially removed material that was all blue because there was little to no stress in these areas on the design. 

I ended up removing material from the sides of the bracket and I added more fillets to the front edge of my feature B, however I had to redo the constrains and add some to hold the front fillet edges in order to rerun the FEA it is depicted in the image below. 


<img width="1276" height="733" alt="image" src="https://github.com/user-attachments/assets/c2b12200-7235-47bb-b399-7889a7417775" />

After these geometric changes were complete I entered the final inner loop for this assignment because we had a maximum of three designs. 


Inner Loop 3 
First I ran the coarse mesh test and I got these as my results
<img width="1182" height="712" alt="image" src="https://github.com/user-attachments/assets/7afd3671-0d64-4145-9a07-be5e64709fe0" />

<img width="1277" height="779" alt="image" src="https://github.com/user-attachments/assets/d1f42dc7-7fe3-40f9-91af-b7320a89ec15" />



After my first test with the coarse mesh I reran the FEA simulation with the medium mesh to check the convergence. 

<img width="1207" height="768" alt="image" src="https://github.com/user-attachments/assets/6f9e4044-7b64-4fa9-a815-b987b0787faa" />

<img width="1213" height="740" alt="image" src="https://github.com/user-attachments/assets/d7d9800c-5d71-4373-becc-e2a8fa6c3eea" />



After I saw that these two results were not converging especially when analyzing the stress values so I ran the fine mesh FEA simulation study after. These were the results I got from that:

<img width="1274" height="708" alt="image" src="https://github.com/user-attachments/assets/6455e2b6-539e-4a74-a176-caf16511e90b" />

<img width="1176" height="732" alt="image" src="https://github.com/user-attachments/assets/b4489141-3adb-4ff6-b3cc-c4319bca0c04" />



After that I saw that the stresses were starting to converge but the displacement wasn't showing a converging trend however this was the end of my optimization process for this assignment. The mass also decreased from the original design. 

Below is a summary of a chart of my results from these simulations. 


<img width="484" height="120" alt="image" src="https://github.com/user-attachments/assets/c79b6af0-1193-4a89-af18-074f8216ec44" />

In each case, I noticed that my safety factor was below 1, meaning none of my designs could safely handle the load. In my original design, I constrained two separate bodies instead of having one continuous body, which most likely affected my maximum stress results. This could have caused higher stress in certain areas because of how I set up my constraints. I also noticed that most of the stress was around the connection between the cylinder and the arm, which showed me where my design needed the most improvement.


The LINK 
Next, I went through the exact same procedure with my link connection I made. I first made sure to set the constrains and forces on my link below. I made a bearing force inside the top link hole that will feel the 800inf load from feature A
 and decided to fix the bottom connection with a bearing fixture. 

 <img width="1253" height="748" alt="image" src="https://github.com/user-attachments/assets/3fe5e6cc-caa6-4fac-9579-935edfed67d9" />

When I went to run the first FEA with the coarse mesh it told me i was unconstrained and the link was rotating from side to side. So I constrained the sides and then ran the first FEA simulation. 

Inner loop 1 
These were my results with the first FEA test run with the coarse mesh 
<img width="1106" height="736" alt="image" src="https://github.com/user-attachments/assets/f0f150c2-f89e-4cd9-8fe9-4f4728aadf6b" />

<img width="1024" height="698" alt="image" src="https://github.com/user-attachments/assets/b315e18f-d492-4409-9f90-4b094551a7db" />



After I ran the medium mesh to see if my results started to converge these were my results

<img width="940" height="728" alt="image" src="https://github.com/user-attachments/assets/2c727fdf-d998-4aa8-8e9f-2670ce8cd1c9" />

<img width="1094" height="736" alt="image" src="https://github.com/user-attachments/assets/6c962145-9098-4b0a-bb79-2937c6f2c01d" />



Since there was an 18.9% increase in stress and a 5.45% increase in displacement there was not a 7% convergence in each category. So I ran one more FEA with the fine mesh. 

<img width="1174" height="721" alt="image" src="https://github.com/user-attachments/assets/ac3f9a71-1340-433f-b44e-daa60fdffffc" />

<img width="1101" height="700" alt="image" src="https://github.com/user-attachments/assets/c6174882-f900-45f0-8857-84ff2aedb6d0" />



Even though the displacement on the fine mesh increased by only 0.98% the stress increased by 42%, but I reached my maximum of three interloop trials so I kicked it to the outer loop to make geometric changes. 

Outer loop 1 
I noticed that on some of the first FEA runs that my link fell below the yield strength so I know going into it I wanted to make it more sturdy so I decided to increase the thickness of my link. I made the thickness increase by 0.50 inches. 

<img width="578" height="453" alt="image" src="https://github.com/user-attachments/assets/7ee64d21-bfd6-4548-806b-e0d3c4ddaee2" />

After I went back into the second inner loop to run the FEA simulation with the different meshes

Inner Loop 2 
I first ran my new design with the coarse mesh and these were the results 
<img width="2320" height="1800" alt="image" src="https://github.com/user-attachments/assets/37f5554d-5d79-4911-a0df-02070d803674" />

<img width="2370" height="1802" alt="image" src="https://github.com/user-attachments/assets/22fe7f7d-8387-46ca-9a5c-4504ddc96753" />



After I went ahead and ran the results with medium mesh to test the convergence, these were the results
<img width="2415" height="1777" alt="image" src="https://github.com/user-attachments/assets/fd5162a4-b2e5-4558-a5d1-e8ac4af0217f" />

<img width="2515" height="1892" alt="image" src="https://github.com/user-attachments/assets/d9e7bcc9-c09a-4a69-b525-491339f1810a" />


The two meshes did not have a convergence of 7% in the displacement or max stress category so I went and ran it with the fine mesh. These were the results of this run. 

<img width="2392" height="1832" alt="image" src="https://github.com/user-attachments/assets/960f95c1-d7bb-41ec-819a-378cc1595c01" />

<img width="2355" height="1832" alt="image" src="https://github.com/user-attachments/assets/64398d15-4d8d-465f-bd86-1747cf93c5e8" />



While the displacement from coarse to fine only had a 7.8% convergence the max stress first had a convergence of 12% then had another at 31.1%. Since this was my third run in the inner loop I kicked it back to the outer loop for one last geometric change. 

Outer loop 3

I decided to add some fillets to the edges that were receiving max stress at the top and removed some material from the middle to try to make it lighter it is depicted below. 

<img width="2775" height="1895" alt="image" src="https://github.com/user-attachments/assets/acae9d46-71ec-4c10-9d0f-10cc9eba1308" />

After I entered my last inner loop with my third design. 

Inner Loop 3 
First I ran the FEA under the coarse mesh. These were my results
<img width="2048" height="1491" alt="image" src="https://github.com/user-attachments/assets/a7d1eb41-3a76-4db6-8646-e83f6d680103" />

<img width="2048" height="1576" alt="image" src="https://github.com/user-attachments/assets/d789923d-ba20-4191-91d6-e636152996a2" />

After I ran the FEA with my medium mesh. Below are the results

<img width="2410" height="1845" alt="image" src="https://github.com/user-attachments/assets/057f675e-b911-4280-babf-526edc1d0bf5" />

<img width="2715" height="1815" alt="image" src="https://github.com/user-attachments/assets/83151954-fc03-4ac8-9435-a7aa7e3ef7be" />


After this I got a convergence of stress of 7.44% so almost 7% flat, then I got a displacement convergence of 0.49%. But because it was just above 7% I went ahead and ran the last FEA with the fine mesh. Below are the results I got. 

<img width="2420" height="1762" alt="image" src="https://github.com/user-attachments/assets/77786494-c2bc-4822-ace2-74e188700d0d" />

The medium to fine did not have a convergence close to 7% with the stresses it decreased by 21.8%, then the displacenment only changed by 0.92%. However since this was my third design run this concluded the assignment. 

Below is a chart that summarized my designs for the link. 


<img width="2043" height="770" alt="image" src="https://github.com/user-attachments/assets/6a633b78-dad1-41e5-896f-5e54e19a95a9" />

After completing the FEA simulations for all three designs, I was able to compare how each geometric change affected the stress, displacement, and overall mass of the link. Design 1 had the lowest mass, but it also had the highest stress and displacement, making it the least effective design. For Design 2, I increased the thickness, which significantly reduced both stress and displacement, but also increased the mass. For Design 3, I added two holes and fillets to try to reduce the weight while maintaining strength. This lowered the mass compared to Design 2, but the stress and displacement increased slightly. Overall, I think Design 3 provided a good balance between strength and weight since it maintained a factor of safety above 3 while using less material. However, the stress results did not fully converge, so I would need to continue to test the mesh and refine it to really see if these results are true. 






Below are links to my parts 


<a href="https://raw.githubusercontent.com/alinahsarratt/megr2157-portfolio/main/A6part.SLDPRT" download>
  Download A6 Part (.SLDPRT)
</a>





<a href="https://raw.githubusercontent.com/alinahsarratt/megr2157-portfolio/main/Link%20part%20A6.SLDPRT" download>
  Download Link Part (.SLDPRT)
</a>















## Communicate

Throughout this assignment, I learned that even the smallest changes in my FEA setup can really mess with my results. One thing I noticed was how much the mesh size affected my maximum stress. When I switched from a coarse mesh to a fine mesh, the number of elements went up, meaning SolidWorks had to do way more calculations and took longer to solve. I also realized that just because I used a finer mesh doesn't automatically mean my results are right, especially if I messed up my constraints.

Another thing I learned was that changing my design doesn't always mean it's going to perform better. When I added fillets and changed the shape of my bracket, I thought my stress would go down, but it actually went up. My third design ended up being the lightest and had the least amount of displacement, but somehow had the highest maximum stress. This showed me that fixing one problem in my design can sometimes create another one. In total with fixing my mistakes this assignment took me about 6 hours.



