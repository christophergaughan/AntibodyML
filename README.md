Machine Learning Antibody Design: Structure and Beyond
Machine learning models like RFdiffusion and AlphaFold3 represent a breakthrough in computational antibody design, achieving sub-angstrom structural accuracy for CDR loops and rigid-body docking. The Baker and Jumper labs have demonstrated that AI can now design antibodies de novo that bind user-specified epitopes with atomic precision—a remarkable achievement that opens new possibilities for therapeutic development.
These structure-prediction models excel at their intended purpose: designing geometrically optimal binding interfaces from sequence. However, the path from a perfect computational structure to a manufacturable therapeutic involves additional layers of biological complexity that emerge during cellular production.
Post-Translational Modifications in Antibody Variable Regions
Recent work by van de Bovenkamp et al. (2023) revealed that N-linked glycosylation occurs preferentially in and around CDRs—precisely where RFdiffusion designs binding interfaces. Key findings include:

CDR-proximal glycosylation: N-glycosylation sites (NXS/T sequons) emerge during somatic hypermutation in CDRs and the adjacent DE loop
Functional consequences: Fab glycans directly modulate antigen binding, with effects ranging from enhanced affinity to complete loss of binding
Positive selection: Glycosylation sites that enhance binding are retained during affinity maturation
Subclass variation: IgG4 exhibits significantly higher Fab glycosylation (>30%) compared to other subclasses
Disease relevance: Aberrant Fab glycosylation is associated with rheumatoid arthritis and autoimmune disorders

Experimentally validated glycosylation sites in therapeutic antibodies include positions NH59, NH77, NH82, NH84 (heavy chain) and NL37, NL86 (light chain) in adalimumab—all within or immediately adjacent to CDRs.
This creates a fundamental challenge for sequence-based design tools: a computationally "perfect" CDR may acquire glycosylation during production that sterically blocks the epitope, reduces affinity through electrostatic changes, or triggers unwanted immune responses.
Additional PTM Complexity Beyond Fab Glycosylation
Other PTMs that impact antibody developability include:

Fc glycosylation (ubiquitous in IgGs) - affects ADCC, CDC, serum half-life
CDR deamidation (Asn→Asp at NG/NS sites) - causes heterogeneity and charge variants
Methionine oxidation (CDRs and Fc) - impacts stability and immunogenicity
Fc sialylation patterns - modulate anti-inflammatory activity

AntibodyML Consulting addresses the critical gap between computational design and cellular reality. Our kinetic models predict PTM profiles from sequence and structural features, with particular emphasis on glycosylation sites that emerge in and around designed CDRs. This enables assessment of developability before expensive wet-lab validation.
Our approach is complementary to structural design: RFdiffusion/AlphaFold3 optimize binding geometry; our models ensure those designs will behave predictably in CHO/HEK293 production systems and won't acquire PTMs that abolish the designed function.

References
van de Bovenkamp, F.S., Derksen, N.I.L., Ooijevaar-de Heer, P., et al. (2023). Adaptive antibody diversification through N-linked glycosylation of the immunoglobulin variable region. PNAS Nexus, 2(3), pgad138. https://doi.org/10.1093/pnasnexus/pgad138
