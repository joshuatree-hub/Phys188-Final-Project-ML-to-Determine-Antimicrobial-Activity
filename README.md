# Physics 188 Final Project  
## Atomic-to-Peptide Hierarchical Graph Neural Network

This project implements a hierarchical Graph Neural Network (GNN) to predict peptide-level antimicrobial activity directly from molecular structure. The model integrates an atomic-level GNN—where atoms are represented as nodes and covalent bonds as edges—with an amino acid–level GNN, in which amino acids form nodes connected along the peptide sequence, using a GraphSAGE. Collaborated in a group of six, the approach synthesizes and reproduces recent methodologies in peptide property prediction to classify peptides as antimicrobial or non-antimicrobial.

## File Structure

- phys188_final_project_atomic_to_peptide_gnn.ipynb             # contains the two GNNS and predictions, along with application to a bioengineered peptide chain at the end
- README.md                                                     # this file, explaining what's what
- requirements.txt                                              # all imports needed for to run the ipynb in totality
- data/                                                         # data collected from out cited research papers
  - Train_clean.csv                                             # peptide sequence and data on whether they are or aren't antimicrobial (amp) to TRAIN peptide gnn
  - Test_clean.csv                                              # peptide sequence and data on whether they are or aren't antimicrobial (amp) to TEST peptide gnn
  - aaindexc/                                                   # an index of non-cannonical amino acids used in the atomic gnn
     - ncAAs/  
     - quality/  
     - models/  

## Other comments to grader

- Note the code will take ~10 minutes to run. 
- We work with molecules, an import you need is rdkit which for this physics class you may not have. For your convenience: 
 - pip install -r requirements.txt

