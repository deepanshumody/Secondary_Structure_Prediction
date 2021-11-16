# Protein structure prediction using RNN
## Introduction
Protein structure prediction is one of the most important problems in bioinformatics and theoretical chemistry. On 30 November 2020, it was announced by the alphafold team at google deepmind that the problem of protein structure prediction has been "solved" by achieving an accuracy of greater than 90% in predicting the protein structure. This project aims to predict the structure of proteins based on the protein's amino acid residues and evolutionary data obtained from PSI-Blast and HHBlits in the form of multiple sequence alignments.
The two ways to classify a protein in terms of secondary structure are 3-state and 8-state predictions.

For 3 state prediction the goal is to classify them into the following.
```
E = extended strand, participates in β ladder
H = α-helix
C = coil (residues which are not in any of the above conformations)
```

For 8 state prediction the goal is to classify them into the following
```
E = extended strand, participates in β ladder
B = residue in isolated β-bridge
H = α-helix
G = 3-helix (3-10 helix)
I = 5-helix (π-helix)
T = hydrogen bonded turn
S = bend
_ = loop (any other type)
```
For the scope of this project, the 3 state prediction has been chosen.

## Dataset
Porter5 dataset has been used for the above, which consists of 24 features for each amino acid residue in the protein.
