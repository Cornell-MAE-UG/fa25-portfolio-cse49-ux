---
layout: project
title: "ENGRD 2210 - Portfolio Assignment"
description: "Portfolio deliverables and reflections for ENGRD 2210."
technologies: []
image: /assets/images/kohler-engine.jpg
---

For this assignment, we will be analyzing and comparing the thermal efficiency of the Rehlko Command PRO CH440 Engine. This is the regulation engine mandated by SAE International for the collegiate Baja SAE Competition. 

Throughout this analysis, most data will be sourced from the manufacturer specification sheet for the CH440 engine and the SAE International Competition Rulebook for the Baja SAE competition.

The efficiency of this ideal system is given by the equation 
= 1-(1r)k-1 where r is the compression ratio (given by the manufacturer as r = 8.3) and k is the specific heat ratio, typically k = 1.4 when modeling air as an ideal gas.

Thus we find that = 1-(1(8.3))(1.4)-1=0.5711 = 57.11%. This is typical for an ideal air standard Otto Cycle.

This is the thermal efficiency of a cycle at 14 HP, yet as regulated by Baja SAE, the engine must be limited such that they only have a power of 10 HP. Let’s use the thermal efficiency from the 14 HP engine to find the thermal efficiency of the engine used in competition. 

First let’s find the work of a 14 HP cycle. Per the CH440 datasheet, the maximum torque output of 22.7 ft-lb is at 2800 rpm. 

The power output is torque times the angular speed.
P=tau*omega=30.78Nm*2*pi * 280060=9.03 kw/s 
The work of a cycle is that power per cycles per second
W=PRPM*120= 386.79 J
With the efficiency and work per cycle, we can calculate the heat inputted.
Qin= Wcyc = 677.28 J

The modification to make the engine limited to 10 HP is just to the air intake, meaning that, once the work of a cycle of a 10 HP CH440 engine is determined, the efficiency can be determined with the same formula used above.

Last year as part of his work for Cornell Baja Racing, Trevor created a dynamometer setup which measured the rpm where power band was reached, and the maximum torque the engine could reach with a hall effect sensor, a load cell, and a water break. The maximum torque was determined to be around 19 ft-lb, and powerband was determined to be at 3000 rpm. 

Insert dyno photo

With this information, we can reuse many of the equations above to find the work of the cycle, and from that, the efficiency of said cycle.

Insert Equations

P=tau*omega=22.7*2*pi * 280060= 
W=PRPM*120= 
Qin= Wcyc = 


Now that we have the theoretical efficiency of the CH440 engine modified for use in Baja SAW, let’s see how it compares to the real performance in competition.

Thermal efficiency of a power cycle in general is expressed as  = WcycQin, that is, the work produced by a cycle of work divided by the heat added during this cycle.

To calculate the amount of heat inputted, we analyze the fuel used for the engine and its lower heating value (LHV). For unleaded gasoline, the typical LHV is 12.2 kWh/kg or 43.92 MJ/kg. Baja SAE rules state all competition vehicles must use Pyrotect Part Number SFC100 as a fuel tank. The dimensions of the fuel tank are shown in the drawing (8.00in ⌀ x 7.94in). When full, the volume of fuel inside the tank is given by V=hr2=(7.94)(4)2=399.1in3=0.00654m3.

<p>
  <img src="{{ 'assets/images/baja-fuel-tank.jpeg' | relative_url }}" alt="Baja fuel tank" style="width:48%;display:inline-block;margin-right:2%" />
  <img src="{{ 'assets/images/baja-fuel-tank-drawing.jpeg' | relative_url }}" alt="Baja fuel tank drawing" style="width:48%;display:inline-block" />
</p>

The typical density for unleaded gasoline is about 0.71 to 0.77 g/mL or 710 to 770kg/m^3. To be conservative in our calculation of efficiency, we choose the highest density (i.e., a less efficient engine will need more gas to produce the same amount of work).  Thus we find that the mass of gas when the gas tank is full is m=V=(770)(.00654)=5.0358kg.
To calculate the total heat energy that can be obtained from this amount of fuel, we use the previously mentioned LHV value to calculate Q= m  LHV = (5.0358)*(43.92)=221.17MJ.
Now the trickier part: figuring how much work we get out of one full tank.

To do this, we will analyze Cornell's vehicle’s motion and fuel consumption during the 4-hour Baja SAE Endurance race. Looking at lap times, track length, and fuel consumption during the last Endurance Race, we find that the vehicle started the race with a full fuel tank and stopped to refuel after.

To find work, we calculate it as W=Fdl and assuming that all force is used to propel the vehicle forward, it can be reduced to W = Fl. To find the length traveled during the consumption of one full fuel tank, we look at the fact that during the most recent endurance race, Cornell’s vehicle stopped to refuel after about 2.25 hours of the endurance race. Looking at the competition’s lap logs, at this time, Cornell had completed 41 laps of the track. Given that one lap of the track at this competition measured about 1.2 miles, we find that the approximate distance traveled by the car on one fuel tank was about 49.275 miles or 79300.4256 meters. 

To find the average force exerted on the car to move it forward, we perform a static calculation. Taking the coefficient of friction between the wheel and a dirt track to be approximately  = 0.4, the free body diagram for one of the wheels looks as below:

![Free body diagram — Baja wheel]({{ 'assets/images/fbd-baja-wheel.png' | relative_url }}){: class="project-image" }

Multiplying the result of the friction force by four wheels, we find that the total forward force necessary to move the car forward is 889.952N. 

Going back to the work calculation, we find that the work produced by the engine using up one fuel tank is approximately W=(889.952)(79300.4256)= 70.57 MJ. 

We can finally return to the efficiency calculation to find that the real life efficiency of the engine is approximately =70.57221.17= .319=31.9 %.

We find that, as would be expected, the actual efficiency is much lower than the ideal-air standard efficiency. This being said, it is more than obvious that this is not only the product of the real cycle not being ideal air (i.e., not an ideal gas but rather a fuel-air mixture, not isentropic, expansion as a result of combustion rather than heat transfer, etc.) but also due to other broader simplifying assumptions such as assuming only forward motion, assuming constant torque as average torque (when in reality the front and rear wheels produce different amounts of torque at all times and the torque varies between the transmission’s low and high-end ratios), and assuming perfect torque transmission between the wheels and ground (ignoring wheel slip and losses of energy to to friction, air resistance, etc.)
