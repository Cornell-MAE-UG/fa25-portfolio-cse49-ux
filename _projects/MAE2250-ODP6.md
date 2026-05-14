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

**Team Name:** Lanternfly Bye-Bye

**Collaborators:** Gabriel Hwang, Owen LaPierre, Camille Eckert, Ryan Cruz, Claire Kim


**Clients:**  Cornell CALS Extension / E&J Gallo Winery 

---

## Table of Contents
1. [Introduction](#introduction)
2. [Client Pitch](#client-pitch)
3. [Functional Protytpe](#functional-prototype)
4. [Client Report](#client-report)
5. [Reflection](#reflection)

---

## Introduction
Spotted lanternflies (SLF) are invasive insects that feed on plants and agricultural crops. They cause significant damage to native ecosystems and the US agriculture industry. SLF have a one-year life cycle, with egg masses being laid during fall and hatching during the spring. Our goal for this project was to design a tool that aids local vineyards in managing SLF populations.

We ultimately decided to target SLF in their adult stage of life due to minimal knowledge of instar stages and challenges associated with targeting egg masses. Our primary goal was to design a system that would attract SLF and eliminate 75% of them within a 5-inch radius. 

---

## Client Pitch

#### Problem statement
Since 2014, spotted lanternflies (SLF) have permeated the northeast, feeding on produce such as grapes and infecting over 70 plant species, threatening agriculture and biodiversity. The economic impacts of this invasive species have been estimated at $324 million annually.

#### Impact
In 2025, the National Association of American Wineries valued New York’s wine industry at $16.81 billion. This high-value industry depends on a narrow 2-3 month harvest window, but the presence of spotted lanternflies can result in yield loss and reduced quality, costing the vineyards millions of dollars. 

#### Proposed direction
Our team has ideas for two products to either manage the lanternfly population or deter them from vineyards. However, each approach has its own potential and risks, so we would appreciate any feedback on the viability of our ideas. 

##### Concept A: Poisonous Tree of Heaven

**What it is:** Our first idea focuses on managing the population of spotted lanternflies using a decoy tree of heaven. Our team would design a small container and fill it with a mix of tree of heaven sap and a toxin.  
**How it would be used:** Attracted by the sap, the lanternflies will dig into the container and ingest the toxin. A brief search found that some have used milkweed to varying degrees of success. However, there is currently no research on its toxicity. Otherwise, the container can be equipped with a weight-activated nozzle that would douse the lanternflies in a toxic mix, similar to what many households currently use. 

**Potential:**  
- The decoys are easily scalable and stackable
- When placed in vineyards, will attract the flies away from the harvesters
- Is able to protect the harvesters from the bugs and work to reduce the fly population

##### Concept B: Essential Oils

**What it is:** Our second proposal attempts to prevent the spotted lanternflies from entering the vineyard by dettering them with essential oils.
**How it would be used:** These flies are naturally deterred by essential oils such as lavender or eucalyptus. By creating individual diffusers to place around the vineyard, the flies will not enter, and the plants will remain unharmed. Ideally, this idea could be developed to include a way to harm the lanternflies as well as deter them in order to help control the population and further protect the vineyard.

**Potential:**
- Non toxic to plants and other animals
- Does not require much maintenence
- Protects teh harvesters from the lanternflies

#### Key risks / unknowns

- Placement of the products is crucial. Because we are using a two-step solution, including attraction and detraction, we want to make sure we detract the flies into the attraction termination sites and not the other way around. Ideally we would conduct a study to see how far the scents travel and in what direction, but we do not have the budget nor time for that so we will have to rely on secondary research and data such as wind speed and direction.

- Location of egg masses. Because spotted lanternflies lay their eggs anywhere, we have to assume that there will already be SLF within the vineyard during spring. As a result, any product must have a way to deal with the starting population.

- Plant-safe compounds. Both of our proposed solutions involve liquid compounds to deter and remove lanternflies. The compounds used in the final solution will need to be safe for the grapes and approved by the FDA.

- Attracting SLF. A decoy would be most effective if it contained the sap or chemical signals that naturally draw SLF to the Tree of Heaven. This might be difficult to obtain and replace.



#### Questions for the client
1. Have you found anything that is effective at killing spotted lanternflies?
   *Decision affected: What component we add to reduce the population. For example, deciding between toxins or sprays and the concentration of them.* 
2. Are spotted lanternflies deterred by other factors such as locations of the vineyards or human presence? 
   *Decision affected: What location or factors should we examine when deciding how to implement out product* 
3. Are there any parts of our plans that raise conerns for you? 
   *Decision affected: Future Steps* 

#### References

- “New York Wine Industry - WineAmerica Economic Impact Study.” 2025. WineAmerica. WineAmerica Mobile. May 29, 2025. https://wineamerica.org/economic-impact-study-2025/new-york-wine-industry-2025/.

- “Spotted Lanternfly Reported Distribution Map.” 2017. CALS. 2017. https://cals.cornell.edu/integrated-pest-management/outreach-education/whats-bugging-you/spotted-lanternfly/spotted-lanternfly-reported-distribution-map.

- “Spotted Lanternfly in Perspective (U.S. National Park Service).” n.d. Www.nps.gov. https://www.nps.gov/articles/000/slf-in-perpective.htm.

[Back to top](#table-of-contents)

---

## Functional Prototype
#### Design Documentation

<table>

    <tr>

        <th>Description</th>

        <th>Specs</th>

        <th>McMaster Code</th>

        <th>Fabrication Details</th>

    </tr>

    <tr>

        <td>Casing Body</td>

        <td>7in diam x 8in H</td>

        <td>N/A</td>

        <td>3D printed in RPL with PLA</td>

    </tr>

    <tr>

        <td>Casing Lid</td>

        <td>7in diam x 7in H</td>

        <td>N/A</td>

        <td>3D printed in RPL with PLA</td>

    </tr>

    <tr>

        <td>Motion Sensors</td>

        <td>4x:2-6m sensing distance, 110° field of

            view, 1.25x1in </td>

        <td>8194N13</td>

        <td>Assembled with breadboard

            and coded</td>

    </tr>

    <tr>

        <td>Aerosol Sprayer</td>

        <td>2.5x7.25in, 8fl

capacity</td>

        <td>7773T4</td>

        <td>N/A</td>

    </tr>

    <tr>

        <td>Arduino Starter Kid</td>

        <td>16MHz processing

speed, ARM Cortex

A-9 CPU</td>

        <td>Amazon</td>

        <td>Assembled and coded</td>

    </tr>

    <tr>

        <td>Nozzle Straws</td>

        <td>19.7in length</td>

        <td>Amazon</td>

        <td>N/A</td>

    </tr>

    <tr>

        <td>Spray Bottle Straw

Attachment</td>

        <td>0.1in diam, 1.5in

length</td>

        <td>N/A</td>

        <td>3D printed in RPL with PLA</td>

    </tr>

</table>

<br>



####  Prototype Illustration:
<img src="{{ '/assets/images/Final_cad.jpg' | relative_url }}" alt="cad model exploded view" width="100%">

<img src="{{ '/assets/images/crosssection.jpg' | relative_url }}" alt="prototype cad no cap" width="100%">

<img src="{{ '/assets/images/prototype-cad-cap.jpg' | relative_url }}" alt="prototype cad cap" width="100%">
#### Prototype Assembly

1. Gently press the motion sensors into the holes in the lid. Thread the wiring through the
lid, ensuring connection is maintained between the sensors and the arduino.

2. Attach the bottle/nozzle connector to the spray bottle and the rest of the electronics in the center area of the base. Make sure that the arduino can rest on and activate the spray bottle.

3. Fill the outer area of the base with Tree of Heaven Sap or your preferred Spotted Lanternfly Bait

[Back to top](#table-of-contents)

---

## Client Report

#### Final Prototype and Application:
Our final design is a lightweight device that attracts SLF before immobilizing them with a combination of adhesives and a directed spray. It leverages sap from the Tree of Heaven as the attraction mechanism. Upon approach, the insects are detected by an infrared sensor, triggering an actuation mechanism that releases a spray of organic soap and water mixture, rapidly immobilizing the SLF without damaging nearby plants. The spray can be replaced as desired. Additionally, the outer housing contains adhesive flypaper that captures insects approaching from outside the effective range. 

The device was designed with the intent of being scalable. Individual units can be mounted to a variety of locations, and once mounted, are largely autonomous. While the prototype currently runs off disposable batteries, a final product would ideally run off solar power. Each unit provides approximately 180 degrees of coverage, but multiple units can be strategically arranged to maximize coverage and performance.

<img src="{{ '/assets/images/final-prototype-pic.jpg' | relative_url }}" alt="final prototype" width="100%">

<img src="{{ '/assets/images/cad-assembly.jpg' | relative_url }}" alt="cad assembly" width="100%">

<img src="{{ '/assets/images/final-section-view.jpg' | relative_url }}" alt="final prototype section view" width="100%">

#### Testing and Results:
To evaluate our prototype’s performance, we tested the spray range, IR sensor detection range, and strength of the adhesive paper. 

We assessed the IR sensor performance by measuring the detection rate as a function of angle. Experimental observations showed an effective FOV of approximately 120–140 degrees, with accuracy decreasing towards the edges. As a result, we included two sensors into the design to increase reliability.

Finally, we tested the adhesive paper to determine its strength. Our results show that the flypaper is easily capable of retaining a lanternfly-sized object. The adhesive remained effective under moderate loading conditions, though overcrowding reduced marginal capture efficiency due to decreased sticking area. Overall, the flypaper is robust, reliably capturing insects missed by the spray.

At the system level, overall efficiency was evaluated by introducing a controlled number of objects and recording the proportion successfully detected and immobilized. The prototype achieved an average effectiveness of approximately 75% within the intended operating region, achieving our target specified in the problem statement. This discrepancy was primarily attributed to the limited spray radius and partial sensor coverage, which allowed some targets to pass through undetected or unsprayed.

<img src="{{ '/assets/images/sensor-graph.jpg' | relative_url }}" alt="sensor graph" width="100%">

<img src="{{ '/assets/images/flypaper-graph.jpg' | relative_url }}" alt="flypaper graph" width="100%">

#### Prototype Details: 
Our initial full-scale functional prototype was designed as a branch-mounted, modular trapping system intended to provide 360° coverage of the surrounding area.

<img src="{{ '/assets/images/prototype-cad.jpg' | relative_url }}" alt="prototype cad" width="100%">

A central feature of this design was a custom four-way nozzle intended to distribute spray evenly in all directions. This configuration was selected to improve the likelihood of SLF contact regardless of approach angle. However, during implementation, compatibility issues were identified between the custom nozzle design and the commercially available spray canisters, specifically related to pressure delivery and nozzle interface geometry. These constraints prevented the successful integration of the multi-directional spray system in the current iteration.

<img src="{{ '/assets/images/prototype-cad-no-cap.jpg' | relative_url }}" alt="prototype cad no cap" width="100%">

Despite these challenges, further investigation into alternative nozzle geometries, pressurized delivery systems, and adapter mechanisms suggests that a fully functional 360-degree spray configuration remains technically feasible. With appropriate redesign of the pressure regulation and nozzle coupling system, the original concept could be realized in a future iteration of the prototype, potentially improving overall capture efficiency and reducing reliance on auxiliary trapping components.

#### Conclusion and Recommendation: 
After spending the semester designing and testing our system, we believe that our prototype has potential, but would benefit from further refinement. The primary limitation is the spraying mechanism, as our initial design specified a system capable of distributing fluid through multiple nozzles. Due to our time constraints, we chose to alter our housing to work with our original spraying mechanism, which can achieve a radius of about 10 inches. While this configuration could potentially work, the limitations of the spray required the addition of adhesive surfaces to achieve our desired efficiency. Further developments should prioritize a pressurized delivery system combined with multiple nozzles to enable 360-degree coverage.

<img src="{{ '/assets/images/poster.jpg' | relative_url }}" alt="poster" width="100%">

#### Bill of Materials:

<img src="{{ '/assets/images/bill-of-materials.png' | relative_url }}" alt="bill of materials" width="100%">


[Back to top](#table-of-contents)

---

## Reflection


[Back to top](#table-of-contents)