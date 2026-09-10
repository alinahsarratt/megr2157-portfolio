# A3 – [Topic]

## Objective

In this assignment we were tasked with designing a aluminum beam with a circular cross section based on the parameters given. The force had to be between 300ibf and 500 ibf. The modulus of elasticity had to be between 8.5x10^6 and 11.5x10^6 psi and the maximum elongation was 0.009in. The material of the beam was aluminum, this gave us room to pick the values of the beam that we wanted such as height, length and diameter of the cross section in order to model it, then we parametrically designed it in a CAD software to compare those projected results to our calculated ones based on our values. 

## Analyze
When looking at the given parameters, it would make the most sense to stay away from the lower ends of the spectrum because that would be the best case scenario especially in terms of force load. I also wanted to keep in mind that flat numbers would most likely make the the math work out easier. 

## Decide
I decided to choose 400ibs for the force, 10x10^6 for the elastic modulus and 0.5in for the diameter. I kept the maximum elongation value the same. I used the assumed diameter I gave to solve for the length of my beam, with the elastic elongation formula depicted in the image below. The length I hand calculated for my beam was 44.18 inches. 



Now it was time to parametrically design this in a CAD software to compare the length to my hand calculated one. I first extruded a 0.5 in diameter circle. Then, I was able to enter the parameters depicted in the image below into the Solid works software. I acquired the same length as I had in my hand calculations which was 44.18 inches. I then was able to run the simulation using the parameters I had assigned and my extruded material I assigned which was 6061 aluminum. When I first ran the test I got these displacement results depicted in the image below. 





Here I realized the displacement FEA calculation of 2.25x10^-5in was way smaller than my target one of 0.009in, from this I immediately knew something was wrong. I realized in the FEA calculation I accidentally set my tensile force to 1ibf instead of 400ibf. So once I fixed it I got the correct FEA results. My actual maximum displacement was about 9.007x10^3 which was actually way closer to my target of 0.009in. I calculated the difference or discrepancy between the two values in the image below. 



My hand calculation gave me an axial deflection of 0.009 in, while my FEA gave me 0.009007 in. When I calculated the percent difference, I only got about 0.078%, so basically the two values were almost exactly the same. I think they came out so close because my bar is pretty simple. It has the same cross section throughout the whole bar and the force is just pulling straight on it, so there really aren’t any stress concentrations or anything complicated that would make the FEA act much differently from my hand calculations.I would probably trust my FEA result a little more just because it actually uses my CAD model and includes the way I fixed and loaded the bar in SolidWorks. But since my hand calculation was less than 0.1% different from my FEA, I would still trust both results for this design. The bar and loading are simple enough that there really shouldn’t be a huge difference between the two anyway.




Next I wanted to test the length change of my beam if I changed some of my original parameters. Below in the image I depicted my original parameters and what I changed them two. I also listed what I guess what would happen once these parameters were changed and what actually occurred. 



There was an increase in length as I predicted which can also be seen in the solid works calculation. 









## Communicate
Some engineering lessons I learned in this assignment is to work through your mistakes and understand what may have caused them in order to fix your design. I also learned the importance of how to analyze how changing certain parameters can change your design at hand, along with how to analyze how those certain parameters will impact the design itself. I spent about 6 hours on this assignment due to difficulties with the CAD software and all the mistakes I had to work through. 
