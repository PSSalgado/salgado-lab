---
title: "It's finally out!"
date: 2022-02-24T10:11:17+06:00
draft: false
# page title background image
bg_image: "images/backgrounds/page-title.jpg"
# meta description
description : "Behind the BugS-layer paper"
# post thumbnail
image: "/images/research/s-layer.png"
# post author
author: "Paula Salgado"
# type
type: "post"
---

## Behind the BugS-layer paper 


It's finally out! Our work describing the structure and assembly of the S-layer in *C. difficile* is published today in [Nature Communications](https://www.nature.com/articles/s41467-022-28196-w). 

<div id="viewer" class="protein-viewer"></div>

<!-- Protein viewer -->
<script type='text/javascript' src='/js/bio-pv.min.js'></script>

<script type='text/javascript'>
var options = {
  width: 400,
  height: 300,
  antialias: true,
  quality : 'medium'
};
var viewer = pv.Viewer(document.getElementById('viewer'), options);

function loadPDB() {
  pv.io.fetchPdb('/pdbs/CD630HL_final.pdb', function(structure) {
      viewer.cartoon('protein', structure, { color : color.byChain() });
      viewer.autoZoom();
      viewer.centerOn(structure);
      
  });
}
document.addEventListener('DOMContentLoaded', loadPDB);
</script>

You can find out the key scientific findings  [here](/research/s-layer/). 

Instead, I'd like to tell you about the journey to get to today.

This has been the longest project I worked on. I set up my first SlpA crystal trays back in 2011, when working in Neil Fairweather's lab at Imperial College. Soon after, me and Rob Fagan were testing them at Diamond Light Source. The road has been hard, bumpy but we got there.

I was recently asked why it took so long to solve the structure. I've also been asked why I kept working on this problem when it didn't seem to go anywhere. The answer to both is "*because it was difficult, but not impossible*". 

The main difficulty is that S-layer proteins like to make crystals - but only in two dimensions, like a sheet of ordered pieces, a mosaic. Getting those sheets to stack in regular pattern to make the 3D crystals we need for X-ray crystallography was the problem. I got crystals, but they were far from perfect, even when they looked good.
 
![SlpA crystal](/images/blog/xtalSlpa2.png)

When we shot them with X-rays, we'd get a reasonable pattern in one direction, but poor resolution in another. And there was no way to know without testing. So I spent many, many hours, mostly at night, at Diamond Light Source, testing crystal after crystal, doing scans to find the sweet spot of good diffraction.

![DLS data collection](/images/blog/datacollection2016.jpeg)

I also spent time trying to optimise the crystals, of course! I've lost count of how many drops were prepared and observed under the microscope, several thousands, I would guess. 

Even with a reasonable dataset, we still couldn't solve it. The partial models were not enough for molecular replacement solutions. When me and Rob tried the next thing on a protein crystallographer's kit by replacing sulphur atoms with selenium in the protein, the whole lab ended up having to be checked by Occupatinal Health! We found out in these conditions, *C. difficile* makes dangerous componds! Maybe we'll tell that story and how we ended up making charcoal "sausages" some other time.

For years, as I set up my lab in Newcastle, the project was running in the background, as we focused on other aspects of *C. difficile* pathogenecity. Occasionally, I would have a new idea or hear of a recent new method and have a burst of activity, trying to get better crystals or use other ways to solve it.  Many such ideas came from CCP4 Study Weeekends, sitting at the banquet table with one of the Diamond Light Source (DLS) beamline scientists and chatting about this really difficult protein I was working on. Without such an amazing collaboration with MX staff, who always welcomed my ideas and were keen to try and push the technical boundaries together, we wouldn't have solved it. Even my ambitious idea of doing high throughput heavy atom screening was embraced and facilitated! A huge thank you to all of them! 

![High throughput](/images/blog/HAhighthroughput.jpeg)

A key experiment was collecting data on I23, using the anomalous signal from sulphur, combined with available partial models, to have first phases - a huge thank you to Kamel El Omari from DLS for the mamoth effort in building this! However, it still wasn't enough - we couldn't build a complete model...

I kept pushing it as I knew this was possible - there was enough information there for the structure to be solved. 

And then Rob got an S-layer mutant strain - for the first time ever, we could see what happened when there was no armour! We got together with Gill Douce and secured a Wellcome Trust Collaborative Award to study the structure and function of the S-layer in *C. difficile*. This meant I finally got more hands on deck to crack the puzzle - Anna Barwinska-Sendra as a postdoc and Paola Lanzoni-Mangutchi as a PhD student joined the lab and the quest for the SlpA structure! They joined forces, shared experiences, data and worked on the technical challenges together while I was away, focusing on my other project - my newborn son.

Fast forward to September 2018. We had spent a year trying a different strategy: divide and conquer, crystallising subdomains of SlpA and mutated versions of the protein. We organised a trip to I24 - the three of us in my car, driving down to DLS with a dewar full of hope. It was a long night but that's when we get the datasets that will eventually allow us to build a full model. At 5am, as we come out of the beamline, we knew this had been a good data collection. We were exhausted, but happy. Mission acomplished. 

![night shift at DLS](/images/blog/data_collection_all.jpeg)

It took another 2 years to complete all the models. And just as we were writing the first drafts of the manuscript, COVID-19 struck. Writing a paper at a distance, during a lockdown, with a toddler running around, was yet another hard obstacle in our path. But we got there, supporting each other throught the difficult moments.

Thank you to the whole BugS-layer team. And thank you, Neil, for introducing me to this fascinating problem! And thank you especially to Anna and Paola! 

It was difficult, but I always knew it was possible. I just needed the help of an amazing team to get there. 