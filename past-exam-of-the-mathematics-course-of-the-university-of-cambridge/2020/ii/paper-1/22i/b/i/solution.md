<h1 id="22i/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $h(t)=t/(1+t)$ for $t\ge0$. Every summand in $d$ is nonnegative and at most $2^{-m}$, so the series converges. Symmetry is immediate. If $d(x,y)=0$, then $\phi_m(x-y)=0$ for every $m$. For arbitrary $\phi\in(\ell^p)^*$, choose a sequence of $\phi_m$ converging to $\phi$ in operator norm. Since $x-y$ is fixed, $\phi(x-y)=0$. The [continuous dual space](../../../../../../../continuous-dual-space-split.md) separates points, so $x=y$.

The function $h$ is increasing and subadditive:

$$
h(a+b)\le h(a)+h(b)\qquad(a,b\ge0).
$$

Combining this with the [triangle inequality](../../../../../../../triangle-inequality.md) for each $|\phi_m(x-y)|$ and summing proves the triangle inequality for $d$. Hence $d$ is a [metric](../../../../../../../metric.md) on $B$.

Suppose first that $x^{(n)}$ converges weakly to $x$, meaning that

$$
\phi(x^{(n)})\to\phi(x)
\qquad\text{for every }\phi\in(\ell^p)^*.
$$

For each fixed $m$, the $m$th summand of $d(x^{(n)},x)$ tends to zero. A finite-head and geometric-tail estimate, using that every summand is bounded by $2^{-m}$, then gives $d(x^{(n)},x)\to0$.

Conversely, if $d(x^{(n)},x)\to0$, each nonnegative summand tends to zero, and therefore

$$
\phi_m(x^{(n)}-x)\to0
$$

for every $m$. Given $\phi\in(\ell^p)^*$ and $\varepsilon>0$, choose $m$ with $\|\phi-\phi_m\|<\varepsilon$. Since $x^{(n)},x\in B$,

$$
|\phi(x^{(n)}-x)|
\le|\phi_m(x^{(n)}-x)|+2\varepsilon.
$$

Taking the limit superior and then letting $\varepsilon\downarrow0$ proves weak convergence. Thus

$$
\boxed{\phi(x^{(n)})\to\phi(x)\ \forall\phi\in(\ell^p)^*
\iff d(x^{(n)},x)\to0}.
$$

The same approximation argument for neighbourhoods shows that $d$ induces the weak topology on $B$, as in the [metrization of the weak topology on a bounded set](../../../../../../../metrization-of-the-weak-topology-on-a-bounded-set.md).

If $q$ is conjugate to $p$, the given [duality of sequence spaces](../../../../../../../duality-of-sequence-spaces.md) applied twice gives

$$
(\ell^p)^{**}\cong(\ell^q)^*\cong\ell^p,
$$

so $\ell^p$ is a [reflexive Banach space](../../../../../../../reflexive-banach-space.md). Its closed unit ball is weakly compact by the [weak compactness characterization of reflexivity](../../../../../../../weak-compactness-characterization-of-reflexivity.md). Since $d$ induces that topology on $B$,

$$
\boxed{(B,d)\text{ is a compact metric space}}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [22I](../../../22i.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
