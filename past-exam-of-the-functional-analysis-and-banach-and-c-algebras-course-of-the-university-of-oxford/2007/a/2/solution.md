<h1 id="a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Regard the spaces as real and set $u=\operatorname{Re}\phi$. Its real [norm](../../../../norm.md) equals $\|\phi\|$, since rotating any test vector makes its functional value real and nonnegative without changing its [norm](../../../../norm.md). By the allowed real [Hahn-Banach theorem](../../../../hahn-banach-theorem.md) extend $u$ to a real-linear $v:X\to\mathbb R$ with that [norm](../../../../norm.md), and define $\psi(x)=v(x)-iv(ix)$. Real linearity gives $\psi(ix)=i\psi(x)$, so $\psi$ is complex linear. On $Y$ this formula recovers $\phi$. Also $\operatorname{Re}\psi=v$; rotating a test vector again gives $|\psi(x)|\leq\|v\|\|x\|$. The reverse [norm](../../../../norm.md) inequality follows by restriction to $Y$, proving **a [norm](../../../../norm.md)-preserving complex extension**.

We use two standard consequences: a point outside a [closed subspace](../../../../closed-subspace.md) can be separated by a bounded functional annihilating that subspace, and the [norm](../../../../norm.md) of a vector is the supremum of its pairings with dual unit-ball functionals. If $\psi\in X^*$ annihilates $Y$, the scalar [holomorphic function](../../../../holomorphic-function-split.md) $\psi\circ f$ vanishes at the prescribed sequence tending to zero. Its [identity theorem](../../../../identity-theorem.md) makes it identically zero. Separation then gives **$f(z)\in Y$ for every $z\in D$**.

For $\phi\in Y^*$ extend to $X^*$ with the same [norm](../../../../norm.md) and put $F=\phi\circ f$. Then $F$ is holomorphic with $|F|\leq\|\phi\|$. For the understood nonzero increments $h,k$, the [Cauchy integral formula](../../../../cauchy-integral-formula.md) on $|\zeta|=r$ gives

$$
\frac{F(z+h)-F(z)}h-\frac{F(z+k)-F(z)}k=\frac{h-k}{2\pi i}\int_{|\zeta|=r}\frac{F(\zeta)}{(\zeta-z)(\zeta-z-h)(\zeta-z-k)}d\zeta.
$$

Taking absolute values, bounding the contour length by $2\pi r$, and each denominator below by $r-|z|$, $r-|z|-|h|$, $r-|z|-|k|$ proves **exactly the stated estimate**.

Fix $z,r$ and restrict $|h|,|k|<(r-|z|)/2$. Taking the supremum over $\|\phi\|\leq1$ bounds the [norm](../../../../norm.md) of the difference of the two $Y$-valued difference quotients by a fixed constant times $|h-k|$. They are therefore Cauchy as $h\to0$. Since $Y$ is a [closed subspace](../../../../closed-subspace.md) of a [Banach space](../../../../banach-space-split.md), it is complete. Consequently **the derivative exists as a [norm](../../../../norm.md) limit in $Y$**. The labelled (a)-(c) are the simultaneous hypotheses, not separate claims to prove.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../split.md)
5. [Functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../functional-analysis-and-banach-and-c-algebras-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
