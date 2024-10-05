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
IHQQAVARFSPAAKDADARMSAIADSPHLTTRQKSQQIQAIMDSLSESVRREIINALSPQE""

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
