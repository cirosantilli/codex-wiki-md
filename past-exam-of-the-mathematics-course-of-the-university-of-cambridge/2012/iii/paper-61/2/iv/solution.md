<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Take every finite positive [drag coefficient](../../../../../../drag-coefficient.md) $\gamma>0$ and define

$$
K=2\Omega(2\Omega-S),\qquad L=\Omega(\alpha+\beta-S),\qquad P=\alpha\beta.
$$

The coefficients of the [characteristic polynomial](../../../../../../characteristic-polynomial.md) are $c_3=2\gamma$, $c_2=K+\gamma^2$, $c_1=2L\gamma$ and $c_0=P\gamma^2$. The nontrivial [Routh-Hurwitz criterion](../../../../../../routh-hurwitz-stability-criterion.md) reduces exactly to

$$
c_3c_2c_1-c_3^2c_0-c_1^2=4\gamma^2\left[L(K-L)+\gamma^2(L-P)\right]>0.
$$

The printed strict chain $K>L>P>0$ makes every coefficient positive and both bracket terms positive, so it proves attraction for every positive [drag coefficient](../../../../../../drag-coefficient.md).

There is, however, a boundary error in the asserted necessity. To have the bracket positive for every $\gamma>0$, its constant and slope as a function of $\gamma^2$ must be nonnegative, and cannot both vanish. Together with coefficient positivity this gives the exact [drag-polynomial stability for all positive stopping rates](../../../../../../drag-polynomial-stability-for-all-positive-stopping-rates.md):

$$
\boxed{K\geq L\geq P>0,\qquad K>P.}
$$

Necessity follows by taking arbitrarily small and arbitrarily large positive $\gamma$; if one bracket coefficient is negative, the inequality fails in the corresponding limit. Sufficiency follows because at least one coefficient is strictly positive. Thus $K=L>P$ and $K>L=P$ still give strict decay at each finite positive $\gamma$. They need not give a uniform stability margin in the zero- or infinite-drag limit.

In a [Keplerian shearing sheet](../../../../../../keplerian-shearing-sheet.md), $S=3\Omega/2$ and

$$
\frac K{\Omega^2}=1,\quad\frac L{\Omega^2}=\frac{3(r+1)}{2r(r-1)},\quad\frac P{\Omega^2}=\frac9{4(r-1)^2}.
$$

The differences are

$$
\frac{K-L}{\Omega^2}=\frac{(r-3)(2r+1)}{2r(r-1)},\qquad\frac{L-P}{\Omega^2}=\frac{3(2r+1)(r-2)}{4r(r-1)^2}.
$$

Hence $r>3$ establishes the requested strict chain and trapping conclusion. At $r=3$, however, $K=L=\Omega^2$ and $P=9\Omega^2/16$, so

$$
c_3c_2c_1-c_3^2c_0-c_1^2=\frac74\Omega^2\gamma^4>0.
$$

All coefficients remain positive. This is an explicit counterexample within the stated vortex model: **$r=3$ also attracts particles for every finite positive [drag coefficient](../../../../../../drag-coefficient.md), so the literal strict “if and only if” is false.** The exact Keplerian all-positive-drag condition is $r\geq3$. If $\gamma=0$ is included, the polynomial has zero and purely imaginary roots and there is no asymptotic attraction; “all drag coefficients” must mean positive drag. The local attraction claim presumes the particle remains in the patch, as is assured for sufficiently small perturbations of its centre.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
