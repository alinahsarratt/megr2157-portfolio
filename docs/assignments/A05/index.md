# A5 – [Topic]

## Objective
This week we were tasked to design a bracket out of one of the three given materials A36 steel, aluminum 6061 T6 or Titanium (Ti-6Al-V4). In order to design the bracket we had to perform a strength analysis and stiffness analysis on each of the five features in the initial bracket design. This determined what was the controlling factor through a comparison of the strength and stiffness analysis which then led to dimension determination for the actual design. 

## Analyze
When considering the problem at hand we had to make initial design choices such as the material and what would be the applied load on the bracket. There was a range of 500 lbf < F < 800 lbf. There was also a need for assumptions to be made to aid in figuring out the design especially when it came to certain failures, so each of those had to be analyzed per feature. However there was one assumption already given to us which was that there was no consideration of direct shear stress failure.             

## Decide
One of the first decisions I made was what material I was going to use, I decided to go with the A36 steel. I wanted the bracket to have a strong material so it could handle heavy loads since the second decision I made was to design for the worst case scenario in the applied load which was 800ibf. After that I researched the steel material properties so I could use them in my design calculations. After the standard design choices were complete I started to calculate my dimensions for feature A. For each feature I started out with strength analysis then later went into a stiffness analysis. 

Strength Analysis calculations and assumptions for Feature A:

<img width="655" height="1100" alt="image" src="https://github.com/user-attachments/assets/8fdddec8-4c02-499f-86ef-47762a0fb9b3" />



After strength analysis for feature A was complete I had a minimum diameter that I could use for the design dimensions. After I moved on to feature B. I modeled feature B as an axially loaded bar and had the same applied load transferred from A. After I made my assumptions for feature B I solved for the minimum cross sectional area. This is depicted in the image below. Even though the cross sectional area is equal to the base multiplied by the thickness I did not choose those dimensions until after the stiffness analysis so I wouldn't choose the wrong dimensions before I knew the controlling minimum area was. 

Strength Analysis calculations and assumptions for Feature B:
<img width="1000" height="1500" alt="image" src="https://github.com/user-attachments/assets/f0e69238-2208-408f-9b25-2a3edc6ba2f1" />


Once feature B was complete I then went on to complete my strength analysis calculations for feature C. I modeled C as a simply supported beam with a point load, in this case the 800ibf applied load, acting at the center. One of my assumptions was that this was symmetric so I knew in feature D that this load would be split in half because there is two feature D's on each side. Below are my calculations for the dimensions of the minimum base and height for the feature. Just as in B I did not decide on the official specific base and height dimensions until after my stiffness analysis. 

Strength Analysis calculations and assumptions for Feature C: 
<img width="1600" height="700" alt="image" src="https://github.com/user-attachments/assets/835bb3a5-5d6c-4a71-933d-d2099ba89d18" />


Then I moved on to feature D, this was modeled as an axially loaded member however the applied force was 400ibf due to the symmetric center load of feature C as previously mentioned. Just as in feature B I was able to solve for the minimum cross sectional area.

Strength Analysis calculations and assumptions for Feature D: 
<img width="570" height="1462" alt="image" src="https://github.com/user-attachments/assets/a90e2aa2-8b01-4ea7-9349-403e88f0d210" />


The last strength analysis was for feature E, I modeled this as a cantilever beam. Since I broke the design as two feature E's the halved applied load of 400ibf from feature D was transferred into feature E which is how I completed the calculations below. Similar to feature C I found the minimum base and height dimensions, however each base and height specifically would be chosen after the stiffness analysis. 

Strength Analysis calculations and assumptions for Feature E:
<img width="695" height="1450" alt="image" src="https://github.com/user-attachments/assets/957a8646-5b61-48dc-9ab5-43e1bf86d1ee" />



After I completed the strength analysis for each feature I followed the exact process but this time I completed a stiffness analysis. This allowed me to see what was the controlling factor for each feature within my design. Then I could pick dimensions based on that. 

For feature A I solved for the diameter again using the equations below and a minimum deflection of 0.005 inches, that minimum deflection was used in every calculation going forward as well. 

Stiffness Analysis calculations and assumptions for Feature A:




Once I found the diameter from the stiffness calculation I compared it to the strength minimum diameter found before and realized that the strength minimum diameter was larger. This meant that the strength was my controlling factor for feature A so now I had my first set dimension of 0.968in diameter. 


After I conducted the stiffness analysis for feature B. I found the minimum cross sectional area in terms of stiffness.

Stiffness Analysis calculations and assumptions for Feature B:


