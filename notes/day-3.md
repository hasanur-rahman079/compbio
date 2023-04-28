# Protein Modeling

## AlphaFold Colab

A hitchhiker's guide to protein structure modeling

why moduling
Crystallography, NMR

</br>

## Cryoem (Cryogenic electron microscopy) is the most popular to solve protein structure

</br>

## Protein modeling

1. Template Based Modeling TBM (Homology) (I-TASSER),
2. Template free modeling FM (MD Simulation, [Rosetta](https://www.rosettacommons.org/) [powerful tools, must learn])

</br>

## Multiple siquence allignment MSA

</br>

## Critical assessment of structure prediction [CASP](https://predictioncenter.org/)

</br>

## Direct coupling analysis

[Alphafold2](https://alphafold.ebi.ac.uk/) - pLDDT
IDDT:
the pLDDT score will give the accuracy the modeling
predicted align error
AF2 can calculate the protein protein interactions accourtely

</br>

## Pickup local problems and collaborations

Purpose: to reduce the phage

## Equilibration

step-4_equilibration.dcd (ions, water)
step-5 = final analysis (productions)

## Analysis of MD

In this step there will be

1. Temo, Tempreatue is no defined at atomic system.
2. Energy. If the Potential energy and kinetic energy is decreadsing then the simulaiton is right.

### RMSD (Average over the resuidues, How do you check the protein is stable?)

= RMSD (equation), for every time frame, there will be a RMSD value. We have to use a reference structure either time steps from others. there will be never a rmsd valuu 0. if the line is stable after a timeframe and be stable then the simulaiton is valid, but if the curve is keep increasing then there have some biological issue or other technical errors. 8 A is really bad but 4 is not bad.

The goal is to make as close as possible to the goal.

### RMSF (Fluctions of residues)

= all the snapshots can read together. Residues in X axis,alpha and beta helical is not move much (1 A). This is the protein mutaion by analysis the higher flactions in the residues.

### How do you find the mutations.

= We can take a wild card residues of proteins and take the experimental one and compare the RMSF of those residues

### H bond (Master of Biology ):, Fluctions of residues)

= counting the donar and acceptior distance. H bond reduced then there will be the mutations and if it increased then the simulaiton is ok.

</br>

### Ramachandra plot (how much the bonds corated and their ploting)

=

</br>

## Words

1. superimpose

[Overleaf](https://www.overleaf.com/)
