








# A2 – Truss Stress Analysis

## Objective

The task for this assignment was Design a truss based on the given parameters and document the entire process to full length. With the designed trust at hand there also must be a safety and failure analyzation along with an engineering lesson that was learned. 

## Analyze
Sketch Drawings

When looking at the problem at hand I had to analyze what was given and debate how I was going to use the parameters given. I noticed we had the liberty to set the external force p to what we wanted so I set mine to 20kN. When looking at the given pin connections and parameters I had come up with two geometric design options for my trust. These are shown in the images below. 

<img width="597" height="685" alt="2initialtrussdesigns" src="https://github.com/user-attachments/assets/3d0539c3-bb48-42a5-aa3c-da07ef89ca57" />

After that I was analyzing the parameters and made my first mistake I assumed pin A was the roller pin and pin B was the static pin connection this led to a miscalculation in the external forces which would be further explained later on. After the initial analyzaiton of the problem I began designing my truss. 

## Decide
I ended up picking the geometric truss with less members within it to aid in cleaner design process and I wanted less members in the truss itself. I figured if this were actually manufactured the material costs would be lower and it would create a lighter truss overall. In my design I did add a pin connection, E in order to connect the two inner members. 

External Forces

Once I had decided on a design I decided that I would first solve for my external forces. As stated earlier in the analysis section I had originally made an incorrect assumption about the external loads acting on the truss. I assumed that A was a roller pin connection and b was a static pin connection. Once I started solving for the external forces though I quickly caught my mistake because the loaded forces made no sense. In order to solve for the external force you need to calculate a moment reaction happening at the static pin connection but, when I assumed A was the roller this mean that moment reaction occurred at pin B. The surface depicted at pin A would have made it a horizontal roller pin force, meaning it could not balance out the moment reaction happening at pin B. This would have made the truss very unstable. Once I realize my mistake I quickly fixed it and recalculated the actual external forces. 

Mistake External Force FBD/Calculation


Correct External Force FBD and Calculation


<img width="700" height="600" alt="externalforces and official truss" src="https://github.com/user-attachments/assets/8d723f03-24bd-49f5-8b93-273458f5f8d2" />




Internal Loads

Once I solved for the external forces I then switched to finding the internal loads in the truss of each member. I did this by examining each joint. Now that the external forces were solved for the the easiest joint to start with was joint B since it had the most known forces acting upon it. I drew a FBD for each joint I solved for as depicted in the picture. After joint B I moved on to joint C then Joint D from there. After analyzing the truss and some of the joints I used the concept of symmetry to state that some of the members were equal to each other instead of resolving for that internal force. In order to solve for some of the forces of the internal members I had to use a trigrammatic ratio using the given lengths in the problem. 

Joint Calculations and FBD's 

<img width="697" height="905" alt="full static analysis with joints" src="https://github.com/user-attachments/assets/c7c72ab6-c125-4f25-82fd-0f642e692499" />


Symmetry of truss FBD

<img width="600" height="500" alt="symmetry" src="https://github.com/user-attachments/assets/8ca4fb19-6b99-410d-83f8-3269bcf39cce" />



