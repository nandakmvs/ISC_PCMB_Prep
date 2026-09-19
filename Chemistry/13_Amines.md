# Chapter 13: Amines

## 1. Exhaustive Theory & Precise ISC Terminology

Amines are derivatives of ammonia ($NH_3$), obtained by replacement of one, two, or all three hydrogen atoms by alkyl/aryl groups.
- **Primary ($1^\circ$) Amine**: $R-NH_2$ (one H replaced).
- **Secondary ($2^\circ$) Amine**: $R_2NH$ (two H replaced).
- **Tertiary ($3^\circ$) Amine**: $R_3N$ (three H replaced).

### Preparation of Amines
1. **Reduction of Nitro Compounds**: $R-NO_2 \xrightarrow{Sn/HCl \text{ or } H_2/Pd} R-NH_2$. (Sn/HCl is preferred for aromatic nitro to aniline).
2. **Ammonolysis of Alkyl Halides**: $RX + NH_3 \rightarrow 1^\circ, 2^\circ, 3^\circ$ amines and quaternary salts (mixture is a drawback).
3. **Reduction of Nitriles**: $R-C\equiv N \xrightarrow{LiAlH_4 \text{ or } H_2/Ni} R-CH_2NH_2$.
4. **Hoffmann Bromamide Degradation**: Primary amides treated with $Br_2$ and aqueous/ethanolic NaOH. 
   $R-CONH_2 + Br_2 + 4NaOH \rightarrow R-NH_2 + Na_2CO_3 + 2NaBr + 2H_2O$.
   **ISC Keyword**: Gives a primary amine with **one carbon less** than the parent amide (step-down reaction).
