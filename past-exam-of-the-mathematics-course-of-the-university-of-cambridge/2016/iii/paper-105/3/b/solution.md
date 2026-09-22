<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $B=-A=-\partial_x^2+1+x^2$. Smooth compactly supported functions lie in $D(A)$ and are dense in [L2 space](../../../../../../l2-space-is-a-hilbert-space.md), so $A$ is densely defined.

For $\lambda>0$, use the form

$$
a_\lambda(u,v)=\int_{\mathbb R}u'\overline{v'}+(1+\lambda+x^2)u\bar v\,dx
$$

on the [one-dimensional harmonic oscillator form domain](../../../../../../one-dimensional-harmonic-oscillator-form-domain.md) $X$. It is bounded and coercive in the $X$ norm. The [Lax-Milgram theorem](../../../../../../lax-milgram-theorem.md) gives a unique $u\in X$ satisfying $a_\lambda(u,v)=\langle g,v\rangle$ for every $v\in X$. Thus $-u''+(1+\lambda+x^2)u=g$ in [distributions](../../../../../../distribution-mathematical-analysis.md).

We must verify the full specified [operator domain](../../../../../../operator-domain.md), not just the form domain. The equation first gives $u\in H^2_{\mathrm{loc}}$. For compactly supported $H^2$ functions, [integration by parts](../../../../../../integration-by-parts.md) gives the [graph estimate for the harmonic oscillator](../../../../../../graph-estimate-for-the-harmonic-oscillator.md), obtained from

$$
\begin{aligned}
\|-v''+(1+\lambda+x^2)v\|_2^2
={}&\|v''\|_2^2+\|(1+\lambda+x^2)v\|_2^2\\
&+2\int(1+\lambda+x^2)|v'|^2\,dx-2\|v\|_2^2.
\end{aligned}
$$

Apply this to $v=\chi_Ru$, with $\chi_R=1$ on $[-R,R]$, supported in $[-2R,2R]$, and derivatives bounded by $C/R$ and $C/R^2$. Its right-hand source is $\chi_Rg-2\chi_R'u'-\chi_R''u$, uniformly bounded in [L2 space](../../../../../../l2-space-is-a-hilbert-space.md). The estimate and the [Fatou lemma](../../../../../../fatou-s-lemma.md) give $x^2u\in L^2$; the original equation then gives $u''\in L^2$, and hence $u\in H^2$. Thus $u\in D(A)$, proving that $\lambda-A$ is onto. The energy identity proves injectivity and the [resolvent of the shifted harmonic oscillator](../../../../../../resolvent-of-the-shifted-harmonic-oscillator.md) estimate

$$
(1+\lambda)\|u\|_2^2\leq a_\lambda(u,u)=\operatorname{Re}\langle g,u\rangle
\leq\|g\|_2\|u\|_2,
\qquad
\boxed{\|(\lambda-A)^{-1}\|_{2\to2}\leq\frac1{1+\lambda}.}
$$

To prove closedness, suppose $u_n\to u$ and $Au_n\to v$ in [L2 space](../../../../../../l2-space-is-a-hilbert-space.md). For one fixed $\lambda>0$,

$$
u_n=(\lambda-A)^{-1}(\lambda u_n-Au_n)\longrightarrow(\lambda-A)^{-1}(\lambda u-v).
$$

Therefore $u$ belongs to the range of the resolvent, namely $D(A)$, and $Au=v$.

All hypotheses of the [Hille-Yosida theorem](../../../../../../hille-yosida-theorem.md) now hold; the resolvent bound is stronger than $1/\lambda$. Let $S(t)$ be its [contraction semigroup](../../../../../../contraction-semigroup.md). The [exponentially shifted semigroup](../../../../../../exponentially-shifted-semigroup.md)

$$
\boxed{\psi(t)=e^tS(t)\psi_0}
$$

has generator $A+I=\partial_x^2-x^2$. It is continuous in [L2 space](../../../../../../l2-space-is-a-hilbert-space.md), takes the initial value $\psi_0$, and satisfies $\boxed{\|\psi(t)\|_2\leq e^t\|\psi_0\|_2}$. For $\psi_0\in D(A)$, its time derivative exists in [L2 space](../../../../../../l2-space-is-a-hilbert-space.md) and equals $(A+I)\psi(t)$, so the equation holds as a strong [L2 space](../../../../../../l2-space-is-a-hilbert-space.md) solution. For general initial data it is the semigroup solution, without an unproved pointwise differentiability claim.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
