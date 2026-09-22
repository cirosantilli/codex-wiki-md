<h1 id="2/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Assume **$\operatorname{argmin}f\ne\varnothing$**, as is necessary for convergence to a minimizer. The printed hypotheses alone omit this condition: $f(x,y)=x$ in scalar $x$ is convex with an $L$-[Lipschitz gradient](../../../../../../lipschitz-gradient.md) for any prescribed $L>0$, but has no minimizer, and the update sends $x^k=x^0-k\tau$ to $-\infty$.

Under existence, define the full update $T(x,y)=(x^+,y^+)$. The proximal $y$-step is uniquely defined by strong convexity of its quadratic term and satisfies

$$
y-y^+=\tau\nabla_y f(x,y^+),\qquad x-x^+=\tau\nabla_x f(x,y^+).
$$

The [partial subdifferential](../../../../../../partial-subdifferential.md) in this equation belongs to the scalar function $y\mapsto f(x,y)$; differentiating a subdifferential itself would not define the printed proximal minimization.

We prove directly that the [alternating proximal-gradient operator](../../../../../../alternating-proximal-gradient-operator.md) $T$ is averaged. For two inputs $z=(x,y)$ and $\widetilde z=(\widetilde x,\widetilde y)$, set

$$
w=(x,y^+),\quad\widetilde w=(\widetilde x,\widetilde y^+),\quad
p=x-\widetilde x,\quad q=y^+-\widetilde y^+,\quad
(a,b)=\nabla f(w)-\nabla f(\widetilde w).
$$

The input difference is $(p,q+\tau b)$, the output difference is $(p-\tau a,q)$, and the difference of the two update residuals is $\tau(a,b)$. Exact expansion gives

$$
\begin{aligned}
\|Tz-T\widetilde z\|_2^2
&=\|z-\widetilde z\|_2^2-2\tau[\langle p,a\rangle+\langle q,b\rangle]
+\tau^2(\|a\|_2^2-\|b\|_2^2)\\
&\leq\|z-\widetilde z\|_2^2
-\left(\frac{2\tau}L-\tau^2\right)\|a\|_2^2
-\left(\frac{2\tau}L+\tau^2\right)\|b\|_2^2\\
&\leq\|z-\widetilde z\|_2^2
-\left(\frac2{\tau L}-1\right)\|(I-T)z-(I-T)\widetilde z\|_2^2.
\end{aligned}
$$

The first inequality uses [cocoercivity](../../../../../../cocoercivity.md) at the mixed points $w,\widetilde w$. Therefore **$T$ is $(\tau L/2)$-averaged** for the requested $0<\tau L\leq1$. In particular, the endpoint $\tau L=1$ is covered: $T$ is [firmly nonexpansive](../../../../../../firmly-nonexpansive-mapping.md), not merely nonexpansive.

A [fixed point](../../../../../../fixed-point.md) has $y^+=y$ and $x^+=x$, so the two optimality equations give $\nabla_y f=0$ and $\nabla_x f=0$. Conversely, at a minimizer both gradients vanish and neither step moves. By [convexity](../../../../../../convex-function.md),

$$
\boxed{\operatorname{Fix}T=\operatorname{argmin}f}.
$$

The assumed existence of a minimizer supplies a [fixed point](../../../../../../fixed-point.md). The [Browder convergence theorem for averaged operators](../../../../../../browder-convergence-theorem-for-averaged-operators.md) now gives

$$
\boxed{(x^k,y^k)\longrightarrow(x^*,y^*)\in\operatorname{argmin}f}.
$$

No uniqueness of the minimizer is needed. The same estimate even proves averagedness for $0<\tau L<2$ in this smooth setting, but the requested interval already suffices. The existence condition and the use of the gradient at $(x^k,y^{k+1})$ are both essential to the proof as presented.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [2](../../2.md)
3. [Paper 325](../../../paper-325-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
