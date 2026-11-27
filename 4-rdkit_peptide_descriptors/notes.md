04: Automated Physicochemical Descriptor Calculation & 2D Structure Rendering with RDKit

Overview
Used Python and RDKit in Google Colab to automate molecular descriptor calculations (Molecular Weight, cLogP, TPSA, H-bond donors/acceptors)
and 2D structure visualization comparing the native GLP-1 N-terminal tripeptide (His7-Ala8-Glu9), Semaglutide's DPP-4-resistant N-terminal motif (His7-Aib8-Glu9), 
and the oral non-peptide GLP-1R agonist Danuglipron.

Computed RDKit Descriptors
- Native_GLP1_Nterm (His-Ala-Glu): MW = 355.35 Da, cLogP = -1.78, TPSA = 187.50 A^2, HBD = 6, HBA = 6
- Semaglutide_Nterm (His-Aib-Glu): MW = 369.38 Da, cLogP = -1.39, TPSA = 187.50 A^2, HBD = 6, HBA = 6
- Danuglipron (Oral Small Molecule): MW = 505.59 Da, cLogP = 4.80, TPSA = 85.41 A^2, HBD = 1, HBA = 5

Medicinal Chemistry Takeaways
1. Steric Shielding at Position 8 (Ala8 to Aib8): Replacing the alpha-hydrogen of Alanine-8 with a second methyl group (aminoisobutyric acid, Aib) increases molecular
weight by 14.03 Da and slightly increases lipophilicity (cLogP from -1.78 to -1.39) without altering TPSA (187.50 A^2). This gem-dimethyl group sterically blocks
dipeptidyl peptidase-4 (DPP-4) hydrolysis while inducing alpha-helical conformation.

2. Oral Permeability Contrast: Even a 3-residue peptide fragment exceeds Veber's oral TPSA threshold (187.50 A^2 > 140 A^2) with 6 H-bond donors,
whereas Danuglipron maintains low TPSA (85.41 A^2), 1 H-bond donor, and positive cLogP (4.80) for passive transcellular absorption.
