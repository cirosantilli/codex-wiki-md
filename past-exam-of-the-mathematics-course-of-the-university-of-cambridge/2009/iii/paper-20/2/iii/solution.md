<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For the shaded bigon, a holomorphic strip is a conformal parametrization of its interior. Send its two corners to the two ends of $\mathbb R\times[0,1]$. The Riemann map is unique up to translation, so quotienting the moduli space by translations leaves a single point. The embedded strip is regular, and a coherent orientation assigns it sign $+1$ or $-1$. Thus **the signed count is $\pm1$**. The other three small bigons have the same argument.

For the shaded rectangle, a disk in $\operatorname{Sym}^2(\Sigma)$ is represented by a two-sheeted surface over the strip, with its projection to $\Sigma$ covering the rectangle once. There is one simple branch point. The four alternating boundary arcs and the conformal modulus of the rectangular region determine the branched cover up to strip translation: cutting along an arc from the branch point produces two simply connected strips, whose conformal maps are fixed by their marked corners, and gluing fixes the relative translation. The index calculation in part (ii) gives a zero-dimensional quotient; regularity of this embedded empty rectangle makes its one solution an isolated regular point. Hence **its signed count is also $\pm1$**. The same construction applies to the lower rectangle. This is the [empty bigon and rectangle counts in Heegaard Floer homology](../../../../../../empty-bigon-and-rectangle-counts-in-heegaard-floer-homology.md) calculation, including the geometric reason for the counts.

The listed bigons and rectangles give all positive index-one domains in these diagrams. One can check this by following the alpha and beta boundary arcs: the four two-corner regions in Figure 2a and the two empty four-corner regions in Figure 2b are the possibilities with convex corners; a domain reaching around a handle has an additional corner or a negative region coefficient. There is no nonzero basepoint-normalized periodic domain, because the displayed [homology](../../../../../../homology-split.md) presentations have nonzero determinant. Adding the whole surface increases the [Maslov index](../../../../../../maslov-index.md) by two, so does not give another index-one representative. Thus no extra [chain differential](../../../../../../boundary-operator.md) term is hidden in the calculations below.

For Figure 2a with the basepoint outside the four small bigons, coherent signs can be absorbed into the choices of generator orientations, yielding a [chain complex](../../../../../../chain-complex.md) of the form

$$
\partial 2=1+3,\qquad\partial 5=6,\qquad\partial 7=6,\qquad\partial1=\partial3=\partial4=\partial6=0.
$$

The first summand has [homology](../../../../../../homology-split.md) $R\langle[1]\rangle$, with $[3]=-[1]$. The singleton $4$ contributes $R$. In the last summand, $6$ is a boundary and the cycles are $R\langle5-7\rangle$. Consequently

$$
\boxed{HF^-(\text{Figure 2a})\cong R\oplus R\oplus R,}
$$

one free tower in each [Spin-c structure](../../../../../../spin-c-structure.md). With the normalizations in part (i), their top [relative Heegaard Floer gradings](../../../../../../relative-grading-in-heegaard-floer-homology.md) are $0,0,1$.

The absent visible basepoint in Figure 2a does not change this [homology](../../../../../../homology-split.md) answer. For the multiplicities of part (i), replace the three nonzero [chain differential](../../../../../../boundary-operator.md) formulas by $\partial2=\pm U^a1\pm U^b3$, $\partial5=\pm U^c6$, $\partial7=\pm U^d6$. At most one of $a,b,c,d$ equals one, and the others are zero, so each two-term relation contains a unit. Elementary elimination again leaves one free $R$ tower in each class; its [relative Heegaard Floer grading](../../../../../../relative-grading-in-heegaard-floer-homology.md) is read from the multiplicity-dependent grading formulas.

For Figure 2b, write $A=(1,a)$, $B=(2,b)$, $C=(3,c)$. The two rectangles give, after choosing orientations,

$$
\partial B=A+C,\qquad\partial A=\partial C=0,
$$

and both singleton generators have zero [chain differential](../../../../../../boundary-operator.md). The first summand has cycles $RA\oplus RC$ modulo the primitive relation $A+C$, hence is $R$. Therefore

$$
\boxed{HF^-(\text{Figure 2b})\cong R\oplus R\oplus R,}
$$

again with one free tower in each [Spin-c structure](../../../../../../spin-c-structure.md). All three can have top [relative Heegaard Floer grading](../../../../../../relative-grading-in-heegaard-floer-homology.md) zero in the independent normalizations of part (ii).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