Cross Section Area 

  After I solved for all the internal loads by method of joints I used the largest internal load I found and used it to calculate the minimum cross sectional area of the truss member. With this calculation the yield strength was needed. So I went back up to the instructions given to us and saw that we were using A500 structural steel as a material. I then researched tables or websites that could give me the yield value for that specific material at hand. I found on tottentubes (https://www.tottentubes.com/astm-a500-specification-information) website a table that listed the yield strength as 228MPa. I then used this in my calculation for the minimum cross sectional area. I needed to implement a factor safety of 3.5 into my solving which was depicted below. 

Then I solved for the minimum cross sectional area of the pins given. The assumption was for a single shear in the instructions. In order to do this I needed to find the pin with the most force acting on that and for me it was pin C. It not only had the highest internal load acting on it but I also had other forces as well including the external 20kN force. It was noted that pin D is the same exact way, they are equal in loads so I could have chosen either one but they would each have the same outcome. Once that was picked I used it to calculate the cross sectional area. In order to do this I first had to find the allowable shear stress using the allowable shear yield strength given and the safter factor of 4. Once I determined the allowable shear stress I used it and the max shear stress which in this case would be the 20kn force, to solve for the minimum cross sectional area of the pin. This was a value of 0.106in^2 and 68,387mm^2. Here I did a quick mental check to make sure that cross sectional area was smaller than the cross sectional area of the truss and it was. So I proceeded 


<img width="700" height="800" alt="areacross" src="https://github.com/user-attachments/assets/c68532ce-587c-4d7c-8a04-521873fd2823" />


Diameter calculation 
I shortly after found the diameter of each pin because I thought it would be useful later in my CAD design. 

<img width="300" height="300" alt="pindiameter" src="https://github.com/user-attachments/assets/bb80aa48-8555-47fe-a509-1e790a887eab" />

Weight Calculations 

The last thing I did before proceeding to making the CAD model for the design was approximate the weight of the truss itself and each of the pins in it. First I calculated the approximate weight of the truss which is shown in the depiction below, I used the given values of density and the area value I had solved for originally. I had to list the length of each member in meters because that was useful in my calculation as shown. 

I followed up with the calculation of the pin weights. I realized I needed to assume a width for each member so I could use that width and the truss cross sectional area to solve for the thickness of each member. This was important because that thickness would directly affect the length of each pin. I assumed to use a width of 30mm making the thickness of each member 8.2. I had originally made the mistake of not taking into account that the amount of members at each pin would affect how long that pin would have to be. I originally thought that each pin would be equal in length but I quickly caught myself and realized that wasn't the case. So after I corrected my mistake by breaking the pins up by how many members were attached to each and calculated each of their lengths based off of that. These lengths were then used in the weight calculation as depicted below. 

<img width="600" height="700" alt="weight calculations" src="https://github.com/user-attachments/assets/e79297ae-95e9-466c-b6c5-b8ed58f0de39" />


At the end of my project I then implemented the material low carbon steel into the Mass properties on the CAD system so it could calculate a mass for me which I then used to calculate the weight. I wanted to inlude this section in the weight calculations. The number I go from doing this was 231,706.25 in pound force which is about 1,030,681N. I realized this was a huge number so I decided to look into it and change the properties to fix the units. I changed it to mm/N. Then got an adjusted mass number shown in the 2nd picture. 

<img width="800" height="600" alt="mass calculation CAD" src="https://github.com/user-attachments/assets/ace6ed30-bbfa-42ba-b9ed-fe2b171b4bac" />


<img width="800" height="600" alt="mass calculation metric" src="https://github.com/user-attachments/assets/3734c9d7-6e45-4772-b27b-8a82ed509702" />



CAD Design

Next I began to work on my CAD design of this. I decided to try to use the 3d assembly tool on Creo to model my truss. I began to use the extrude feature to make each of my parts I was going to use in the assembly I first used the sketch inside extrude to make a basic rectangle, I adjusted the length for each member based on which one I was making, if the members were equal in length I used the same part file for them both in the assembly. I then drew two circles, each were 15mm from the bottom of the member and 10mm away from the end of the member. I adjusted the diameter to the diameter of the pin I calculated earlier so it would create a hold that size when I extruded it. 


<img width="800" height="600" alt="trussextrude" src="https://github.com/user-attachments/assets/b5980c81-8462-4fe9-a249-5def01c4c9d9" />




I then created a part files for my pins, if they were equal in length I used the same part file for each in the assembly for convenience. I used the extrude tool to create a circle and adjusted the diameter to the one I previously calculated. Each pin length was adjusted in the extrude tool to match the calculated values that came from how many members were attached to it. 

<img width="800" height="600" alt="Screenshot 2026-09-02 233634" src="https://github.com/user-attachments/assets/d43d1a2c-b00c-4d1b-a9b2-ddae8acc1ca0" />

After that I created an assembled model of my parts. Unfortunately during this part I had trouble with the constrains, the pins were made to the right length based on the calculated values but the members were not constraining so that they laid flat against each other so the pins were a bit offset in the assembly. This mis assembly only affected the pin connections that had more than 2 members attached to it. I tried multiple times to fix this issue but I was unsuccessful. I depicted the gaps present in the image below along with the assembly of my truss. 

Gap picture 

<img width="600" height="500" alt="assemblygapexample" src="https://github.com/user-attachments/assets/50e0f635-103a-406b-a32f-6e16c7e83fb3" />

<img width="600" height="500" alt="Gapwithpin" src="https://github.com/user-attachments/assets/964be05b-9d43-4623-a9c6-c7d62d9e14b7" />



Assembly with pins 

<img width="700" height="600" alt="assemblywithpins" src="https://github.com/user-attachments/assets/d1c03f37-05b9-45f8-adfc-75943716d5b9" />





Assembly without the pins added yet 


<img width="600" height="500" alt="Screenshot 2026-09-02 233809" src="https://github.com/user-attachments/assets/dc9928df-12fb-4bd6-9d6c-85d2a17b1ce8" />

## Communicate

Failure evaluation for Members: Both Members BC and DA are under the same forces and have equal lengths. When looking at there type of failures it would be most likely due to yielding.  Some of my members are in tension and some are in compression, but for this project we are told to assume the compression members will not fail from buckling. For these specific members they have a tension force acting on them so it is likely to fail due to yielding if put under high stress.  So because of that, I mainly looked at whether the stress in my members would get high enough to cause the A500 steel to start yielding.  When looking at the other members such as BE or CE these embers have compressive forces typically this could create buckling but again due to the parameters, I would say it would still fail because of compressive yielding. Since BC has such a high force acting on it, a design that could help would be increase the cross sectional area of this member. Member CD has barely a tension force acting on it since it is essentially a 0 force member it is actually helping provide stability in the truss so it would be something that is good to keep in the design. All members are made out of the A500 steel and this material is considered ductile. 

Failure evaluation for joints/pins: Pin A and B are under the same force pressure, they are a single shear connection carrying two members one with 8.89kN of tension and the other was a 11.11kN compressive force, this creates a large amount of stress on a very small pin. This would likely cause failure due to shear failure, in order to fix this you can increase the cross sectional area of the pin which can lighten the load. Pins C and D are helped out by member CD since it is essentially a 0 force member but they still have some high loads of two compressive force of 16.03 and 11.11 kN. In order to lighten the load on these pins you could turn it into a double or triple shear pin making the load a 1/2 or 1/3 of a single shear load, especially because these pins hold 3 members. I would probably implement the same design upgrade into pin E since it is holding together four members. I would turn it into a multi-shear pin so it can withstand the heavy loads from 4 members making it less likely to fail because of shear failure. Each one of these pins is made out of hardened tool steel which is classified as a hard brittle material.  


citations: 

ASTM International. “Standard Specification for Cold-Formed Welded and Seamless Carbon Steel Structural Tubing in Rounds and Shapes.” ASTM International, ASTM A500/A500M, store.astm.org/standards/a500. Accessed 3 Sept. 2026.

American Institute of Steel Construction. Specification for Structural Steel Buildings. ANSI/AISC 360-16, American Institute of Steel Construction, 7 July 2016. AISC Specification for Structural Steel Buildings. Accessed 3 Sept. 2026.



Engineering Lesson: I learned the process of designing by your own choice and learning how to defend your design choices. I got to not only practice my critical thinking skills I learned the importance of documenting and communicating your process to others. Remembering to even document the mistakes I made was something I had never practiced before I was used to giving individuals the finished product. For a total I spent about 12 hours on this project over a couple days it took a lot of time working out my mistakes and making sense of the math in terms of how it affected my design. 


Below is a link to my zip file for assembly 

[trussmodel.asm.zip](https://github.com/user-attachments/files/31771151/trussmodel.asm.zip)

Below is a link to my pdf with my work

[A2 project  (1).pdf](https://github.com/user-attachments/files/31771242/A2.project.1.pdf)
