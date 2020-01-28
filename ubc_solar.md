---
layout: post
title: UBC Solar
description: My experience at UBC Solar
image: assets/images/ubc_solar_car.jpg
nav-menu: true
---

UBC Solar is a student-led engineering design team. The goal is to build a solar-powered vehicle and compete on the international stage in the Formula Sun Grand Prix and American Solar Challenge.

I had the pleasure of co-leading the team administration and leading the electrical division from January 2018 to August 2019. In that time, I lead the team through the development of its third solar car since the clubs inception in 1996. I was responsible for managing the organization of 50 members and the finances of a $100 000 budget. We designed the car from the ground up with little prior documentation or connections to the rest of the solar car world. It was a chaotic 20 months, and an experience that shaped who I am as a person, a leader and an engineer. 

<img src="assets\images\the_team.jpg">

## Co-Captain
As co-captain I was responsible for the operational administration which included:
- Creating a budget and managing team finances 
- Writing sponsorship and grant applications
- Leading weekly meetings including a team-wide presentations, updates and SCRUMs
- Acting as the team’s liaison to UBC’s Faculty of Applied Science, competition organizers - Innovators Education Foundation (IEF), and the solar car community
- Organizing team safety training and procedures 

 
As head of the team I learned what made this organization so special. The document linked below is an example of a report we would send to our supporters. The Daniel's Family Foundation committed $60 000 over three years while I was co-captain. The admin team and I worked hard to make this happen.
<br/>
[Daniels Family Foundation Year End Report](https://drive.google.com/open?id=1b5JVWUEGK7YGHlsSY8RqUhjPsevMjyPm)
(A link to a viewing file in my google drive)

<center> <h4>  A thinking session on we hoped the Admin team would do </h4> </center>
<img src="assets\images\Importance of Admin.jpg">
During my time at UBC Solar I re-designed the structure of the team. When I became co-captain there wasn’t a proper leadership transition and it was a very stressful experience. We needed a way to ingrain the knowledge we spent so long to achieve. One of the solutions to solidify this organizational knowledge was to develop a strong administrative team presence. 

<center> <h4>  Here's me working on the car!</h4> </center>
<img src="assets\images\working_on_the_car.jpg">

## Electrical Lead
As the electrical lead I was responsible to organize and synchronize the four subteams under the electrical division. These sub-teams include:
- Power Electronics: Responsible for design specifications and selecting components for the motor, motor controller, maximum power-point trackers and solar array
- Battery: Responsible for the design of the high-voltage battery pack and the low-voltage battery management system
- Low-voltage Systems: Responsible auxiliary low-voltage systems and boards such as: the dashboard, connectors, main control node
- Software: Responsible for the firmware for in-house designed boards and the software for the data management website
<br/>
Specifically, I worked with a group of leads that then organized the members of their sub-team. This entailed:
- Developing a timeline of major milestones and working with subteam leads to develop gantt charts on a team-by-team basis
- Twice-a-week meetings to talk through designs, and to address development gates
- Helping subteam leads find resources through research or campus connections
- Developing budgets for each subteam

 
As head of the electrical team I vetted the design, purchased and manufactured the electrical system. Knowing the system inside-out was necessary for the submission of the electrical design report to competition officials. This document provides a detailed summary.  <br/>
[FSGP Electrical Design Report](https://drive.google.com/file/d/1JXfAFOqf5ivnvS3uNIGVRVvpx85yX1YJ/view?usp=sharing)
(A link to a viewing file in my google drive)

<center> <h4> The Electrical Block Diagram </h4> </center> 
<span class="image fit"><img src="assets\images\electrical_diagram.jpg" alt="" /></span>

## Daybreak

<center> <h4>  Here is a rendering of the car the team envisioned in January 2018. </h4> </center>

<span class="image fit"><img src="assets\images\rendering.jpg" alt="" /></span> 

## Technical Details

In this section I will outline some technical details of the project. As Electrical Lead my primary role was to mobilize a group of talented young engineers and in no way do I want to take credit for others work. Related to design, my responsibility was to vet the functionality and effectiveness of the design. For example I did not construct the low-voltage system PCBs in Altium, but I did guide every decision in the design path. That being said, I personally contributed to the manufacturing and testing of every electrical component of the car. At the end of the day, I ensured everything worked.

### Power Electronics

<p><span class="image left"><img src="assets\images\NGM_on_it's_face.jpg" alt="" /></span> This is our solar cars in-hub motor, an NGM SCM150. To use an in-hub motor is common practice in the solar vehicle building. Specially built motors fit torque requirements of the light vehicle, and demand a suitable power from the battery pack.  </p>

<p><span class="image right"><img src="assets\images\solar_testing.jpg" alt="" /></span> Most critically, high efficiencies without drivetrain losses are ideal when each watt of solar power is precious. In design we had originally opted not to use this motor, because it is almost double the weight of similarly efficient/powerful motors. We made a concession because this motor was almost an eighth the price of the "ideal motor". <br/><br/> Here is an example of the cars solar array. In this photo we are conducting a functionality test of the Maximum Power-Point Tracker (MPPT). This particular MPPT is a boost converter selected so that the 60V solar arrays strings could charge the 100.8V battery pack. Two 12V lead-acid batteries were used as a load. We measured the input and output voltages and currents to make sure everything was performing as expected. It was! </p>

### Battery 

<p><span class="image left"><img src="assets\images\battery_pack.jpg" alt="" /></span> The battery pack of the solar car is composed of 420 Li-ion 18650 cells. </p>
 
<p><span class="image right"><img src="assets\images\working_on_battery.jpg" alt="" /></span> 28 modules of 15 parallel cells are strung together to form a 100.8V nominal battery back with 5.14kWh of power. The battery pack voltage, current, temperature and state of charge are monitored by an off-the-shelf Elithion battery management system (BMS). Pictured below are the “cell boards” that relay pack voltage to the BMS master. <br/> <br/> This battery pack was easily the most significant electrical challenge of the car. The mechanical design features cells arranged in plastic holders, spot-welded to an aluminum grid then soldered to copper plates that can be bolted to an adjacent module. The electrical design features 4 contractors to each of the major terminals of the high voltage system (array, motor controller, positive and negative terminals of the battery pack), a supplemental battery pack for start up and a circuit to switch to the DC-DC converter power. It was a profoundly buggy circuit further complicated by the black box that is an off-the-shelf component (the Elithion BMS master).</p>
<br/>
<center> <h4>  The BMS cell boards up close! </h4> </center>

<img src="assets\images\battery_up_close.jpg">

### Low Voltage System

<center> <h4>  Main Control Node PCB </h4> </center>

<div class="box alt">
	<div class="row 50% uniform">
		<div class="6u"><span class="image fit"><img src="assets\images\main_control_node_bare.jpg" alt="" /></span></div>
		<div class="6u"><span class="image fit"><img src="assets\images\main_control_node.jpg" alt="" /></span></div></div>
</div>
The low-voltage system (LVS) is a catch-all term to cover many critical components of the car that simply were power components. <br/> In particular the LVS covered:
- driver input: acceleration, signal lights, horn etc.
- standard vehicle lighting
- a CAN network for module communication
- radio and cellular driver and system communication 
The majority of electrical in-house design was covered in this section of the vehicle. The PCBs pictured below are the main control node and the driver dashboard.
<br/>
<br/>
Through the development of these I learned the importance of thorough design. As you can see the right photo of the main control node (above) I had to make some last minute changes to correct the pull-up resistors of the accelerator’s encoder. This oversight could have been eliminated with a component-by-component design verification and test prior to manufacturing the PCB.

<center> <h4>  Driver Dashboard: That big red buttton is the emergency off switch </h4> </center>
<span class="image fit"><img src="assets\images\Dashboard.jpg" alt="" /></span> 

### Thank you for reading about my solar car project! It was quite an experience to say the least. I have only included a sliver of the information here, so should you be interested in hearing more feel free to reach out to me!

<br/><br/><br/>

<!---

<p><span class="image right"><img src="assets\images\motor_controller.jpg" alt="" width="1100" height="663"  /></span> <br/> <br/> . </p>




<img src="assets\images\Don't try to build an MPPT.jpg">
<img src="assets\images\electronics_location.jpg">
<img src="">
<img src="assets\images\solar_testing.jpg">

### Battery 
<img src="assets\images\battery_pack.jpg">
<img src="assets\images\battery_up_close.jpg">
<img src="assets\images\working_on_battery.jpg">


### Low Voltage System

<img src="assets\images\Dashboard.jpg">

<img src="assets\images\main_control_node.jpg">
<img src="assets\images\main_control_node_bare.jpg">

<br/><br/><br/><br/>


## Competition 


<img src="assets\images\work_day.jpg">
<img src="assets\images\UBC Solar with NUSoalr.jpg">
<img src="assets\images\vacuum_seal.jpg">
<img src="assets\images\bottom_aeroshell.jpg">





<img src="assets\images\lighting_schematic.jpg">
<img src="assets\images\low_votlage_system.jpg">
<img src="assets\images\im_in_a_car_frontview.jpg" align="right">
<img src="assets\images\im_in_a_car_sideview.jpg">


--->
