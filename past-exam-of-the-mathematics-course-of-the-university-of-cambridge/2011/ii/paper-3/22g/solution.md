<h1 id="22g/solution">Solution</h1>

↑ **Parent:** [22G](../22g.md)

The [Monodromy theorem](../../../../../monodromy-theorem.md) states that if a holomorphic germ can be analytically continued along every path in a domain, its continuations along paths homotopic with fixed endpoints coincide. In a [simply connected domain](../../../../../simply-connected-domain.md) this gives a single-valued holomorphic function on the whole domain.

Write $\zeta_j=e^{2\pi ij/n}$. Remove the radial rays $R_j=\{t\zeta_j:t\geq1\}$ and set $U=\mathbb C\setminus\bigcup_jR_j$. This is an open star-shaped domain containing zero, hence simply connected, and $h=z^n-1$ never vanishes there. Locally its logarithm continues along all paths in $U$, so monodromy gives a holomorphic logarithm $L$ and

$$
\boxed{h^{1/r}=e^{L/r}\quad\text{on }U.}
$$

Equivalently, integrate $h'/h$ on the simply connected domain and choose the additive constant to obtain $e^L=h$.

Take $r$ copies of the slit domain, labeled by $j\in\mathbb Z/r\mathbb Z$, carrying values $e^{(L+2\pi ij)/r}$. Across each cut identify banks so that a positive loop around its simple zero increments the sheet index by one. This cyclic gluing produces the unbranched [Riemann surface](../../../../../riemann-surfaces.md) over $\mathbb C\setminus Z$, on which $w^r=z^n-1$ is single valued. Completing each finite puncture gives local coordinate $w$, with

$$
z-\zeta_j=\frac{w^r}{n\zeta_j^{n-1}}+O(w^{2r}).
$$

There is one ramification point of index $r$ over each of the $n$ roots of unity.

At infinity a loop around all $n$ zeros acts on sheet labels by $j\mapsto j+n\pmod r$. With $d=\gcd(n,r)$ this permutation has $d$ cycles, each of length $r/d$. In the compactification there are therefore $d$ points over infinity, each with ramification index $r/d$. Infinity is unbranched precisely when $d=r$, namely when $r\mid n$. Counting branch values in the base sphere,

$$
\boxed{\#\{\text{branch values of }\widetilde\pi\}=n\iff r\mid n;\quad\text{otherwise it is }n+1.}
$$

If “branch points” denotes ramification points upstairs instead, the count is $n$ or $n+d$ respectively, with exactly the same stated equivalence.

## ↑ Ancestors (10)

1. [22G](../22g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
