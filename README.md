# Vaccine-Modelling (River blindness)
## Onchocerciais Vaccine Candidate Repo

Comparative modelling and docking analysis comparing Toll-like receptor-4 (TLR4)immune recognition affinity for Ov-FUS-1 with Ov-103+Ov-RAL-2 (given together) 

         Protein sequence:
Fus-1 is a fusion of the open reading frame encoding the Onchocerca volvulus larval protein, Ov-103, 
a glycinyl/serinyl linker domain, followed by the O. volvulus
immunodominant hypodermal antigen, Ov-RAL-2. Ov-103 (GenBank: AAA63412.2) is a 158 aa
surface-associated protein on O. volvulus microfilaria first identified in 1992 but later it was
revealed that it is also expressed by other stages of the parasite including L3s. The Ov-103
segment in Fus-1 is 100% conserved with proteins from related parasitic pathogens including
Brugia malayi, Wuchereria bancrofti, Loa Loa, and other related filarial parasites. Ov-RAL-2
(GenBank: ACB70199.1), a 164 aa protein, is a rainforest immunodominant hypodermal antigen
present in both adult and juvenile O. volvulus worms first identified in 1992. Although it is a
family member of the SXP protein family, the Ov-RAL-2 sequence in Fus-1 is only found in O.
volvulus and the closely related species O. ochengi. Neither Ov-103 nor Ov-RAL-2 exhibit any
significant amino acid homology with any known proteins from humans. 
        
        The amino acid sequence of Fus-1 is as follows:
1 DLLSEAGDFF TKHFTDIKSL FAKDEKQLQQ SVDRVKDLLA TIQDKMSMLQ PLANDMQKTT 60
61 LGKIGDLISQ VNSFRETMSN PKMDFTNKEN KWEELLKKIF VTEGLNKVIP LLQKLKNSAG 120
121 GGGSGGGGSG GGGSPQRRQQ QQQQQQQQQR DEREIPPFLE GAPPSVIDEF YNLLKTDENK 180
181 TDQQTEADVE AFINRLGGSY KVRFTQFMEE VKKARADYER IHQQAVARFS PAAKDADARM 240
241 SAIADSPHLT TRQKSQQIQA IMDSLSESVR REIINALSPQ E

         Simple seq stretch:

""DLLSEAGDFFTKHFTDIKSLFAKDEKQLQQSVDRVKDLLATIQDKMSMLQPLANDMQKTTLGKIGDLISQVNSFRETMSNPKMDFTNKENKWEELLKKIFVTEGLNKVIP 
LLQKLKNSAGGGGSGGGGSGGGGSPQRRQQQQQQQQQQQRDEREIPPFLEGAPPSVIDEFYNLLKTDENKTDQQTEADVEAFINRLGGSYKVRFTQFMEEVKKARADYER 
IHQQAVARFSPAAKDADARMSAIADSPHLTTRQKSQQIQAIMDSLSESVRREIINALSPQE"

        Peptide sequence of OV-FUS-1:
The Ov-103 portion is highlighted in blue, the linker domain is in red, and the Ov-RAL-2 domain 
is in green. The sequence has GGGGSX3 times vs. GGGSX3 times.
Ov-FUS-1 Recombinant Protein: Ov-Fus-1 is a recombinant protein of 279 amino acids. It is
produced in P. pastoris with a predicted molecular weight of 31510.49 and an observed
molecular weight of 32 kDa on reducing 4-20% Tris-glycine SDSPAGE. The “Fus-1” stands for
the Fusion of the two proteins Ov-103 and Ov-RAL-2 with Ov-103 as the N-terminal protein. The
two proteins are separated by a flexible, 12 amino acid glycine-serine linker
(GGGSGGGSGGGS). In the context of onchocerciasis, we refer to this protein simply as Ov-
FUS-1.

         Molecular model of the Fus-1 protein. 

To understand potential mechanisms of humoral inhibition of Fus-1 activity 
and to look at surface charge distribution profiles when selecting chromatographic 
matrices, a model of Fus-1 was built using the Google Colab version of Alphafold. 
The model shows largely alpha helical domains for the Ov-103 (blue), the
disordered linker (red) and the alpha helical Ov-RAL-2 (green).


         Independent Ov-103 and Ov-RAL-2 sequences:
>Ovo-MSA-1 Ov-103(Wormbase ID: WBGene00241039)
MLKYGILLMLITVGAYCDLLSEAGDFFTKHFTDIKSLFAKDEKQLQQSVDRVKDLLATIQDKMSMLQPLANDMQKTTLGK
IGDLISQVNSFRETMSNPKMDFTNKENKWEELLKKIFVTEGLNKVIPLLQKLKNSAPTTFATYLFTCIVPVLINTLRE
        
