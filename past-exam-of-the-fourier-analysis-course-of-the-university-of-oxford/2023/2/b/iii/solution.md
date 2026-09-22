<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $U=\widehat u$, $V=\widehat v$, and $\langle\xi\rangle=(1+\xi^2)^{1/2}$. By the [Sobolev space](../../../../../sobolev-space-split.md) hypotheses, $A=\langle\xi\rangle^sU$ and $B=\langle\xi\rangle^tV$ belong to the [L2 space](../../../../../l2-space-is-a-hilbert-space.md). Their product is an [integrable function](../../../../../lebesgue-integrable-function.md) by [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md). Thus $UV=\langle\xi\rangle^{-s-t}AB$ is a [locally integrable function](../../../../../locally-integrable-function.md) defining a [tempered distribution](../../../../../tempered-distribution.md), with estimate

$$
\left|\int UV\phi\,d\xi\right|
\leq\|u\|_{H^s}\|v\|_{H^t}
\sup_\xi\bigl(\langle\xi\rangle^{-s-t}|\phi(\xi)|\bigr).
$$

The supremum is controlled by finitely many [Schwartz seminorms](../../../../../schwartz-seminorm.md). Define the [convolution of Sobolev distributions](../../../../../convolution-of-sobolev-distributions.md) by

$$
\boxed{u*v:=\mathcal F^{-1}(UV)\in\mathcal S'(\mathbb R).}
$$

It is independent of the representatives chosen for $U,V$, and the [convolution theorem](../../../../../convolution-theorem.md) shows that it agrees with ordinary [convolution](../../../../../convolution.md) for [Schwartz functions](../../../../../schwartz-function.md). More generally, approximate $u,v$ by [Schwartz functions](../../../../../schwartz-function.md) in their respective [Sobolev norms](../../../../../sobolev-norm.md); the displayed estimate shows convergence of the products in [tempered distributions](../../../../../tempered-distribution.md), so their ordinary [convolutions](../../../../../convolution.md) converge to this definition. For $u,v\in L^1$ that also satisfy the stated [Sobolev space](../../../../../sobolev-space-split.md) hypotheses, the ordinary [convolution theorem](../../../../../convolution-theorem.md) gives the same result.

There need not be any real $r$ with $u*v\in H^r(\mathbb R)$. Choose

$$
U(\xi)=V(\xi)=\xi^{-1/3}\mathbf1_{(0,1)}(\xi),\qquad
u=\mathcal F^{-1}U,\quad v=\mathcal F^{-1}V.
$$

Here $\mathbf1_{(0,1)}$ is an [indicator function](../../../../../indicator-function.md). Since $\int_0^1\xi^{-2/3}\,d\xi=3$ and every weight $(1+\xi^2)^q$ is bounded above and below by positive constants on $[0,1]$, both $u$ and $v$ belong to every [Sobolev space](../../../../../sobolev-space-split.md). But their [convolution](../../../../../convolution.md) has [Fourier transform](../../../../../fourier-transform-split.md) $UV=\xi^{-2/3}\mathbf1_{(0,1)}$, and for every real $r$,

$$
\int(1+\xi^2)^r|UV|^2\,d\xi
\geq\min(1,2^r)\int_0^1\xi^{-4/3}\,d\xi=\infty.
$$

Thus $\boxed{u,v\in\bigcap_{q\in\mathbb R}H^q(\mathbb R)\quad\text{but}\quad u*v\notin\bigcup_{r\in\mathbb R}H^r(\mathbb R)}$. The obstruction is failure of local square integrability at zero; a weight controlling large [frequencies](../../../../../frequency.md) cannot fix it.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the fourier analysis course of the University of Oxford](../../../../split.md)
6. [Fourier analysis course of the University of Oxford](../../../../../fourier-analysis-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
