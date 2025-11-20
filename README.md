# CONSTRUCTING-A-PHYLOGENETIC-TREE-of-INSULIN-USING-EMBL-EBI-MUSCLE-TOOL
CONSTRUCTING-A-PHYLOGENETIC-TREE-of-INSULIN-USING EMBL EBI MUSCLE-TOOL
💉 Insulin Chain Phylogenetic Analysis (MUSCLE)

This repository contains the results of a multiple sequence alignment (MSA) and phylogenetic analysis for a set of Insulin A and B chains, performed using the EMBL-EBI MUSCLE (Multiple Sequence Comparison by Log-Expectation) tool. This analysis is crucial for understanding the conservation and evolutionary divergence within the Insulin protein across different species and PDB structures.

📁 Repository Contents
Filename,Description,Source
muscle-I20250718-071908-0115-39479710-p1m.sequence,"Input FASTA File containing 10 Insulin A and B chain protein sequences, including species information.",Input
muscle-I20250718-071908-0115-39479710-p1m.aln-clustalw,"Multiple Sequence Alignment (MSA) output in CLUSTALW format, showing aligned residues and conservation.",Output
muscle-I20250718-071908-0115-39479710-p1m.pim,"Percent Identity Matrix (PIM), detailing all pairwise sequence similarities.",Output
muscle-I20250718-071908-0115-39479710-p1m.phylotree,"Newick format of the Phylogenetic Tree (Guide Tree), detailing branch lengths.",Output
INSULIN PHYLOGENETIC TREE PHYLOGRAM MUSCLE TOOL.png,Graphical representation of the Phylogenetic Tree (Phylogram) .,Output
🧬 Alignment and Conservation

The analysis confirms the expected high conservation of mammalian Insulins and highlights the significant divergence of cone snail Insulin.

1. Sequence Conservation (Mammalian vs. Cone Snail)

The data separates the sequences into highly conserved groups based on chain type (A or B) and divergence based on species (Mammalian vs. Mollusk):

    Mammalian Insulin B Chains (3I40_2, 4E7U_2, 1ZNI_2, 4INS_2): These sequences (from Homo sapiens, Bos taurus, and Sus scrofa) are 100% identical to each other in the aligned region.
    Mammalian Insulin A Chains (3I40_1, 1ZNI_1, 4INS_1): These three chains are also 100% identical.
    Divergent Insulin Chains (5JYQ_1, 5JYQ_2): The Insulin chains from Conus geographus (cone snail) are highly divergent from the mammalian chains, showing only ≈20% pairwise identity with the mammalian A/B chains
    2. Key Species Information (from Input FASTA)
    PDB ID,Chain Type,Species,PDB Details
3I40,"A, B",Homo sapiens (Human),"Insulin A chain, Insulin B chain"
4E7U,"A, B",Bos taurus (Cattle),"Insulin A chain, Insulin B chain"
1ZNI / 4INS,"A, B",Sus scrofa (Pig),INSULIN
5JYQ,"A, B",Conus geographus (Cone Snail),"Insulin 1, Insulin 1b"
🌳 Phylogenetic Tree Topology

The phylogenetic tree confirms that chain type (A vs. B) is a more fundamental evolutionary division than the slight species differences among mammals, and that cone snail Insulin is a clear outlier.

    B Chain Clade (Highly Conserved): The four mammalian B chains (3I40_2, 4E7U_2, 1ZNI_2, 4INS_2) collapse to a single basal node with zero branch length. This grouping is the evolutionary root of the tree.

    A Chain Clade (Closer Group):

    The core mammalian A chains (3I40_1, 1ZNI_1, 4INS_1) form a tight subgroup with zero branch length.
    The Bovine A chain (4E7U_1) is slightly divergent (0.03095).
    Divergent Clades (5JYQ): The cone snail Insulins branch off first, illustrating their distant evolutionary relationship to the entire mammalian group:

    The most highly divergent sequence is the cone snail B chain (5JYQ_2) with a large branch length (0.40077).
    The cone snail A chain (5JYQ_1) is also significantly divergent (0.23868).
    The overall topology demonstrates that the A and B chains are functionally and structurally separated, but the high sequence identity within the mammalian group reflects the intense evolutionary constraint on the canonical insulin structure.
    🛠️ Methods and Citation

Tool Execution Details

    Program: MUSCLE (Multiple Sequence Alignment).

Version: v3.8.425.

Clustering Method: UPGMB (Unweighted Pair Group Method with Arithmetic mean).

Job Title: INSULIN-MUSCLE TOOL.
Citation

If you utilize this analysis in your work, please cite the MUSCLE publication:

    Edgar, R.C. (2004). MUSCLE: multiple sequence alignment with high accuracy and high throughput. Nucleic Acids Research, 32(5): 1792-97.
