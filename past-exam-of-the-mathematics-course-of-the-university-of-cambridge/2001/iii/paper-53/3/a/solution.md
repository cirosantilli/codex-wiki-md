<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

At a current approximation $p$, [Taylor's theorem](../../../../../../taylor-theorem.md) replaces $\Phi(p+h)=0$ by the affine equation $\Phi(p)+D\Phi(p)h=0$. Solving this equation gives the [Newton iteration in a Banach space](../../../../../../newton-iteration-in-a-banach-space.md)

$$
\boxed{N(p)=p-[D\Phi(p)]^{-1}\Phi(p),\qquad p_{n+1}=N(p_n).}
$$

The inverse is a bounded linear inverse by the [bounded inverse theorem](../../../../../../bounded-inverse-theorem.md). The displayed operator is defined where the [derivative](../../../../../../derivative.md) is invertible, in particular on the specified open domain; the hypotheses do not supply a globally defined Newton operator on all of $\mathcal X$. If $\Phi(\bar p)=0$ with $\bar p$ in that domain, then $N(\bar p)=\bar p$.

For [quadratic convergence](../../../../../../quadratic-convergence.md), choose a sufficiently small neighbourhood of $\bar p$. Continuity of the inverse [derivative](../../../../../../derivative.md) and of $D^2\Phi$ gives constants $M,L$ there such that

$$
\|[D\Phi(p)]^{-1}\|\leq M,\qquad
\|D\Phi(p)-D\Phi(q)\|\leq L\|p-q\|.
$$

Put $e=p-\bar p$ and $B(p)=[D\Phi(p)]^{-1}$. The [quadratic Newton error bound in a Banach space](../../../../../../quadratic-newton-error-bound-in-a-banach-space.md) follows from the integral remainder:

$$
\begin{aligned}
N(p)-\bar p
&=B(p)\{D\Phi(p)e-[\Phi(p)-\Phi(\bar p)]\}\\
&=B(p)\int_0^1\{D\Phi(p)-D\Phi(\bar p+te)\}e\,dt,
\end{aligned}
$$

so

$$
\boxed{\|N(p)-\bar p\|\leq C\|p-\bar p\|^2,\qquad C=ML/2.}
$$

Take a closed radius-$r$ ball lying in the neighbourhood with $Cr<1$. This inequality maps the ball into itself and makes errors tend to zero. More explicitly, for $e_n=\|p_n-\bar p\|$, induction gives $Ce_{n+j}\leq(Ce_n)^{2^j}$. Hence every sufficiently close initial point converges to $\bar p$ at least quadratically; special maps can converge still faster.

For a fixed-point equation, apply the same method to $F(p)=\Phi(p)-p$. Wherever $D\Phi(p)-I$ is invertible, the exact adapted map is

$$
\boxed{A(p)=p-[D\Phi(p)-I]^{-1}[\Phi(p)-p].}
$$

Every [fixed point](../../../../../../fixed-point.md) of $\Phi$ is fixed by $A$, and conversely on this domain. This additional invertibility condition is distinct from invertibility of $D\Phi$; for example, $D\Phi=I$ is invertible but $D\Phi-I=0$ is not.

For certification, a [frozen Newton correction for a fixed-point equation](../../../../../../frozen-newton-correction-for-a-fixed-point-equation.md) is often more useful. Choose a bounded, injective approximate inverse $J$ of $D\Phi(p_0)-I$ and set

$$
A_J(p)=p-J[\Phi(p)-p],\qquad
DA_J(p)=I-J[D\Phi(p)-I].
$$

Again $A_J(p)=p$ if and only if $\Phi(p)=p$. A well-chosen $J$ makes the corrected operator contract even if the original operator has an expanding direction. The subsequent [contraction mapping](../../../../../../contraction-mapping.md) argument requires the stated [derivative](../../../../../../derivative.md) and residual bounds; it does not assume that arbitrary inverse approximations provide them.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