>OVOC9988 Ov-RAL-2(WormBase ID:WBGene00246797)
MKFVILLTIGLLVVAAIPQRRQQQQQQQQQQQRDEREIPPFLEGAPPSVIDEFYNLLKTDENKTDQQTEADVEAFINRLG
GSYKVRFTQFMEEVKKARADYERIHQQAVARFSPAAKDADARMSAIADSPHLTTRQKSQQIQAIMDSLSESVRREIINAL
SPQE


## Our Approach
The focus was on predicting and analyzing the 3D structures of Ov-FUS-1 and Ov-103 + Ov-RAL-2 vaccine candidates, 
as well as their interaction with the human TLR4 receptor. The key steps:

### Structure Prediction:
AlphaFold2 via ColabFold v.1.5.5 was used to predict high-resolution 3D structures.
Ov-FUS-1 was modelled as a single unit, while Ov-103 and Ov-RAL-2 were modelled as a complex.
Five models were generated for each protein, with the best model selected based on pLDDT and pTM scores.
### TLR4 Structure Preparation:
A 2.40 Å resolution structure of human TLR4 (PDB ID 3FXI) was obtained from the Protein Data Bank.
The structure was cleaned and prepared using Molecular Operating Environment (MOE) software.
### Structure Optimization:
All models underwent protonation and energy minimization to optimize atomic positions, bond geometries, and torsion angles.
### Molecular Docking:
The HADDOCK server was used to characterize binding affinity between vaccine candidates and TLR4.
Previously identified critical residues of TLR4 (R264, K341, K362, K388, F440, L444, F463, Q436) were used to specify the binding region.
The HADDOCK algorithm docked each vaccine antigen to these binding site residues.
### Molecular Dynamics Simulation:
Resulting structures underwent MD simulation with a gentle refinement in TIP3P water molecules.
Simulation parameters included 5000 steps at 300 K with position restraints, followed by cooling stages.
Energies were computed using electrostatic and van der Waals terms with OPLS nonbonded parameters.
### Analysis and Visualization:
Top-ranked low energy docked vaccine-TLR4 complexes were grouped based on fraction of common contacts and pairwise backbone RMSD.
Structural analyses and visualization were performed using PyMOL Molecular Graphics System.

## Results Summary

 Key findings include:

1. Structural Modeling:
   - AlphaFold2 successfully predicted 3D structures for both vaccine candidates.
   - Ov-FUS-1 achieved a high confidence score (pLDDT = 86.5%).
   - Ov-103 + Ov-RAL-2 complex scored moderate confidence (pLDDT = 63.3%, ipTM = 0.23).
   - Both models showed low predicted aligned error (PAE < 5Å) and good sequence depth.

2. Molecular Docking:
   - HADDOCK platform effectively produced docked complexes for both candidates with TLR4.
   - OvFUS1-TLR4 complexes were categorized into 19 clusters.
   - Ov103OvRAL2-TLR4 complexes were categorized into 5 clusters.

3. Binding Affinity:
   - Ov-FUS-1 showed stronger binding affinity to TLR4 compared to Ov-103 + Ov-RAL-2 complex.
   - OvFUS1-TLR4 top cluster:
     * Binding affinity: -316.28 Kcal/mol
     * HADDOCK score: -93.7 +/- 11.2 Kcal/mol
     * Cluster size: 10 complexes
     * Z-score: -1.2
   - Ov103OvRAL2-TLR4 top cluster:
     * Binding affinity: -234.96 Kcal/mol
     * HADDOCK score: -42.5 +/- 0.4 Kcal/mol
     * Cluster size: 2 complexes
     * Z-score: -1.5

4. Structural Examination:
   - OvFUS1-TLR4 complex exhibited more hydrogen bonds at the interaction interface.
   - Ov-FUS-1 established conserved interactions with TLR4 receptor key active residue K388 and passive residues G363, K388, E439, and R460.
   - K388 formed a significant interface hotspot with Q149 and E152 of Ov-FUS-1.
   - The G/S linker peptide in Ov-FUS-1 contributed to a flexible conformational structure, potentially enhancing receptor recognition.

### In conclusion, Ov-FUS-1 demonstrated higher binding affinity and more favorable interactions with the TLR4 receptor compared to the Ov-103 + Ov-RAL-2 complex. 
## This suggests that Ov-FUS-1 may be a more effective vaccine candidate in terms of innate immune system activation via TLR4 signaling.
