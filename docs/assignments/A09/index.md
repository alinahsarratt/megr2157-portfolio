# A9 – Pulleys

## Objective
For this project, we were tasked with solving for multiple values to help us select a suitable belt size for our designed pulley system. We also had to determine the forces acting on the tight and loose sides of the belt, calculate the minimum shaft diameter, and select a suitable bearing material using  After completing these calculations, we would use SolidWorks to design a frame that supports our pulley system. 

## Analyze
For this part of the project, I started by choosing the design parameters I wanted to use for my pulley system. I decided to use two steel pulleys with a diameter of 3 inches and a center distance of 5 inches. I also chose a rotational speed of 2000 rpm and a static belt tension of 6 lbf since both were within the requirements of the assignment.

After choosing my values, I created a free-body diagram to show the tight-side and loose-side forces acting on the pulley. From there, I used the equations from our lecture to calculate the limiting forces before slipping occurs. I found that the tight-side force was approximately 10.42 lbf and the loose-side force was 1.58 lbf, using a coefficient of friction of 0.6.

Next, I used the normal stress equation and the required safety factor of 3 to calculate the minimum cross-sectional area of the belt. This gave me an area of 0.0664 in² and a minimum belt diameter of approximately 0.291 inches. I also calculated the approximate belt length to be 19.42 inches based on the pulley diameter and center distance. After I did these calculations I was able to choose a belt this can be found in the Decide section. 

After these calculations I moved on to conducting and analyzing a second part of calculations I began to try to find the minimum diameter of the shaft. For this part, I used Machinery's Handbook (32nd edition) to find the yield strength of 1060 hardened steel. I decided to use steel that was quenched and tempered at 400°C since the assignment asked for hardened 1060 steel as the material. It had a listed strength of 113,000 psi. After finding this value, I plugged it into my minimum shaft diameter equation along with my previously calculated torque of 13.26 lbf·in and safety factor of 3. From these calculations, I found that my minimum shaft diameter was approximately 0.146 inches.Below are my calculations in how I did this.

After it was time to analyze the PV rating so I could select a journal bearing from the machinery's handbook. I started by using the forces I had previously calculated, which were 10.42 lbf and 1.58 lbf. Adding these together gave me a total load of 12 lbf. Since I was using two bearings to support the shaft, I divided the load equally between them, giving me a reaction force of 6 lbf per bearing.

Next, I calculated the bearing pressure using the load, shaft diameter, and bearing length. I decided to use a shaft diameter of 0.25 inches and a bearing length of 0.50 inches. Using these values, I calculated a bearing pressure of 48 psi.

After finding the pressure, I moved on to calculating the surface velocity of the shaft. For this calculation, I used the shaft diameter of 0.25 inches and a rotational speed of 2,000 RPM. This gave me a velocity of 130.90 ft/min.

Finally, I multiplied the pressure and velocity together to find the PV rating. My work for this is down below:



Then I decided on a journal bearing which can be found in the Decision section. 



## Decide
My first decesion was to choose a belt based on my minimum diameter I calculated in the above section, since it was 0.291 inches I chose the 5/16 inch diameter 	
Polyurethane Rubber belt. This had a diameter of 0.3125 inches which is slightly greater than my minimum diameter allowing it to be suitable for the design. Below is a link to the website I used to choose this belt. 

https://www.mcmaster.com/59725K733

The second decision I made was based on the Table 4 in Machinery's Handbook page 2442, I selected a journal bearing for my design. I needed to check not only the max load capacity but also the surface speed and pv limit on each bearing material. I was considering porous iron because it had a pv limit way above my calculated value at 50,000 psi ft/min and it had a max load capacity of 8000 psi. However it had a slow surface speed at 800 fpm. So I decided to keep the same pv limit value and look at what porous bronze had and it had a max load capcity of 4500 psi this was above calculated 48 psi and it also had a higher surface speed of 1500fpm. I then decided to design my journal bearing out of this material. 

Next it was time to start designing my frame but since I had my bearing material I needed its outside diameter, since I knew the inner nominal matched the 0.25 inch diamter on the shaft, so I did a calculation. I assumed a thickness of 0.0625 for the wall thickness, this would left be with an outer diamter of 0.375 as you can see in my calculations below. 

However I had to make sure that the design could actually support this wall thickness in terms of bearing pressure and how it compares to the load capacity of the material. So I plugged it into the bearing pressure equation and got the answer to that below. It was way below the material's loading capacity meaning the design could sustain those dimensions. Then I moved on to creating my solid model based on these dimensions. 

I first began with this simple sketch I was going to extrude. 
<img width="2902" height="1912" alt="image" src="https://github.com/user-attachments/assets/b689fa40-0280-4693-aa3f-546884b8970e" />

I then added dimensions I previously had or solved for. I had just solved for the outside diameter of the bearings which is why the two holes have a diameter of 0.375 and then I used the center distance of 5.00 that I previously used to find my belt length as well. 
<img width="2790" height="1867" alt="image" src="https://github.com/user-attachments/assets/73bb0be3-2cf0-41da-9a92-64bf748e6cd3" />

After I decided to extrude out my sketch, I knew my bearing lengths were 0.50 inches in length so I wanted to give a little extra room on each side and extruded it out to 0.75 inches. 
<img width="3007" height="1712" alt="image" src="https://github.com/user-attachments/assets/4dda7af2-d41e-47e8-b4de-2ae388684c60" />

Below is the link to download my frame:




## Communicate
Throughout this assignment, I learned how important it is to use engineering calculations to support the decisions I make when designing something. I spent approximately 5 hours working on this project, and a lot of that time went toward figuring out the journal bearing calculations, selecting a suitable material, and creating my frame in SolidWorks. One of the biggest things I learned was how the pressure, surface velocity, and PV rating all play a role in determining whether a bearing material is suitable for a design. I also learned how important it is to understand the dimensions of each component before starting my CAD model. At first, I was a little confused about how the bearing dimensions related to my frame, but after working through everything, I was able to understand how the bearing's outside diameter determines the size of the holes in my frame.
