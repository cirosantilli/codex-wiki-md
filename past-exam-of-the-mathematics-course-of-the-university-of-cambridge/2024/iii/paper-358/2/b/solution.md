<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $E_n$ and $E$ be the [projection-valued measures](../../../../../../projection-valued-measure.md) of $A_n$ and $A$. Using the projection $P_n:\mathcal H\to\mathcal H_n$, define

$$
\mu^{(n)}_{v,w}(B)
=\langle E_n(B)P_nv,P_nw\rangle.
$$

The [scalar spectral measures](../../../../../../scalar-spectral-measure.md) converge weakly when

$$
\boxed{
\int_{\mathbb R}f\,d\mu^{(n)}_{v,w}
\longrightarrow
\int_{\mathbb R}f\,d\mu_{v,w}}
$$

for every bounded [continuous function](../../../../../../continuous-function.md) $f$ and every $v,w\in\mathcal H$. By the [spectral theorem for normal operators on a separable Hilbert space](../../../../../../spectral-theorem-for-normal-operators-on-a-separable-hilbert-space.md), this is equivalent to

$$
\langle f(A_n)P_nv,P_nw\rangle
\longrightarrow
\langle f(A)v,w\rangle.
$$

The assumed moment identities say precisely that this convergence holds for every monomial $f(x)=x^m$. It follows by [linearity](../../../../../../linearity.md) for every [polynomial](../../../../../../polynomial-split.md). For $v=w$, the $m=2$ identity gives

$$
\int x^2\,d\mu^{(n)}_v(x)\longrightarrow
\int x^2\,d\mu_v(x),
$$

so [Markov inequality](../../../../../../markov-inequality.md) makes the positive measures $(\mu^{(n)}_v)$ tight. Higher even moments similarly control the tails of any fixed polynomial.

Given a bounded continuous $f$ and $\epsilon>0$, choose $R$ so that the measure tails are uniformly small. The [Weierstrass approximation theorem](../../../../../../weierstrass-approximation-theorem.md) supplies a polynomial $p$ with

$$
\sup_{|x|\leq R}|f(x)-p(x)|<\epsilon.
$$

Moment convergence handles $p$; tightness and a sufficiently high even moment handle the two tails. Hence $\int f\,d\mu_v^{(n)}\to\int f\,d\mu_v$. The [polarization identity](../../../../../../polarization-identity.md) then gives the same conclusion for $\mu_{v,w}^{(n)}$. This proves [weak convergence of scalar spectral measures](../../../../../../weak-convergence-of-scalar-spectral-measures.md).

The assertion fails if only $m=1$ is assumed. Let $\mathcal H=\ell^2(\mathbb N)$, let $\mathcal H_n=\operatorname{span}\{e_1,\ldots,e_n\}$, take $A=0$, and let

$$
A_ne_j=e_{n+1-j}
\qquad(1\leq j\leq n).
$$

The reversal matrices are self-adjoint unitaries. For fixed $v,w\in\ell^2$,

$$
\langle A_nP_nv,P_nw\rangle\longrightarrow0,
$$

because the finite head of one vector is paired with the vanishing tail of the other. Thus the $m=1$ condition holds. However, $A_n^2=I_{\mathcal H_n}$, so

$$
\langle A_n^2P_nv,P_nw\rangle
\longrightarrow\langle v,w\rangle
\ne0=\langle A^2v,w\rangle
$$

in general. Taking $f(x)=x^2$ shows that the spectral measures do not converge weakly.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 358](../../../paper-358-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
