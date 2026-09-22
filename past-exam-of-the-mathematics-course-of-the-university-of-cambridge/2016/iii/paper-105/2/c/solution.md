<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Work with real-valued functions. The [screened sine-Gordon energy](../../../../../../screened-sine-gordon-energy.md) is well defined: $0\leq1-\cos u\leq u^2/2$, and $fu$ is integrable by the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). It is coercive, because

$$
E[u]\geq\tfrac12\|u\|_{H^1}^2-\|f\|_2\|u\|_2
\geq\tfrac14\|u\|_{H^1}^2-\|f\|_2^2.
$$

A minimizing sequence is bounded in the [Hilbert space](../../../../../../hilbert-space-split.md) $H^1$. [Weak sequential compactness of bounded sequences in a reflexive Banach space](../../../../../../weak-sequential-compactness-of-bounded-sequences-in-a-reflexive-banach-space.md) supplies a weakly convergent subsequence. The squared [H1 space](../../../../../../h1-space.md) norm is weakly lower semicontinuous, the source pairing is weakly continuous, and the nonlinear term is covered by [local Sobolev compactness gives lower semicontinuity of a nonnegative integral](../../../../../../local-sobolev-compactness-gives-lower-semicontinuity-of-a-nonnegative-integral.md). The [direct method in the calculus of variations](../../../../../../direct-method-in-the-calculus-of-variations.md) therefore gives a minimizer $\phi$.

Taking its [first variation](../../../../../../first-variation.md) in any $v\in H^1$ gives

$$
\int_{\mathbb R^3}\nabla\phi\cdot\nabla v+\phi v+\sin\phi\,v\,dx
=\int_{\mathbb R^3}fv\,dx.
$$

Thus the [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md) is

$$
\boxed{-\Delta\phi+\phi+\sin\phi=f,}
$$

as a [weak solution](../../../../../../weak-solution.md), equivalently in [distributions](../../../../../../distribution-mathematical-analysis.md) when tested against smooth compactly supported functions. The derivative of the nonlinear term is justified by $|\sin\phi|\leq|\phi|$ and the second-order remainder bound $|\cos|\leq1$.

Now $G=f-\sin\phi\in L^2$, so the supplied [elliptic regularity](../../../../../../elliptic-regularity.md) estimate puts $\phi$ in $H^2$. Applying the [Sobolev inequality](../../../../../../sobolev-inequality.md) to $\phi$ and each first [weak derivative](../../../../../../weak-derivative.md) gives $\phi\in W^{1,6}(\mathbb R^3)$. [Morrey's inequality](../../../../../../morrey-s-inequality.md) and [uniformly continuous integrable functions vanish at infinity](../../../../../../uniformly-continuous-integrable-functions-vanish-at-infinity.md) prove that its continuous representative tends to zero.

**The final printed supremum estimate is false in general.** The [maximum bound for a monotone reaction term](../../../../../../maximum-bound-for-a-monotone-reaction-term.md) involves $h(s)=s+\sin s$, which is odd and strictly increasing: $h'=1+\cos s\geq0$, and its zeros are isolated. If $M=\|f\|_\infty<\infty$, a positive maximum $m$ of $\phi$ satisfies $h(m)\leq f\leq M$; apply the same argument to $-\phi$. The valid general estimate is

$$
\boxed{\|\phi\|_\infty\leq h^{-1}(M)\leq M+1.}
$$

The bound by $M$ is valid if $M\leq\pi$, but $h(s)$ can be smaller than $s$ for larger positive $s$.

For an explicit [failure of the source-size bound for the screened sine-Gordon equation](../../../../../../failure-of-the-source-size-bound-for-the-screened-sine-gordon-equation.md), take $a=3\pi/2$, $L=10$, $\phi(x)=a e^{-|x|^2/L^2}$ and $f=-\Delta\phi+\phi+\sin\phi$. These are smooth functions in the required spaces. With $q=|x|^2/L^2$,

$$
|\Delta\phi|=\frac{a}{L^2}|4q-6|e^{-q}\leq\frac{6a}{L^2},
\qquad
0\leq h(\phi)\leq h(a)=a-1.
$$

Hence $\|f\|_\infty\leq a-1+6a/L^2<a=\|\phi\|_\infty$. Moreover $V(s)=s^2/2+1-\cos s$ has $V''=1+\cos s\geq0$, so the energy is convex and this critical point is a minimizer. The example therefore satisfies even the minimizing and $C^2$ hypotheses of the printed claim.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
