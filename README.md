# Pareto-Archetypal-Analysis-PBMCS-Covid-19

Pareto Archetypal Analysis on Peripheral Mononuclear Blood Cells from Infected Covid-19 Patients
Sars-Cov-2 not only has been shown to damage the respiratory tract and lung tissues, but it has a substantial effect on neurological pathologies,
the cardiovascular system and thrombotic effects throughout different organs particularly organs with high abundance of ACE2 receptors. 
This strongly suggests the virus can move past the lungs and has a role within the endothelial cell linings of the blood vessels. 
Mechanisms behind the virus's invasive properties and ability to cause blood vessel and brain damage is explored to determine proteins 
that can be considered for drug targets to mitigate virus spread.

Archetypal analysis is an unsupervised learning method to identify archetypes or extreme points in multidimensional data. 
The archetypes are put on a Pareto front, that is, no state can be made better without making one worse(Pareto optimality) 
where these arcs are contained within an efficient representation of a polytope using the principal convex hull algorithm. 
In a biological context, archetypes found in gene expression data may indicate highly expressed genes, that is, certain tradeoffs 
are made within cell and genes to achieve an optimal biological function determined by the archetype.

Here, I implement a Pareto Archetypal Analysis using R's ParetoTI package to find key biological processes or archetypes within peripheral 
blood mononuclear cells(PBMC) of infected Covid-19 Patients. I use Python's gseapy package to perform a gene set enrichment analysis at each 
archetype, and observe protein-protein interactions(PPI) at each archetype using STRING. Another Archetypal Analysis is done on CD4 T cells 
determined to be the cell type closest to the specific archetype of interest along with a GSEA and PPI network analysis.

Single-cell metadata of PBMCs taken from the Human Covid-19 Cell Atlas.
