# A4 – [Topic]

## Objective
This week we were tasked to design a motor mount that attaches to a wall and holds a Brushed 24V DC Gear Motor 3.6Kg.cm/46RPM w/ 99.5:1 Planetary Gearbox. We had the decision to choose what material to use out of ABS,PLA or PETG. We had to design for both yield strength and a maximum deflection of 0.30mm. We were to neglect the weight of the motor, take into account a safety factor of 3 and have a received force on the shaft of the motor of 300N. 







## Analyze
The first steps I took was analyzing the materials I has to choose from. I researched each of the materials parameters on Mat web. I also considered analyzing specifically what the design was asking me to do, originally I was leaning towards ABS but I had to consider the fact that while it is stronger plus less brittle than PLA my design parameters have a small window for maximum deformation. ABS absorbs a lot more of the forces and allows for more deformation to before breaking, meaning i might have to make other design adjustments in my mount to account for that in order to meet the deformation parameters. Ultimately I ended up choosing PLA as my material.


<img width="1000" height="800" alt="PETG Matweb ss" src="https://github.com/user-attachments/assets/9c9cd89f-f214-47b8-978d-d976d94f5833" />

<img width="1000" height="800" alt="Matweb PLA ss" src="https://github.com/user-attachments/assets/0980c8a1-4818-4c3b-87b7-f7736f619a1d" />

<img width="1000" height="800" alt="ABS Matweb ss" src="https://github.com/user-attachments/assets/3145f781-ffaf-46b1-9ac7-66f80cda8eaf" />




## Decide
As previously stated I decided on PLA as my material, it is pretty brittle material but it doesn't allow for as much deformation which I thought would be simpler for designing within the parameters given. For starting dimension assumptions I picked simple numbers at first to see if they would meet the design parameters. The calculations can be seen in the image below. 


Feature 1

Below is an image of the free body diagram I sketched and the parameters I have chosen for feature 1. Originally I had chosen a 15mm thickness to go along with feature 1. When I initially did the strength test the maximum stress was well within the safety parameters of 16.5 Mpa however when I went to see if it met the deflection parameters I saw that it was well over 0.30mm as depicted below. 




With this I knew I needed to change my design for feature 1 I increased its thickness to 20mm and recalculated the deflection and saw it now was less than 0.30mm, meaning it fit the design parameters. I then had to recalculate the strength calculations to make sure that the new thickness still allowed for the maximum stress to be below the yield stress. When I redid the calculations I saw that it was well within the safety standard so my dimensions for feature 1 were complete. My calculations are shown below. 


Feature 2 

Next I checked the parameters for the dimensions I assumed for feature 2 luckily it fit within the design parameters off first assumption as depicted in the image below. 





Sketch 

After I completed solving for my dimensions I hands sketched what my CAD design would look like to use as a reference when creating my design in the software.







CAD 

After the sketching process I began to design in the CAD software of solid works. I started with a sketch of an L shape and gave it the basic dimensions I solved for as depicted in the image below. 

<img width="2000" height="1000" alt="CAD sketch A4 project" src="https://github.com/user-attachments/assets/d6476b2b-916d-48cc-8298-e36bb865804f" />

Then I later decided to extrude it using the boss extrude feature on solid works and use the extrude cut feature to place the 3.4mm diameter holes to fit the bolts. I also used the extrude cut feature to make the holes to fit the shaft of the motor into. 

<img width="2000" height="1000" alt="image" src="https://github.com/user-attachments/assets/ee03e182-0acd-4970-9fc8-63bdc3730f19" />

<img width="2000" height="1000" alt="image" src="https://github.com/user-attachments/assets/48016910-8839-4c1b-a153-27bfba2d3f38" />

After I completed these tasks I wanted to parmetrically solve for the two lengths on both feature 1 and feature 2. So i entered the global parameters as follows: 

<img width="2000" height="1000" alt="Parametric equations on solidworks ss" src="https://github.com/user-attachments/assets/e3861c75-4295-4ede-a629-480268e97501" />



Then I used these global parameters to solve for each length also depicted in the equations in the image above, then I made sure to set each dimension equal to the global length parameter so it automatically adjusted for the parametrically designed lengths. This ended up adding about 1mm to each length compared to my hand calculated lengths. With constraining the design to the global parameters I did have one issue with length 2 it I could not get it to set equal to the length even though the global parameter equation correctly solved for the exact length I needed to input. So I ended up just setting that dimension equal to the exact length to global parameter calculated. 

<img width="2000" height="1000" alt="parametrically designed  dimensions except for side" src="https://github.com/user-attachments/assets/2879b4c6-08e5-4222-a1fc-9f3c8d45badf" /> 





After that I made sure to add to add PLA as the material since solidworks didn't already have it I had to add it to the registry then apply the material to my design.


I then created an engineering drawing for my CAD design depicted as follows:

<img width="2000" height="1000" alt="image" src="https://github.com/user-attachments/assets/80664c6a-210f-4302-b159-19c2a614d7d9" />



Link to A4 part download: <a href="A4 part.SLDPRT" download>Download the Part File</a>
Link to download A4 part drawing:  <a href="A4 part.SLDDRW" download>Download the Part File</a>







## Communicate



