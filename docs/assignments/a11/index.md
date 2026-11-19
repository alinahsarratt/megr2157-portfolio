# A11 – Motor Selection

## Objective


## Analyze
For this part of the project, I needed to find two motors that could provide enough torque to move my leadscrews while staying within the required speed range of 1–50 mm/min. Since my design has two leadscrews, I decided to use one motor for each screw. From my previous calculations, I found that each screw needed 2.11 N·m of torque. After using my safety factor of 4, I got a required torque of 8.44 N·m per motor. I also reused my speed calculations that were a range of 0.625-31.5 rpm. These helped me select a motor from McMaster. Below is my work:
<img width="600" height="910" alt="image" src="https://github.com/user-attachments/assets/a0922509-b4e3-4745-af68-38d2ce3b3851" />




## Decide
After looking through different motors on McMaster, I decided to go with the 6470K61 DC gearmotor. This motor runs on 90 V DC and has a continuous torque of 31.64 N·m and a rated speed of 42 RPM. I chose this motor because it provides more than enough torque for my design while also being able to reach my required speed. I also wanted a gearmotor because the gearbox helps provide more torque at lower speeds, which works better for my leadscrew system.
One thing I had to consider was that the motor's rated speed is higher than my maximum required speed of 31.5 RPM. At first, this seemed like it could be a problem because running it at 42 RPM would make my leadscrew move faster than the allowed speed. However, I realized that just because the motor can run that fast doesn't mean I have to operate it at that speed. I would just need a way to limit the motor speed to stay within my required range. Below is the torque speed graph that I used to analyze this:
<img width="1245" height="950" alt="image" src="https://github.com/user-attachments/assets/6936939b-92f2-42c7-8067-4f4b525fdd26" />

After that I needed to do calculations in order to design a motor bracket that would attach my motor to the T-slot frame on the tester. Below are my calculations for my design. I calculated the minimum thickness needed for the motor mounting bracket to safely support the motor during operation. I chose A36 steel as my material, which has a yield strength of 250 MPa. Since the system uses two motors, each driving its own lead screw, I used the operating torque of 2.11 N·m per motor and a safety factor of 4. This gave me a design torque of 8.44 N·m.
I then used the mounting hole dimensions and bolt spacing to calculate the force acting on each of the four bolts. After finding the force, I used the allowable bearing stress to solve for the minimum required thickness, which came out to approximately 0.000865 inches.
Even though the calculated minimum thickness was very small, I decided to use 0.25in for my final design. I chose a larger thickness to make the bracket more rigid, and provide better support for the motor. 

After that I began to design my motor housing bracket in solidworks. I started with extruding the base piece that would connect to the T-slot frame. I had to measure the slots within the T slot frame to make sure the holes for the bolts on the base had the same spacing as the slots. Then I extruded another piece off of that, this piece would connect directly to the motor so I made sure to make the holes slot holes like my chosen motor had and aligned based off of the motor drawing. After that I added a triangle support through the middle to help with the load. This also allowed my design to be more practical. Below are my steps for this process. 

<img width="2505" height="1705" alt="image" src="https://github.com/user-attachments/assets/0a9f09c6-0359-4860-b633-73be4b66ebf5" />
<img width="2972" height="1890" alt="image" src="https://github.com/user-attachments/assets/961a99ac-e7c1-4225-984b-f896fbb9e5bd" />
<img width="3105" height="1870" alt="image" src="https://github.com/user-attachments/assets/6b71a45a-b890-4ebb-8a6f-52209a28d598" />
<img width="685" height="385" alt="Screenshot 2026-11-16 165328" src="https://github.com/user-attachments/assets/88b26e4c-f09d-45f0-bd56-26d5a40c65d5" />
<img width="2845" height="1752" alt="image" src="https://github.com/user-attachments/assets/8e91dbbb-a695-48c6-bc62-c416503cd912" />
<img width="3085" height="1837" alt="image" src="https://github.com/user-attachments/assets/b9ca29c6-51a0-459a-b9f0-ccc52ad56b70" />

For this part of the project, I decided to use A36 steel for my coupler since I was already using it for my motor bracket. I used my previously calculated design torque of 8.44 N·m and the yield strength of A36 steel to calculate the minimum outer diameter using torsional shear stress. Since my motor shaft is 3/4 inch and my leadscrew is 3/8 inch, I decided to use a stepped-bore coupler with two different inner diameters to account for this. After solving the equation, I got a minimum outer diameter of 0.758 inches and a minimum wall thickness of 0.004 inches. Since this thickness was really small and wouldn't be practical for an actual coupler, I decided to use a 1-inch outer diameter instead. This gives me a thicker wall and keeps the torsional shear stress below the material's shear yield strength. I will use these dimensions as my starting point in SolidWorks. Below is my calculations for this part:
<img width="842" height="570" alt="image" src="https://github.com/user-attachments/assets/6a0b3fba-14c9-430a-9909-4248b70074cc" />

Instead of designing my own model in solid works I found a working model on Mc Master. I selected McMaster part 3084K33, a steel clamping rigid shaft coupler. This coupler fits my 3/4-inch motor shaft and allows the opposite bore to be machined to fit my 3/8-inch leadscrew. Since my leadscrew is threaded, I would need to machine a smooth section at the end so the coupler can properly grip it. I chose this coupler because its rated torque exceeds my required design torque of 8.44 N·m. However I adjusted my previous design calculations of 1 inch outer diameter of the coupler because I chose this model instead of designing my own in solid works. Below is my adjusted calculations:
<img width="815" height="545" alt="image" src="https://github.com/user-attachments/assets/b2d84f39-77c0-409a-96a6-dca1a8239419" />


<h3>Motor Mounting Assembly - SolidWorks Files</h3>

<p>
  Below are the SolidWorks part files used for my
  motor mounting assembly.
</p>

<ul>
  <li>
    <a href="3084K33_Machinable-Bore%20Clamping%20Shaft%20Coupling.SLDPRT" download>
      Download Shaft Coupling
    </a>
  </li>

  <li>
    <a href="6470K61_DC%20Gearmotor.SLDPRT" download>
      Download DC Gearmotor
    </a>
  </li>

  <li>
    <a href="motor%20bracket%20housing.SLDPRT" download>
      Download Motor Bracket Housing
    </a>
  </li>
</ul>



## Communicate
