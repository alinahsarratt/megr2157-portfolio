# A2 – Truss Stress Analysis

## Objective

The task for this assignment was Design a truss based on the given parameters and document the entire process to full length. With the designed trust at hand there also must be a safety and failure analyzation along with an engineering lesson that was learned. 

## Analyze
Sketch Drawings

When looking at the problem at hand I had to analyze what was given and debate how I was going to use the parameters given. I noticed we had the liberty to set the external force p to what we wanted so I set mine to 20kN. When looking at the given pin connections and parameters I had come up with two geometric design options for my trust. These are shown in the images below. 

 src="https://github.com/user-attachments/assets/7a58e1ea-2d2a-45e6-9bec-a6399e725dab" />
" alt="Description of image" width="500">

After that I was analyzing the parameters and made my first mistake I assumed pin A was the roller pin and pin B was the static pin connection this led to a miscalculation in the external forces which would be further explained later on. After the initial analyzaiton of the problem I began designing my truss. 

## Decide
I ended up picking the geometric truss with less members within it to aid in cleaner design process and I wanted less members in the truss itself. I figured if this were actually manufactured the material costs would be lower and it would create a lighter truss overall. In my design I did add a pin connection, E in order to connect the two inner members. 

External Forces

Once I had decided on a design I decided that I would first solve for my external forces. As stated earlier in the analysis section I had originally made an incorrect assumption about the external loads acting on the truss. I assumed that A was a roller pin connection and b was a static pin connection. Once I started solving for the external forces though I quickly caught my mistake because the loaded forces made no sense. In order to solve for the external force you need to calculate a moment reaction happening at the static pin connection but, when I assumed A was the roller this mean that moment reaction occurred at pin B. The surface depicted at pin A would have made it a horizontal roller pin force, meaning it could not balance out the moment reaction happening at pin B. This would have made the truss very unstable. Once I realize my mistake I quickly fixed it and recalculated the actual external forces. 

Mistake External Force FBD/Calculation


Correct External Force FBD and Calculation

Internal Loads

Once I solved for the external forces I then switched to finding the internal loads in the truss of each member. I did this by examining each joint. Now that the external forces were solved for the the easiest joint to start with was joint B since it had the most known forces acting upon it. I drew a FBD for each joint I solved for as depicted in the picture. After joint B I moved on to joint C then Joint D from there. After analyzing the truss and some of the joints I used the concept of symmetry to state that some of the members were equal to each other instead of resolving for that internal force. In order to solve for some of the forces of the internal members I had to use a trigrammatic ratio using the given lengths in the problem. 

Joint Calculations and FBD's 


Symmetry of truss FBD



Cross Section Area 

  After I solved for all the internal loads by method of joints I used the largest internal load I found and used it to calculate the minimum cross sectional area of the truss member. With this calculation the yield strength was needed. So I went back up to the instructions given to us and saw that we were using A500 structural steel as a material. I then researched tables or websites that could give me the yield value for that specific material at hand. I found on tottentubes (https://www.tottentubes.com/astm-a500-specification-information) website a table that listed the yield strength as 228MPa. I then used this in my calculation for the minimum cross sectional area. I needed to implement a factor safety of 3.5 into my solving which was depicted below. 

Then I solved for the minimum cross sectional area of the pins given. In order to do this I needed to find the pin with the most force acting on that and for me it was pin C. It not only had the highest internal load acting on it but I also had other forces as well including the external 20kN force. It was noted that pin D is the same exact way, they are equal in loads so I could have chosen either one but they would each have the same outcome. Once that was picked I used it to 


## Communicate

Failure evaluation for Members: 

Failure evalualation for joints/pins: 

Engineering Lesson: I learned the process of designing by your own choice and learning how to defend your design choices. I got to not only practice my critical thinking skills I learned the importance of documenting and communicating your process to others. Remembering to even document the mistakes I made was something I had never practiced before I was used to giving individuals the finished product. 