5. **Gabriel Phthalimide Synthesis**: Phthalimide + KOH $\rightarrow$ Potassium phthalimide. React with $RX$, then hydrolyze to give **only primary aliphatic amines**. (Aryl halides don't undergo nucleophilic substitution here, so aniline cannot be prepared).

### Basic Character of Amines
Amines act as **Lewis bases** due to the lone pair of electrons on the nitrogen atom.
- **Gas Phase Basic Strength**: $3^\circ > 2^\circ > 1^\circ > NH_3$ (due to $+I$ effect of alkyl groups).
- **Aqueous Phase Basic Strength (Methyl groups)**: $2^\circ > 1^\circ > 3^\circ > NH_3$. (Interplay of $+I$ effect, hydrogen bonding/solvation, and steric hindrance).
- **Aqueous Phase Basic Strength (Ethyl groups)**: $2^\circ > 3^\circ > 1^\circ > NH_3$.
- **Aryl Amines (Aniline)**: **Weaker** bases than ammonia because the lone pair on nitrogen is **delocalized into the benzene ring** via resonance, making it less available for protonation.

### Chemical Reactions
1. **Carbylamine Reaction (Isocyanide Test)**: Aliphatic and aromatic **primary** amines react with chloroform and alc. KOH to form foul-smelling isocyanides.
   $R-NH_2 + CHCl_3 + 3KOH \xrightarrow{\Delta} R-NC + 3KCl + 3H_2O$.
2. **Reaction with Nitrous Acid ($HNO_2$)**:
   - $1^\circ$ Aliphatic: Forms alcohol and liberates $N_2$ gas (quantitatively).
   - $1^\circ$ Aromatic: Forms stable **diazonium salts** at 0-5$^\circ$C (Diazotization).
3. **Hinsberg Test**: Benzene sulfonyl chloride ($C_6H_5SO_2Cl$).
   - $1^\circ$ Amine: Forms sulfonamide **soluble** in alkali (due to acidic H attached to N).
   - $2^\circ$ Amine: Forms sulfonamide **insoluble** in alkali (no acidic H).
   - $3^\circ$ Amine: Does not react.
4. **Electrophilic Substitution of Aniline**: $NH_2$ is highly activating, ortho/para directing.
   - **Bromination**: With $Br_2(aq)$, forms **2,4,6-tribromoaniline** (white ppt). To get mono-bromo, protect the $NH_2$ group by **acetylation** (forming acetanilide), brominate, then hydrolyze.

---

## 2. Step-by-Step Derivations & Mechanisms

### Mechanism of Hoffmann Bromamide Degradation
1. **Deprotonation**: Base ($OH^-$) removes a proton from amide $\rightarrow R-CONH^-$.
2. **Bromination**: Attacks $Br_2$ to form N-bromoamide ($R-CONHBr$).
3. **Deprotonation 2**: Base removes second proton $\rightarrow R-CON^-Br$.
4. **Rearrangement (Key Step)**: Alkyl group $R$ migrates from carbonyl carbon to nitrogen, and $Br^-$ leaves, forming an **alkyl isocyanate** ($R-N=C=O$).
5. **Hydrolysis**: Isocyanate hydrolyzes in basic medium to form primary amine ($R-NH_2$) and carbonate ion ($CO_3^{2-}$).

---

## 3. Diagram Blueprints & Labeling Checklists

### Resonance in Aniline Diagram
- Draw 5 resonance structures.
- **Checklist**:
  1. Structure 1: Lone pair on N, neutral.
  2. Structure 2: Double bond C=N, positive charge on N, negative charge on ortho carbon.
  3. Structure 3: Negative charge on para carbon.
  4. Structure 4: Negative charge on the other ortho carbon.
  5. Structure 5: Back to neutral.
- **Conclusion**: Shows electron density is higher at ortho and para positions, explaining directing nature and decreased basicity.

---

## 4. "Avoid the Trap" & Distinction Tables

| Test | Reagent | Primary ($1^\circ$) | Secondary ($2^\circ$) | Tertiary ($3^\circ$) |
| :--- | :--- | :--- | :--- | :--- |
| **Carbylamine** | $CHCl_3$ + alc. KOH | Foul smell (Isocyanide) | No reaction | No reaction |
| **Hinsberg** | $C_6H_5SO_2Cl$ | Soluble in NaOH | Insoluble in NaOH | No reaction |
| **Nitrous Acid** | $NaNO_2$ + HCl | $N_2$ gas (aliphatic) / Diazonium (aromatic) | Yellow oily liquid (Nitrosamine) | Soluble nitrite salt |

### ⚠️ ISC Traps & Subjective Pitfalls
- **Trap**: Using Gabriel phthalimide synthesis to make aniline.
  - *Correction*: Never! The aryl halide does not undergo nucleophilic substitution to break the C-X bond under these conditions.
- **Trap**: Direct nitration of aniline yields a significant amount of *meta*-nitroaniline.
  - *Correction*: This happens because in acidic medium ($HNO_3/H_2SO_4$), aniline is protonated to **anilinium ion** ($+NH_3$), which is strongly deactivating and **meta-directing**.
- **Trap**: Alkylation of amines (Ammonolysis) gives a pure primary amine.
  - *Correction*: It gives a complex mixture of $1^\circ, 2^\circ, 3^\circ$ and quaternary salts. Use Hoffmann or Gabriel for pure $1^\circ$ amines.

---

## 5. High-Yield Worked Model Problems

### Q1. ISC Step-by-Step Problem: Basic Strength Ordering
**Arrange the following in increasing order of basic strength in aqueous solution: $NH_3, CH_3NH_2, (CH_3)_2NH, (CH_3)_3N$. Give reasons.**

**ISC Method:**
1. **Identify the groups**: Methylamines.
2. **State the order**: $NH_3 < (CH_3)_3N < CH_3NH_2 < (CH_3)_2NH$.
3. **Reasoning**:
   - The basicity in aqueous solution is determined by a balance of three factors: **inductive effect** (+I), **solvation effect** (hydrogen bonding of conjugate acid with water), and **steric hindrance**.
   - Inductive effect favors $3^\circ > 2^\circ > 1^\circ$.
   - Solvation (H-bonding) favors $1^\circ > 2^\circ > 3^\circ$.
   - For methyl group (small size), the combination of solvation and inductive effect makes the $2^\circ$ amine the strongest base, followed by $1^\circ$, then $3^\circ$ (due to severe steric hindrance to hydration).
4. **Conclusion**: Hence the order is $NH_3 < 3^\circ < 1^\circ < 2^\circ$.

### Q2. ISC Step-by-Step Problem: Conversion
**Convert Benzene to Aniline.**

**ISC Method:**
1. **Nitration**: Treat benzene with a mixture of conc. $HNO_3$ and conc. $H_2SO_4$ at 323-333 K.
   $C_6H_6 + HNO_3 \xrightarrow{H_2SO_4} C_6H_5NO_2 \text{ (Nitrobenzene)} + H_2O$
2. **Reduction**: Reduce nitrobenzene using Tin (Sn) and concentrated HCl.
   $C_6H_5NO_2 + 6[H] \xrightarrow{Sn/HCl} C_6H_5NH_2 \text{ (Aniline)} + 2H_2O$
*(Always balance the reduction equation with $[H]$ and byproducts).*
