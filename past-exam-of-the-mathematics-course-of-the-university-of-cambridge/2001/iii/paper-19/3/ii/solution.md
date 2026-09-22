<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

We prove that the only finite-order rational point is the origin: $\boxed{E(\mathbb Q)_{\rm tors}=\{O\}}$. The identity always has order one, so “no elements of finite order” must be understood as no nonidentity torsion points.

The given discriminant is a unit at $5$ and $7$, so the integral [Weierstrass equation of an elliptic curve](../../../../../../weierstrass-equation-of-an-elliptic-curve.md) has [good reduction](../../../../../../good-reduction-of-an-elliptic-curve.md) at both primes. For an odd prime $p$, completing the square in $y^2+xy=f(x)$ shows that the number of $y$ above $x$ is determined by

$$
(2y+x)^2=D(x),\qquad D(x)=x^2+4(x^3-120x+576).
$$

A nonzero quadratic residue gives two points, zero gives one, and a nonresidue gives none. Direct evaluation gives

$$
\begin{array}{c|ccccc}
x\pmod5&0&1&2&3&4\\\hline
D(x)\pmod5&4&4&0&1&1\\
\#\{y\}&2&2&1&2&2
\end{array}
\qquad
\begin{array}{c|ccccccc}
x\pmod7&0&1&2&3&4&5&6\\\hline
D(x)\pmod7&1&2&1&1&5&2&2\\
\#\{y\}&2&2&2&2&0&2&2.
\end{array}
$$

Including the origin gives $\#\widetilde E(\mathbb F_5)=10$ and $\#\widetilde E(\mathbb F_7)=13$.

At a good prime $p$, reduction is injective on torsion of order prime to $p$: a point in its kernel belongs to the formal group, where multiplication by that order is bijective by part(i), so a point killed by it must be zero. Suppose a nonidentity rational point has finite order. Taking a suitable multiple gives a point of prime order $\ell$. If $\ell\notin\{5,7\}$, reduction at both primes forces $\ell$ to divide both $10$ and $13$, impossible. If $\ell=5$, reduction at $7$ forces $5\mid13$, impossible. If $\ell=7$, reduction at $5$ forces $7\mid10$, also impossible. This exhausts all primes and proves the claim. The [torsion exclusion from good reduction counts](../../../../../../torsion-exclusion-from-good-reduction-counts.md) explicitly handles the two residual characteristics instead of incorrectly assuming prime-to-$p$ injectivity also controls $p$-torsion.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 19](../../../paper-19-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
