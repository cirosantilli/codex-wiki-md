<h1 id="s18/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Expand $G(x,x')$ in a complete [orthonormal](../../../../../orthonormal-set.md) [eigenbasis](../../../../../eigenbasis.md) in its first argument. Applying the operator yields $\sum_n(E_n-E)c_n\varphi_n(x)=\delta(x-x')$. Completeness expands the [Dirac delta distribution](../../../../../dirac-delta-function.md) as $\sum_n\varphi_n(x)\varphi_n^*(x')$, so

$$
\boxed{c_n=\frac{\varphi_n^*(x')}{E_n-E},\qquad
G(x,x')=\sum_n\frac{\varphi_n(x)\varphi_n^*(x')}{E_n-E}.}
$$

Consequently $\lim_{E\to E_n}(E_n-E)G=\varphi_n(x)\varphi_n^*(x')$.

For the explicit formula, use $E_n-E\simeq-(\hbar^2k_n/m)(k-k_n)$ and $\sin ka\simeq(-1)^na(k-k_n)$. Also  
$\sin[k_n(a/2-x)]=(-1)^{n+1}\sin[k_n(x+a/2)]$. The resulting limit is

$$
\boxed{\varphi_n(x)\varphi_n^*(x')=
\frac2a\sin\frac{n\pi(x+a/2)}a\sin\frac{n\pi(x'+a/2)}a.}
$$

The expression is symmetric in $x,x'$ and holds on either side of the source. The usual complex-analysis [residue](../../../../../residue.md) with respect to $E-E_n$ has the opposite sign, since the source requests the limit with $E_n-E$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [S18](../../../s18.md)
4. [2018](../../../../2018-split.md)
5. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
