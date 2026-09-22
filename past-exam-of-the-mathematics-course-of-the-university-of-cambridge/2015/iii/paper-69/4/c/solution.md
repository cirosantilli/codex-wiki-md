<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix the degree bound $n$. Existence can be proved without a general uniqueness theorem: a minimizing sequence in $\mathcal P_n$ is uniformly bounded because its distances from $f$ are bounded. Values at any fixed $n+1$ distinct points determine its coefficients through an invertible [Vandermonde matrix](../../../../../../vandermonde-matrix.md), so those coefficients are bounded. A convergent subsequence supplies a [polynomial](../../../../../../polynomial-split.md) attaining the minimum.

For [uniqueness of best uniform polynomial approximation](../../../../../../uniqueness-of-best-uniform-polynomial-approximation.md), suppose $p$ and $q$ attain the same minimum $d$, and let $r=(p+q)/2$. The [triangle inequality](../../../../../../triangle-inequality.md) makes $r$ another minimizer. If $d=0$, both [polynomials](../../../../../../polynomial-split.md) equal $f$, so assume $d>0$. Put $e=f-r$ and $E=\{|e|=d\}$. At each $x\in E$, the two real errors $f-p$ and $f-q$ lie in $[-d,d]$ and their average equals an endpoint. Hence they are equal there, and $p(x)=q(x)$.

The set $E$ must contain at least $n+2$ points. Otherwise interpolate the values $\operatorname{sign}e(x)$ on its at most $n+1$ points by a [polynomial](../../../../../../polynomial-split.md) $v\in\mathcal P_n$. Then $ev>0$ on $E$. Continuity gives this positivity on a neighbourhood of $E$, while the error has a strict gap below $d$ on the compact complement. A sufficiently small positive multiple of $v$ decreases the maximum error, contradicting optimality of $r$. This is an elementary perturbation argument, not an appeal to Haar's theorem.

Thus $p-q$ has at least $n+2$ distinct zeros. A [polynomial](../../../../../../polynomial-split.md) of degree at most $n$ with that many zeros is identically zero. **The best uniform [polynomial](../../../../../../polynomial-split.md) is unique for every fixed degree bound**: $\boxed{p=q}$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
