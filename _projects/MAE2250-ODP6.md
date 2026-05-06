---
layout: project
title: MAE 2250 - Exhibit Client Report
description: Class Assignment
image: /assets/images/spotted_lanternfly4.jpg
fontsize: 11pt
geometry: margin=1in
papersize: letter
pagestyle: empty
group: group1
---
**Team:** _Sinicus_
<br>
Camille Eckert, Claire Kim, Ryan Cruz, Owen Lapierre, Gabriel Hwang


## Context and Problem Statement
Spotted lanternflies (SLF) are invasive insects that feed on plants and agricultural crops. They cause significant damage to native ecosystems and the US agriculture industry. SLF have a one-year life cycle, with egg masses being laid during fall and hatching during the spring. Our goal for this project was to design a tool that aids local vineyards in managing SLF populations. We ultimately decided to target SLF in their adult stage of life due to minimal knowledge of instar stages and challenges associated with targeting egg masses. Our primary goal was to design a system that would attract SLF and eliminate 75% of them within a 5-inch radius. 


## Final Prototype and Application
Our final design is a lightweight device that attracts SLF before immobilizing them with a combination of adhesives and a directed spray. It leverages sap from the Tree of Heaven as the attraction mechanism. Upon approach, the insects are detected by an infrared sensor, triggering an actuation mechanism that releases a spray of organic soap and water mixture, rapidly immobilizing the SLF without damaging nearby plants. The spray can be replaced as desired. Additionally, the outer housing contains adhesive flypaper that captures insects approaching from outside the effective range. The device was designed with the intent of being scalable. Individual units can be mounted to a variety of locations, and once mounted, are largely autonomous. While the prototype currently runs off disposable batteries, a final product would ideally run off solar power. Each unit provides approximately 180 degrees of coverage, but multiple units can be strategically arranged to maximize coverage and performance.


<div style="text-align: center;">
  <img src="{{ '/assets/images/Final_prototype.png' | relative_url }}" alt="Centered Image" style="max-width:100%; height:auto;">
</div>
<center> Fig 1. Assembled Final Prototype </center>
<br>


<div style="text-align: center;">
  <img src="{{ '/assets/images/Final_cad.png' | relative_url }}" alt="Centered Image" style="max-width:100%; height:auto;">
</div>
<center> Fig 2a. Final Cad design </center>
<br>


<div style="text-align: center;">
  <img src="{{ '/assets/images/crosssection.png' | relative_url }}" alt="Centered Image" style="max-width:100%; height:auto;">
</div>
<center> Fig 2b. Crosssection of Final Cad </center>
<br>




## Conclusion and Recommendations
<p>After spending the semester designing and testing our system, we believe that our prototype has potential, but would benefit from further refinement. The primary limitation is the spraying mechanism, as our initial design specified a system capable of distributing fluid through multiple nozzles. Due to our time constraints, we chose to alter our housing to work with our original spraying mechanism, which can achieve a radius of about 10 inches. While this configuration could potentially work, the limitations of the spray required the addition of adhesive surfaces to achieve our desired efficiency. Further developments should prioritize a pressurized delivery system combined with multiple nozzles to enable 360-degree coverage. </p>


## Testing and Results
To evaluate our prototype’s performance, we tested the spray range, IR sensor detection range, and strength of the adhesive paper. 


<div style="text-align: center;">
  <img src="{{ '/assets/images/detection.png' | relative_url }}" alt="Centered Image" style="max-width:100%; height:auto;">
</div>
<center>Fig 2. IR Sensor Detection Rate vs. Angle 1</center>
<br>
We assessed the IR sensor performance by measuring the detection rate as a function of angle. Experimental observations showed an effective FOV of approximately 120–140 degrees, with accuracy decreasing towards the edges. As a result, we included two sensors into the design to increase reliability.


<div style="text-align: center;">
  <img src="{{ '/assets/images/flypaper.png' | relative_url }}" alt="Centered Image" style="max-width:100%; height:auto;">
</div>
<center>Fig 3. Effectivenes of Fly Paper for Varying Weight 2</center>
<br>

Finally, we tested the adhesive paper to determine its strength. Our results show that the flypaper is easily capable of retaining a lanternfly-sized object. The adhesive remained effective under moderate loading conditions, though overcrowding reduced marginal capture efficiency due to decreased sticking area. Overall, the flypaper is robust, reliably capturing insects missed by the spray.



<p>At the system level, overall efficiency was evaluated by introducing a controlled number of objects and recording the proportion successfully detected and immobilized. The prototype achieved an average effectiveness of approximately 75% within the intended operating region, achieving our target specified in the problem statement. This discrepancy was primarily attributed to the limited spray radius and partial sensor coverage, which allowed some targets to pass through undetected or unsprayed.</p>



## Prototype Details
Our initial full-scale functional prototype was designed as a branch-mounted, modular trapping system intended to provide 360° coverage of the surrounding area.

<div style="text-align: center;">
  <img src="{{ '/assets/images/prototype.png' | relative_url }}" alt="Centered Image" style="max-width:100%; height:auto;">
</div>
<center>Fig 4. Initial Prototype </center>
<br>

### _Rake test_
<p>A central feature of this design was a custom four-way nozzle intended to distribute spray evenly in all directions. This configuration was selected to improve the likelihood of SLF contact regardless of approach angle. However, during implementation, compatibility issues were identified between the custom nozzle design and the commercially available spray canisters, specifically related to pressure delivery and nozzle interface geometry. These constraints prevented the successful integration of the multi-directional spray system in the current iteration.</p>
<p>Despite these challenges, further investigation into alternative nozzle geometries, pressurized delivery systems, and adapter mechanisms suggests that a fully functional 360-degree spray configuration remains technically feasible. With appropriate redesign of the pressure regulation and nozzle coupling system, the original concept could be realized in a future iteration of the prototype, potentially improving overall capture efficiency and reducing reliance on auxiliary trapping components.</p>

## Appendix A: Bill of Materials


<table>
    <tr>
        <th>Component</th>
        <th>Material/Part</th>
        <th>Quantity</th>
        <th>Price</th>
    </tr>
    <tr>
        <td>Prototype Casing</td>
        <td>Rapid Prototyping Lab PLA</td>
        <td>1/td>
        <td>$43.98</td>
    </tr>
    <tr>
        <td>Final Casing</td>
        <td>Rapid Prototyping Lab PLA</td>
        <td>1</td>
        <td>$82.80</td>
    </tr>
    <tr>
        <td>Ultrasonic Sensors</td>
        <td>McMaster product</td>
        <td>4</td>
        <td>$56.84</td>
    </tr>
    <tr>
        <td>Aerosol Sprayer</td>
        <td>McMaster product</td>
        <td>1</td>
        <td>$15.40</td>
    </tr>
    <tr>
        <td>Arduino Starter Kid</td>
        <td>Amazon product</td>
        <td>1</td>
        <td>$44.99</td>
    </tr>
    <tr>
        <td>Nozzle Straws</td>
        <td>Amazon Product</td>
        <td>1</td>
        <td>$6.99</td>
    </tr>
    <tr>
        <td>Fly Paper</td>
        <td>McMaster product</td>
        <td>1</td>
        <td>$22.49</td>
    </tr>
</table>
<br>

