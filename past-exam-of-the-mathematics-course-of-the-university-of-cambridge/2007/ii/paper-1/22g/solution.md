<h1 id="22g/solution">Solution</h1>

↑ **Parent:** [22G](../22g.md)

The [continuous dual space](../../../../../continuous-dual-space-split.md) $X^*$ consists of bounded linear functionals with [operator norm](../../../../../operator-norm.md) $\|v\|=\sup_{\|x\|\le1}|v(x)|$. For an operator-norm [Cauchy sequence](../../../../../cauchy-sequence.md) $(v_n)$, each $(v_n(x))$ is Cauchy in $\mathbb R$. Define $v(x)=\lim_n v_n(x)$. It is linear, and bounded because the Cauchy sequence has uniformly bounded norms. Passing to the pointwise limit in $|(v_n-v_m)(x)|\le\varepsilon\|x\|$ gives $\|v_n-v\|\le\varepsilon$. Thus $X^*$ is a [Banach space](../../../../../banach-space-split.md), even when $X$ is incomplete.

The canonical map $\phi(x)(v)=v(x)$ is linear and satisfies $\|\phi(x)\|\le\|x\|$. For $x\ne0$, the norm-one functional $tx\mapsto t\|x\|$ on its span extends by the [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) to a norm-one functional on $X$. Hence $\|\phi(x)\|\ge\|x\|$, proving that $\phi$ is an [isometry](../../../../../isometry.md) and therefore [injective](../../../../../injective-function.md).

For a nonsurjective example take $X=c_0$ with the supremum norm. It is complete as a closed subspace of $\ell^\infty$. Every functional is given by an $\ell^1$ sequence: finite-coordinate sign tests give summability of its coefficients, and truncation of each $c_0$ vector gives the series representation. Conversely any $\ell^1$ sequence defines such a bounded functional. Similarly $(\ell^1)^*=\ell^\infty$, so $c_0^{**}=\ell^\infty$. The canonical image is the null sequences; the constant sequence one is outside it. Thus **$c_0$ is a nonreflexive Banach space**.

## ↑ Ancestors (10)

1. [22G](../22g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
