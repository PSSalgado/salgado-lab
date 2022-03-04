---
title: "S-layer"
date: 2019-07-06T15:27:17+06:00
draft: false
# page title background image
bg_image: "images/backgrounds/page-title.jpg"
# meta description
description : "We are interested in the structure, assembly and function of the paracrystalline layer that covers *C. difficile* cells - the S-layer."
# Research image
image: "images/research/s-layer.png"
# type
type: "research"
---

Many bacteria and archaea possess a two-dimensional protein array, the S-layer, that covers the cell surface and plays crucial roles in cell physiology. In *C. difficile*, the S-layer has been implicated in colonisation and inflammation.

We have determined the structure and assembly of SlpA, the main S-layer component in *C. difficile*, which is post-translationally cleaved into two S-layer proteins (SLPs): the high molecular weight, SLP<sub>H</sub>, and low molecular weight, SLP<sub>L</sub>. These subunits then form a complex (H/L) that is incorporated in the S-layer.

Key findings in our Nature Communications paper (2022):


<div id="viewer" class="protein-viewer"></div>

<!-- Protein viewer -->
<script type='text/javascript' src='/js/bio-pv.min.js'></script>

<script type='text/javascript'>
var options = {
  width: 600,
  height: 500,
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

- SLP<sub>H</sub> forms a trimeric prism arrangement
- SLP<sub>L</sub> extends towards the environment
- The interacting domains form an intricate paper-clip motif that links the two SLPs
- Tiling of the SLP<sub>H</sub> creates the 2D array
- Interactions of SLP<sub>L</sub> cover the gaps between SLP<sub>H</sub> 
- SlpA forms a very tightly packed lattice, replicated in crystals and *in situ* S-layer reconstructions
- Electron diffraction of empty S-layer ghosts provides a map of the complete S-layer in the cells
-  The crystal structure of H/L complex mimics the organisation of the S-layer in the cells, providing a model for S-layer assembly in *C. difficile*.

![](/images/research/Slayer_structure.jpg)


We aim to continue to use a combination of structural, biochemical, biophysical and computational methods to further understand the role and dynamics of the S-layer.

&nbsp;

*Image by Lizah van der Aart*
