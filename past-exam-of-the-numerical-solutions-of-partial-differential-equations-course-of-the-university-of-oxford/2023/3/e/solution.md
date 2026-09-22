<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

When $a=0$, the explicit [amplification factor](../../../../amplification-factor.md) becomes

$$
G_E(\theta)=1-i\nu\sin\theta,\qquad |G_E(\theta)|^2=1+\nu^2\sin^2\theta.
$$

A single [Fourier mode](../../../../fourier-mode.md) has constant modulus in space and is not in the [l2 sequence space](../../../../l2-sequence-space.md). Instead choose a whole interval of frequencies on which there is definite growth. Let

$$
E=[\pi/4,3\pi/4]\cup[-3\pi/4,-\pi/4],\qquad\widehat U^0(\theta)=\mathbf1_E(\theta).
$$

The [inverse Fourier transform](../../../../inverse-fourier-transform.md) here gives the real [sequence](../../../../sequence.md)

$$
U_j^0=\begin{cases}
\dfrac{\sin(3\pi j/4)-\sin(\pi j/4)}{\pi j},&j\ne0,\\
\dfrac12,&j=0.
\end{cases}
$$

By the [Parseval identity](../../../../parseval-identity.md), its squared [norm](../../../../norm.md) is $\|U^0\|_{\ell_2}^2=\Delta x\,|E|/(2\pi)=\Delta x/2$, finite and strictly positive. These data are also compatible with sampling a bounded [continuous function](../../../../continuous-function.md): use

$$
u_0(x)=\begin{cases}
\dfrac{\sin(3\pi x/(4\Delta x))-\sin(\pi x/(4\Delta x))}{\pi x/\Delta x},&x\ne0,\\
\dfrac12,&x=0.
\end{cases}
$$

The value at zero is the [limit](../../../../limit-of-a-function.md) of the displayed quotient, and $u_0(j\Delta x)=U_j^0$.

On $E$ we have $\sin^2\theta\geq1/2$. Therefore the transformed solution and the [Parseval identity](../../../../parseval-identity.md) give

$$
\begin{aligned}
\|U^m\|_{\ell_2}^2
&=\frac{\Delta x}{2\pi}\int_E(1+\nu^2\sin^2\theta)^m\,d\theta\\
&\geq(1+\nu^2/2)^m\|U^0\|_{\ell_2}^2.
\end{aligned}
$$

For each fixed pair $\Delta x,\Delta t>0$, take

$$
\boxed{c(\Delta x,\Delta t)=\sqrt{1+\frac12\left(\frac{\Delta t}{\Delta x}\right)^2}-1>0.}
$$

Taking square roots proves $\|U^m\|_{\ell_2}\geq(1+c)^m\|U^0\|_{\ell_2}$ for every $m\geq1$. In particular the [norm](../../../../norm.md) already increases at the first step, so **no positive mesh pair gives practical stability** in the contraction sense of (b).

The native PDF places the existence of $c>0$ before the universal quantifier over mesh pairs. If this means a single positive $c$ independent of $\Delta x,\Delta t$, that assertion is false for nonzero data. Indeed, for every datum the same [Fourier symbol](../../../../fourier-symbol-of-a-difference-operator.md) gives

$$
\|U^1\|_{\ell_2}\leq\sqrt{1+\nu^2}\,\|U^0\|_{\ell_2}.
$$

For any proposed fixed $c>0$, choose $0<\nu<\sqrt{(1+c)^2-1}$. The upper bound then contradicts the requested lower bound at $m=1$. The correct quantifiers are $\forall\Delta x,\Delta t>0\ \exists c=c(\Delta x,\Delta t)>0$, with nonzero square-summable data as constructed above.

Finally, failure of this stronger [practical stability of a finite difference scheme](../../../../practical-stability-of-a-finite-difference-scheme.md) should not be confused with every possible refinement notion of [numerical stability](../../../../stability-of-a-numerical-method.md). If $\Delta t/(\Delta x)^2\leq K$, then $m\Delta t\leq T$ gives

$$
|G_E(\theta)|^m\leq\exp(m\nu^2/2)\leq\exp(KT/2).
$$

Thus a finite-time mesh-uniform bound can hold under this severe refinement even though contraction fails on every positive mesh. This is the distinction recorded in [centered-advection refinement-dependent stability](../../../../centered-advection-refinement-dependent-stability.md).

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the numerical solutions of partial differential equations course of the University of Oxford](../../../split.md)
5. [Numerical solutions of partial differential equations course of the University of Oxford](../../../../numerical-solutions-of-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
