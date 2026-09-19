# 05 - Principles of Inheritance and Variation

## 1. Exhaustive Theory & Precise ISC Terminology
- **Mendel's Laws of Inheritance**:
  - **Law of Dominance**: Characters are controlled by discrete units called **factors** (genes). In a dissimilar pair, one dominates the other.
  - **Law of Segregation**: Alleles do not blend. During gamete formation, alleles of a pair segregate independently so each gamete receives only one allele.
  - **Law of Independent Assortment**: When two pairs of traits are combined in a hybrid, segregation of one pair of characters is independent of the other pair.
- **Exceptions & Extensions**:
  - **Incomplete Dominance**: F1 phenotype is intermediate between parents (e.g., *Antirrhinum* - Snap dragon flower color). F2 Ratio: 1:2:1 (Genotypic AND Phenotypic).
  - **Co-dominance**: Both alleles express themselves fully in F1 (e.g., ABO blood grouping). Alleles $I^A$ and $I^B$ are co-dominant, completely dominant over $i$.
  - **Multiple Alleles**: More than two alleles govern a single character (e.g., ABO blood groups - $I^A$, $I^B$, $i$). Studied at population level.
  - **Pleiotropy**: A single gene controls multiple phenotypic traits (e.g., Phenylketonuria, Sickle cell anemia).
  - **Polygenic Inheritance**: Traits controlled by three or more genes, showing continuous variation (e.g., Human skin color, height).
- **Chromosomal Theory of Inheritance**: Sutton and Boveri unified Mendelian genetics with chromosome movement during meiosis. Genes are located on chromosomes, which segregate and assort independently.
- **Linkage and Recombination**: T.H. Morgan (using *Drosophila melanogaster*). 
  - **Linkage**: Physical association of genes on a chromosome. Tightly linked genes show very low **recombination** (crossing over).
  - Recombination frequency is directly proportional to the physical distance between genes (used for **genetic mapping** by Sturtevant).
- **Sex Determination**: 
  - Male heterogamety: XX-XY (Humans, Drosophila), XX-XO (Grasshopper).
  - Female heterogamety: ZW-ZZ (Birds).
  - Haplodiploidy in Honeybees: Females (2n=32) from fertilized eggs, Males/Drones (n=16) from unfertilized eggs via parthenogenesis.
- **Genetic Disorders**:
  - **Mendelian Disorders**: Haemophilia (X-linked recessive), Sickle-cell anemia (Autosomal recessive, mutation of Glu to Val at 6th position of beta-globin chain), Phenylketonuria (Autosomal recessive, lack of enzyme converting phenylalanine to tyrosine), Thalassemia (Autosomal recessive), Colour Blindness (X-linked recessive).
  - **Chromosomal Disorders**: Aneuploidy (failure of segregation during meiosis). Down's Syndrome (Trisomy 21), Klinefelter's Syndrome (44A + XXY), Turner's Syndrome (44A + XO).

## 2. Step-by-Step Mechanisms
**Drawing a Dihybrid Cross (Mendelian)**:
1. Identify parent genotypes: RRYY (Round Yellow) x rryy (Wrinkled Green).
2. Gametes formed: RY and ry.
3. F1 generation: RrYy (Round Yellow).
4. F1 selfing gametes: RY, Ry, rY, ry.
5. Create a 4x4 Punnett square.
6. Phenotypic ratio obtained: 9 (Round Yellow) : 3 (Round Green) : 3 (Wrinkled Yellow) : 1 (Wrinkled Green).

## 3. Diagram Blueprints & Labeling Checklists
- **Pedigree Analysis Symbols**:
  - Square: Male; Circle: Female; Diamond: Sex unspecified.
  - Shaded: Affected individual.
  - Single line between square & circle: Mating.
  - Double line: Consanguineous mating (mating between relatives).
  - *ISC Marking Scheme*: Always provide a key for the symbols. Ensure generations are marked with Roman numerals (I, II, III).
- **Sickle Cell Anemia Mutation**:
  - *Checklist*: DNA template strand (CTC -> CAC), mRNA (GAG -> GUG), Amino acid (Glutamic acid -> Valine).
  - *ISC Marking scheme*: Exact positions (6th position of beta-globin) and exact codon changes are strictly checked.

## 4. "Avoid the Trap" & Distinction Tables
| Feature | Autosomal Recessive | X-Linked Recessive |
|---|---|---|
| **Transmission** | Appears in both sexes with equal frequency | Much more common in males |
| **Carrier Parents** | Both parents must be at least carriers for child to be affected | Mother carrier + Normal father can have affected son |
| **Father to Son** | Can be transmitted | **Never transmitted** (Father gives Y to son) |

- **Trap**: Test Cross vs Back Cross. A test cross is a *type* of back cross where F1 is crossed with the **recessive parent** to determine heterozygosity. Ratio is always 1:1 or 1:1:1:1.
- **Trap**: Linkage exception to Independent Assortment. Linked genes *do not* assort independently. If the dihybrid ratio deviates significantly from 9:3:3:1, suspect linkage.
- **Trap**: "Male honeybees have no father and thus cannot have sons, but have a grandfather and can have grandsons." *Why? Males come from unfertilized eggs (parthenogenesis from queen/mother), and pass their genetics to female offspring only.*

## 5. High-Yield Worked Model Problems
**Q1 (ISC Subjective):** A haemophilic man marries a normal homozygous woman. What is the probability that their son will be haemophilic? Give a pedigree cross to justify. (3 Marks)
**Step-by-step Answer:**
1. Let the haemophilia allele be $X^h$ and normal allele be $X^H$.
2. Genotype of haemophilic man: $X^hY$. Genotype of normal homozygous woman: $X^HX^H$.
3. Cross: $X^hY$ x $X^HX^H$.
4. Gametes: ($X^h$, $Y$) and ($X^H$).
5. Offspring: All daughters are carriers ($X^HX^h$). All sons are completely normal ($X^HY$).
6. **Probability of haemophilic son is 0%.** The father passes his Y chromosome to his sons, which does not carry the gene.

**Q2 (NEET/JEE Speed):** The recombination frequency between genes A & B is 9%, A & C is 17%, and B & C is 8%. What is the sequence of genes on the chromosome?
**Speed Method:** Map distance = Recombination %. The largest distance is A to C (17). B must be in the middle because A-B (9) + B-C (8) = 17.
**Answer:** A - B - C.
