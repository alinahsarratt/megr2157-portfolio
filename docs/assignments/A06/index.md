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
<img width="2075" height="1092" alt="Global variables A6 ss" src="https://github.com/user-attachments/assets/24edc68c-1a09-46da-a285-745a1553d4f1" />

After that I first parametrically designed feature A tying the diameter to the equation as depicted below. 
<img width="3162" height="1897" alt="diameter constrain" src="https://github.com/user-attachments/assets/467cbf2e-6cd2-4fc8-98a8-601a402216cf" /> 

After that I moved on to globally constrain feature B, this is depicted in the image below. I made sure to constrain the length of b as the length of 2.00 inches, the base of b as the 0.5 I assumed in my previous calculations I solved for, then I constrained the thickness to 0.18 inches as the equation solved for it. 

<img width="2717" height="1507" alt="constrained B" src="https://github.com/user-attachments/assets/98c6c1af-b7c5-4af8-a429-ffaae5fe8a1c" />

I then realized feature B was not centered so I went ahead and centered this feature through the use of geometric constrains below is the uncentered, then below it centered version of this future. 

<img width="3167" height="1887" alt="not centered feature b and A" src="https://github.com/user-attachments/assets/9d06ac87-becb-4cf6-aaab-7d1175f21271" />

<img width="3137" height="1777" alt="centered feature B" src="https://github.com/user-attachments/assets/137fd0f7-e13c-44d4-9652-d3a57bf37683" />

After that I moved on to constraining feature C to my calculations and global equations. I constrained the length of the box to length c in my global parameters which in this case was 4 inches. Then I constrained the height of C. to 1.03 inches, I later figured out this was wrong because it shouldn't have been the height of of the beam. The 1.03 was actually the height of the cross section of c the height of the beam was actually equal to my global parameter b. 

In attempting to constrain c I knew in order to have the total height of the box I need to combine the heights of features c, d and e together so I made a global parameter adding each height together to constrain the box to. However I made the mistake of adding the correction heights not the actual heights of the beams and axial bar. This resulted in my design being way to tall as shown in the image below. 

<img width="3097" height="1890" alt="image" src="https://github.com/user-attachments/assets/8b3ce41e-fddd-4f30-8aec-649cd65e92a0" />







## Communicate

