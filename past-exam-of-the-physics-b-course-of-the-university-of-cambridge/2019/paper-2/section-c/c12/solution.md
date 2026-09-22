<h1 id="section-c/c12/solution">Solution</h1>

↑ **Parent:** [C12](../c12.md)

**Configuration count.** Choose the end-to-end direction as positive and let $N_R,N_L$ count rightward and leftward links. Then

$$
N_R+N_L=N,\qquad a(N_R-N_L)=L,
\qquad N_R=\frac{N+L/a}{2},\quad N_L=\frac{N-L/a}{2}.
$$

A configuration is determined by choosing the positions of its leftward links, so

$$
\boxed{\Omega(L)=\frac{N!}{N_R!N_L!}.}
$$

The counts must be nonnegative integers; in particular, allowed signed extensions occur in steps of $2a$. If distance means $|L|$ with neither direction selected, there are two corresponding sets for $L>0$, adding a factor of two. That constant does not affect the [tension](../../../../../tension.md). There is no excluded-volume penalty in this one-dimensional idealized count.

**[Entropy](../../../../../entropy-split.md) from the multiplicity.** Put $x=L/(Na)$, so $|x|<1$. Applying the leading [Stirling's approximation](../../../../../stirling-formula.md) to all three large factorials gives

$$
S=k_B\ln\Omega\simeq k_B[N\ln N-N_R\ln N_R-N_L\ln N_L]
$$



$$
\boxed{S(x)\simeq Nk_B\ln2-\frac{Nk_B}{2}
\left[(1+x)\ln(1+x)+(1-x)\ln(1-x)\right].}
$$

Terms subleading in $N$, including logarithmic factorial prefactors, have been omitted consistently. Expanding near zero extension gives

$$
S(L)\simeq Nk_B\ln2-\frac{k_BL^2}{2Na^2}
+O\left(Nk_Bx^4\right).
$$

Stretching reduces the number of available configurations and hence the [entropy](../../../../../entropy-split.md).

**[Tension](../../../../../tension.md) and the range of [Hooke's law](../../../../../hooke-s-law.md).** The model assigns no extension-dependent [internal energy](../../../../../internal-energy-split.md). At fixed [temperature](../../../../../temperature-split.md), the externally applied [tension](../../../../../tension.md) is $\mathcal F=(\partial F/\partial L)_T=-T(\partial S/\partial L)_T$. Differentiating the full leading [entropy](../../../../../entropy-split.md) gives

$$
\boxed{\mathcal F=\frac{k_BT}{2a}\ln\frac{1+x}{1-x}
=\frac{k_BT}{a}\operatorname{artanh}x.}
$$

It is the external [force](../../../../../force-split.md) needed to oppose the chain's restoring [entropic force](../../../../../entropic-force.md). Only when $|L|\ll Na$ can one put $\operatorname{artanh}x\simeq x$, yielding

$$
\boxed{\mathcal F\simeq\frac{k_BT}{Na^2}L,\qquad |L|\ll Na.}
$$

The paper's displayed linear law therefore requires this small-extension approximation, which is not explicitly stated in its premise $L<L_0$. It is not the exact [force](../../../../../force-split.md) law up to full extension. The entropic spring constant grows with [temperature](../../../../../temperature-split.md) because stronger thermal disorder makes a given reduction in configurational [entropy](../../../../../entropy-split.md) cost more free [energy](../../../../../energy-split.md). This is the [one-dimensional entropic chain force-extension relation](../../../../../one-dimensional-entropic-chain-force-extension-relation.md).

**A sparse number of backward links.** Write $q=N_L\ll N$, so $N_R=N-q$ and $L=a(N-2q)$. Exactly,

$$
\Omega=\frac{N(N-1)\cdots(N-q+1)}{q!}
=\frac{N^q}{q!}\prod_{j=0}^{q-1}\left(1-\frac jN\right).
$$

For fixed $q$ and large $N$, each numerator factor approaches $N$, giving

$$
\boxed{\Omega\simeq\frac{N^{N_L}}{N_L!}.}
$$

More precisely, the [logarithm](../../../../../logarithm.md) of the product is $-q(q-1)/(2N)+O(q^3/N^2)$. A small relative error in the multiplicity requires $q^2/N\ll1$; merely $q/N\ll1$ need not make the omitted product close to one. The weaker sparse-link condition does suffice for the leading [entropy](../../../../../entropy-split.md) density and leading high-extension [tension](../../../../../tension.md). These are [sparse backward links near full chain extension](../../../../../sparse-backward-links-near-full-chain-extension.md).

**[Tension](../../../../../tension.md) in that limit.** In the overlap regime $1\ll q\ll N$, use Stirling also for $q!$:

$$
S\simeq k_B[q\ln N-q\ln q+q],\qquad
\frac{dq}{dL}=-\frac1{2a}.
$$

Thus

$$
\boxed{\mathcal F\simeq\frac{k_BT}{2a}\ln\frac N{N_L}.}
$$

The full leading [entropy](../../../../../entropy-split.md) would give $(k_BT/(2a))\ln[(N-N_L)/N_L]$, which has the same dominant [logarithm](../../../../../logarithm.md) when $N_L/N\to0$.

**Approaching full extension.** The continuum [force](../../../../../force-split.md) law diverges logarithmically as $N_L\to0$, or $L\to Na$. One must not literally apply Stirling to a zero factorial: at the discrete endpoint there is exactly one directed configuration, $\Omega=1$, and its [entropy](../../../../../entropy-split.md) is zero. A continuous fixed-extension [derivative](../../../../../derivative.md) is not defined at that endpoint.

An independent force-ensemble calculation makes the limiting physical statement precise. For applied [tension](../../../../../tension.md) $\mathcal F$, a link has [partition function](../../../../../canonical-partition-function.md) $z=2\cosh(\beta\mathcal Fa)$, giving the exact [mean](../../../../../expected-value-split.md) extension

$$
\boxed{\langle L\rangle=Na\tanh(\beta\mathcal Fa).}
$$

It approaches $Na$ only as $\mathcal F\to\infty$ at positive [temperature](../../../../../temperature-split.md), and inversion reproduces the logarithmic [force](../../../../../force-split.md) law for [mean](../../../../../expected-value-split.md) extension. In a real chain, bond extension or failure eventually replaces the ideal inextensible-link model.

## ↑ Ancestors (14)

1. [C12](../c12.md)
2. [Section C](../../section-c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
