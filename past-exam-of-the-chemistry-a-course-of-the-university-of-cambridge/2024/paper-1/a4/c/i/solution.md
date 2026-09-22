<h1 id="a4/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Ideal gaseous [phosphorus pentachloride](../../../../../../phosphorus-pentachloride.md) is a trigonal bipyramid with [D3h molecular point group](../../../../../../d3h-molecular-point-group.md) symmetry. There are five chlorine sites and three 3p orbitals per site, hence a fifteen-dimensional basis. A moved atom contributes zero to the character; each fixed chlorine contributes the trace of the three-dimensional polar-vector matrix acting on its local p orbitals.

$$
\begin{array}{c|rrrrrr}
\text{class}&E&2C_3&3C_2^\prime&\sigma_h&2S_3&3\sigma_v\\\hline
\text{fixed Cl sites}&5&2&1&3&0&3\\
\operatorname{tr}D_{xyz}&3&0&-1&1&0&1\\
\chi_{15p}&15&0&-1&3&0&3
\end{array}
$$

For example, a $C_2^\prime$ axis through one equatorial chlorine fixes that site but rotates its p-vector basis with trace $1-1-1=-1$. Counting that atom as $+1$ would be incorrect.

Apply [molecular character reduction](../../../../../../molecular-character-reduction.md) with class sizes $(1,2,3,1,2,3)$ and group order twelve:

$$
n_\lambda=\frac1{12}\sum_C |C|\chi_{15p}(C)\chi_\lambda(C)^*.
$$

For $A_1^\prime$, this gives $(15-3+3+9)/12=2$; for $E^\prime$, $(30+6)/12=3$. The full result is

$$
\boxed{\Gamma_{15p}=2A_1^\prime\oplus A_2^\prime\oplus3E^\prime
\oplus2A_2^{\prime\prime}\oplus2E^{\prime\prime}.}
$$

The dimension check is $2+1+6+2+4=15$. As an additional transparent separation, the two axial chlorines supply $A_1^\prime+E^\prime+A_2^{\prime\prime}+E^{\prime\prime}$, while the three equatorial ones supply $A_1^\prime+A_2^\prime+2E^\prime+A_2^{\prime\prime}+E^{\prime\prime}$. These are all chlorine 3p orbitals, including both radial and tangential functions; a five-orbital ligand-sigma basis would answer a different question.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [C](../../c.md)
3. [A4](../../../a4.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2024](../../../../split.md)
6. [Past exam of the chemistry A course of the University of Cambridge](../../../../../split.md)
7. [Chemistry A course of the University of Cambridge](../../../../../../chemistry-a-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
