<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [dimensional analysis](../../../../../../dimensional-analysis.md)

$$
h=h^*H,\qquad
x=\ell X,\qquad
t=\frac{h^*}{\alpha}\,\mathcal T,
\qquad
\ell=\left(\frac{\rho g(h^*)^4}{3\mu\alpha}\right)^{1/2},
$$

and define the dimensionless sliding parameter

$$
\boxed{s=\frac{3\mu\beta}{\rho g(h^*)^2}}.
$$

The dimensionless flux and steady conservation law are

$$
Q=-(H^3+sH)H_X,
\qquad
Q_X=
\begin{cases}
+1,&H>1,\\
-1,&H<1.
\end{cases}
$$

On the right half-cap, let the [snowline](../../../../../../snowline.md) be $X=X_s$ and the nose be $X=X_n$. The zero-flux condition at the [ice divide](../../../../../../ice-divide.md) gives $Q=X$ in the accumulation region. Continuity of $Q$ gives $Q=2X_s-X$ in the ablation region, and zero nose flux gives

$$
\boxed{X_n=2X_s}.
$$

Introduce the increasing function

$$
\Phi(H)=\frac{H^4}{4}+\frac{sH^2}{2},
\qquad
\Phi'(H)=H^3+sH.
$$

Since $\Phi_X=-Q$, the ablation profile satisfying $H(X_n)=0$ is

$$
\boxed{\Phi(H)=\frac12(2X_s-X)^2},
\qquad X_s\leq X\leq2X_s.
$$

At the snowline $H=1$, so

$$
\boxed{X_s=\sqrt{\frac12+s}},
\qquad
\boxed{X_n=2\sqrt{\frac12+s}}.
$$

In the accumulation region,

$$
\boxed{\Phi(H)=2\Phi(1)-\frac{X^2}{2}},
\qquad 0\leq X\leq X_s,
$$

and the divide thickness $H_0$ is fixed by

$$
\boxed{\Phi(H_0)=2\Phi(1)=\frac12+s}.
$$

These two implicit formulas give a continuous thickness and flux at the snowline. Reflection across $X=0$ gives the full two-dimensional ice cap.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 332](../../../paper-332-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
