# A6 – [Topic]

## Objective
This week we were tasked with taking our design dimensions we solved for last week and create a CAD model of our design. The CAD design was to be parametrically designed with the controlling factor that we found on each factor. After the model was completed we were tasked with creating an engineering drawing of the model. I was also tasked with making a model and drawing for the link that was supposed to connect to my design. 

## Analyze
I went back into my notes to review the which was the controlling factor strength or stiffness on my features. For all of my features strength was the controlling factor, this allowed me to start designing around my strength dimensions. 

## Decide
I started to model the cylindrical feature A first, instead of doing the parametric designs first I did a rough cad model just to get the basic shape down. So I started sketching the circle then later started building off of that. 

<img width="3155" height="1797" alt="circle sketch A6" src="https://github.com/user-attachments/assets/a4dff24e-9420-4e2a-ad83-6887d4458ee2" />

<img width="3165" height="1915" alt="A6 " src="https://github.com/user-attachments/assets/133d9eab-fb8f-4383-bf3e-edbb2c9a5111" />

<img width="3177" height="1885" alt="image" src="https://github.com/user-attachments/assets/17d5b65f-8cd9-44cb-b97b-8a817be06fa2" />

After I made a rough design of the model I decided to add all the global parameters I needed to make the model to the design it parametrically. 
<img width="2205" height="1255" alt="image" src="https://github.com/user-attachments/assets/cae6e9f5-6b58-4589-99bd-57f882fe4653" />

<img width="2292" height="1170" alt="image" src="https://github.com/user-attachments/assets/ad039cb1-f338-436d-b9e1-77efc6578d15" />



After that I first parametrically designed feature A tying the diameter to the equation as depicted below. 
<img width="3162" height="1897" alt="diameter constrain" src="https://github.com/user-attachments/assets/467cbf2e-6cd2-4fc8-98a8-601a402216cf" /> 

After that I moved on to globally constrain feature B, this is depicted in the image below. I made sure to constrain the length of b as the length of 2.00 inches, the base of b as the 0.5 I assumed in my previous calculations I solved for, then I constrained the thickness to 0.18 inches as the equation solved for it. 

<img width="3125" height="1842" alt="image" src="https://github.com/user-attachments/assets/ac88d349-7950-4276-8c47-de73a2942d78" />


I then realized feature B was not centered so I went ahead and centered this feature through the use of geometric constrains below is the uncentered, then below it centered version of this future. 

<img width="3167" height="1887" alt="not centered feature b and A" src="https://github.com/user-attachments/assets/9d06ac87-becb-4cf6-aaab-7d1175f21271" />

<img width="3137" height="1777" alt="centered feature B" src="https://github.com/user-attachments/assets/137fd0f7-e13c-44d4-9652-d3a57bf37683" />

After that I moved on to constraining feature C to my calculations and global equations. I constrained the length of the box to length c in my global parameters which in this case was 4 inches. Then I constrained the height of C. to 1.03 inches, I later figured out this was wrong because it shouldn't have been the height of of the beam. The 1.03 was actually the height of the cross section of c the height of the beam was actually equal to my global parameter b. 

In attempting to constrain c I knew in order to have the total height of the box I need to combine the heights of features c, d and e together so I made a global parameter adding each height together to constrain the box to. However I made the mistake of adding the correction heights not the actual heights of the beams and axial bar. This resulted in my design being way to tall as shown in the image below. 

<img width="3125" height="1765" alt="height E, base D, height C constrains" src="https://github.com/user-attachments/assets/52542810-c85e-4ffc-bac4-02330f89c5bf" />

I immediately knew I had to fix it so I quickly realized the real height of the beam for c was equal to my global parameter b and so was my height for e, then the height for d was actually the base d global parameter I solved for in the equation. I was then as shown in the image above constrain the thickness of D as well while fixing this feature. I constrained D to its correct thickness of 0.56 inches. This fixed the shape of the box feature completely. In making the total height constrain equation I was also able to add the 0.5 inch, "b" global parameter constrain to feature E. The improved and fully constrained designed can be shown in the images below. 

<img width="3180" height="1875" alt="constrained part 1" src="https://github.com/user-attachments/assets/fe62c8bd-58dc-499b-9442-df912896809d" />

<img width="3110" height="1907" alt="constrain part 2" src="https://github.com/user-attachments/assets/d6ba3794-fef0-463b-bb0f-3039e3777513" />

<img width="3157" height="1905" alt="finished part A6" src="https://github.com/user-attachments/assets/5297bea4-6cda-47f9-9de0-9d0bf243b9b1" />

I also made sure in order to extrude the top box to the right constrained length I made sure to examine each of the different features minimum cross section height and for d the length of d. The height e was 1.122 inches the height c was 1.033 inches and the length d calculation was 2.00 inches. So since d had the largest minimum for this dimension I knew I had to use this value to constrain the boxes extrusion to 2.00 inches as depicted in the picture directly above. 


After that I decided to add tolerances on my feature A according to the clearance fit it was supposed to have last week, I based the tolerance dimensions on the Rc3 tables found in my machinery's handbook last week. 

<img width="3165" height="1935" alt="image" src="https://github.com/user-attachments/assets/2bba8ece-9d35-440a-9c62-74d2aab74d8a" /> 

<img width="2292" height="1170" alt="image" src="https://github.com/user-attachments/assets/ad039cb1-f338-436d-b9e1-77efc6578d15" />






## Communicate
Reflection 
One instance where I used a specific equation was the diameter constrain on feature A I knew that the strength equation to solve for it was calculated in my handwork from last week and that same calculation was done by the solid works software in my global parameters I attached both below to see the comparison. There was no need to change it from its original calculation later on in my assignment it worked with the rest of my design calculations. 

<img width="655" height="1127" alt="image" src="https://github.com/user-attachments/assets/25e8cae7-c574-45d1-91c1-67530c955c99" />


<img width="2292" height="1170" alt="image" src="https://github.com/user-attachments/assets/ad039cb1-f338-436d-b9e1-77efc6578d15" /> 



