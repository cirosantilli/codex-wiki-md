<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $L/K$ be a finite [Galois extension](../../../../../finite-galois-extension.md) of non-Archimedean [local fields](../../../../../local-field.md), let $G=\operatorname{Gal}(L/K)$, and normalize the [discrete valuation](../../../../../discrete-valuation.md) by $v_L(L^{\times})=\mathbb Z$. The [lower ramification numbering](../../../../../lower-ramification-numbering.md) is

$$
G_{-1}=G,\qquad
G_i=\{\sigma\in G:v_L(\sigma(x)-x)\geq i+1\text{ for every }x\in\mathcal O_L\},\quad i\geq0.
$$

Here $G_0$ is the [inertia group](../../../../../inertia-group.md) and $G_1$ is the [wild inertia group](../../../../../wild-inertia-group.md). For real $s\geq-1$, put $G_s=G_{\lceil s\rceil}$; thus $G_s=G_0$ for $-1<s\leq0$. Define the [Herbrand function](../../../../../herbrand-function.md) and its inverse by

$$
\varphi(s)=\int_0^s\frac{dt}{[G_0:G_t]},\qquad \psi=\varphi^{-1},
$$

extending $\varphi(s)=s$ on $[-1,0]$. The [upper ramification numbering](../../../../../upper-ramification-numbering.md) is $G^u=G_{\psi(u)}$ for $u\geq-1$.

Let $\alpha^p-\alpha=t^{1-p}$ over $K=\mathbb F_p((t))$, with $t$ its [uniformizer](../../../../../uniformizer.md). The [Artin–Schreier polynomial](../../../../../artin-schreier-polynomial.md) has derivative $-1$ in characteristic $p$, so all its roots are distinct. If $\alpha$ is one root and $\beta$ another, then $(\beta-\alpha)^p=\beta-\alpha$, so $\beta-\alpha\in\mathbb F_p$. Conversely every $\alpha+a$, $a\in\mathbb F_p$, is a root. Thus $L=K(\alpha)$ contains all roots and is a [splitting field](../../../../../splitting-field.md) of a separable [polynomial](../../../../../polynomial-split.md); it is Galois. Every automorphism has the form $\sigma_a(\alpha)=\alpha+a$, and its [Galois group](../../../../../galois-group.md) embeds in the additive group of $\mathbb F_p$.

There is no root in $K$. If $v_K(z)\geq0$, then $z^p-z$ cannot have negative [valuation](../../../../../valuation.md). If $v_K(z)<0$, the [ultrametric inequality](../../../../../ultrametric-inequality.md) gives $v_K(z^p-z)=p\,v_K(z)$, divisible by $p$, whereas $v_K(t^{1-p})=1-p$ is not. The [Galois group](../../../../../galois-group.md) is consequently nontrivial. Its order divides the prime $p$, so

$$
\boxed{[L:K]=p,\qquad G\cong(\mathbb F_p,+).}
$$

Let $e=e(L/K)$ be the [ramification index](../../../../../ramification-index.md). The equation forces $v_L(\alpha)<0$, and hence

$$
p\,v_L(\alpha)=(1-p)e.
$$

As $\gcd(p,p-1)=1$, $p\mid e$. Since $e\leq[L:K]=p$, we get $e=p$, [residue-field degree](../../../../../residue-field-degree.md) one, and $v_L(\alpha)=1-p$. Thus this is a [totally ramified extension](../../../../../totally-ramified-extension.md), and

$$
\pi_L=t\alpha\qquad\text{has }v_L(\pi_L)=p+(1-p)=1.
$$

This is a [uniformizer](../../../../../uniformizer.md). The [uniformizer criterion for lower ramification groups](../../../../../uniformizer-criterion-for-lower-ramification-groups.md) states that for a totally ramified [Galois extension](../../../../../finite-galois-extension.md), $\sigma\in G_i$ exactly when $v_L(\sigma(\pi_L)-\pi_L)\geq i+1$. Here every nonidentity automorphism satisfies

$$
\sigma_a(\pi_L)-\pi_L=a t,\qquad v_L(a t)=p.
$$

Therefore the [ramification break of an Artin–Schreier pole](../../../../../ramification-break-of-an-artin-schreier-pole.md) occurs at $p-1$, and the lower groups are

$$
\boxed{G_i=G\quad(-1\leq i\leq p-1),\qquad G_i=\{1\}\quad(i\geq p).}
$$

This includes $p=2$, where the break is one. There is no off-by-one shift: the condition is $v_L(\sigma\pi_L-\pi_L)\geq i+1$.

For the upper groups, compute the [Herbrand function](../../../../../herbrand-function.md) explicitly:

$$
\varphi(s)=\begin{cases}s,&0\leq s\leq p-1,\\p-1+\dfrac{s-(p-1)}p,&s\geq p-1.\end{cases}
$$

Hence the upper break is also $p-1$ and, with the stated real-index convention,

$$
\boxed{G^u=G\quad(-1\leq u\leq p-1),\qquad G^u=\{1\}\quad(u>p-1).}
$$

As a consistency check, $\pi_L$ satisfies the [Eisenstein polynomial](../../../../../eisenstein-polynomial.md) $X^p-t^{p-1}X-t$. Its derivative in characteristic $p$ is $-t^{p-1}$, giving different exponent $p(p-1)$, equal to $\sum_{i\geq0}(|G_i|-1)=p(p-1)$ from the [different exponent from ramification groups](../../../../../different-exponent-from-ramification-groups.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 136](../../paper-136-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