Since the minimum cross sectional area for feature B in the stiffness analysis was smaller than the minimum cross sectional area for the strength analysis, strength was the governing factor for feature B as well. This allowed me to base my base and thickness dimensions on this cross sectional area. Since it had to be at least 0.089 inches squared. I chose the base of 0.5 in and a thickness of 0.18 inches so it came out to 0.090 inches squared. 



For feature D a similar thing happened. I used conducted the stiffness analysis for feature D to find which minimum cross sectional area was larger and therefore would be controlling. In the image below I found that the strength minimum cross sectional area was larger than the stiffness analysis. This area was 0.0444 inches squared, so I was able to choose my base and thickness after based on this area. So I chose my base as 0.25 in and my thickness as 0.18 in, this would give a total cross sectional area of 0.045 inches squared. All of this is shown in the image below. 




The next thing that was solved for was feature C and E. Both of these features a stiffness analysis was conducted to solve for the base and the height of each. However the in the stiffness analysis it was bh cubed instead of squared. So I couldn't directly compare it to the strength analysis because it technically solved for different things. So I had to pick a base dimension and assume it so I could solve for the height in each analysis. Through the height calculation I could pick a controlling modulus for each feature. For each feature the strength was the controlling modulus this allowed me to have a base and height dimension for each feature. This is depicted in the image below. 

Sketches 




Linkage 

After I had to find the minimum cross-sectional area of the link, I used the 800 lbf applied load, a safety factor of 4, and the yield strength of A36 steel. This gave me a minimum area of 0.0889 in². However, since there is a 1-inch hole going through the link, I had to account for the material that would basically be missing from that section. I used \(A=(w-d)t\) and chose a width of 1.50 in and a thickness of 0.25 in. This gave me an actual net area of 0.125 in², which was greater than my minimum, so those dimensions worked.


I also had to make sure the link would not deform too much, so I did a stiffness analysis using \(\delta=FL/AE\). I used the maximum allowed deflection of 0.005 in and got a minimum area of 0.0166 in². This was way smaller than the 0.0889 in² I needed for strength, so strength ended up controlling my final dimensions. This is shown in the image below. 


Next I worked on the type of fits for each feature. For the hole that connects the link to Feature A, I needed a running/sliding fit so that the parts could actually move freely without having a bunch of extra space between them. I used Table 8a on page 64 of Machinery’s Handbook, 32nd edition. Since my basic diameter was 1.000 in, I used the 0.71–1.19 in range. I then chose an RC3 fit because it was the closest fit that would still allow the  parts to run freely. From there, I used the RC3 values in the table to determine the tolerances for the hole and shaft. Below is a picture of the table I used. 


For the 1-inch shaft, I used an FN1 light drive fit because the design required light assembly pressure. Using the 0.95–1.19 in range in Table 11 on page 659 of Machinery’s Handbook, 32nd edition, I found the hole limits to be 1.0000–1.0005 in and the shaft limits to be 1.0008–1.0012 in. This creates a small interference between the shaft and hole, meaning some pressure is needed to assemble the parts. 













## Communicate
Lessons learned:

When it came to the governing factor of my design it was the strength analysis each time the dimension values on the strength analysis were greater than those of the stiffness analysis. The feature I am going to point out specifically for this would be feature A. The difference between the stiffness and strength analysis for that feature was 0.389 inches. 

Next, there was multiple times the force load calculation from one feature fell into the calculation of the next connecting feature. One distinct instance this happened was when the applied load that acted at the center of feature C, trickled into the next feature D but because it was symmetric it actually split the applied load by 2. This meant instead feature D having an applied load of 800ibf it actually had a 400ibf load. There was no mistake in my work when it came to calculating this and how it fit into my dimension calculations for feature D. But something that would have caught this if the strength analysis calculation or stiffness calculation had an unreasonably high minimum cross sectional area. If the required area was much larger than my other calculations, I could check the load path and realize that I may have incorrectly used the full 800 lbf on each side instead of the correct 400 lbf.

One assumption that I made that would likely change the outcomes if it were different was that the cross sectional areas of the design were considered to be constant. If this assumption weren't true there would have to be sections within each feature that had different dimensions from one another instead of constant ones. For example with feature A there would have to me sections with different diameters, and I would have had to test each one of those instead of solving for one constant diameter across the entire cross section. 

Overall, I learned how to analyze each test of both strength and stiffness in order to apply the appropriate dimension to my design. I got a better understanding of what is the controlling factor when it comes to designing something. This project took me about 9 hours total. 


