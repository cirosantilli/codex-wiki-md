<h1 id="16d/solution">Solution</h1>

↑ **Parent:** [16D](../16d.md)

Taking the vertical component of the curl of the [momentum](../../../../../momentum.md) equation gives

$$
\omega_t+f\nabla\cdot\mathbf u=0.
$$

The continuity equation gives $\eta_t+h_0\nabla\cdot\mathbf u=0$, and hence

$$
\boxed{\frac\partial{\partial t}
\left(\omega-\frac f{h_0}\eta\right)=0}.
$$

Since initially $\mathbf u=0$ and $\eta=\eta_0$,

$$
\omega=\frac f{h_0}(\eta-\eta_0).
$$

Taking the divergence of the [momentum](../../../../../momentum.md) equation and using

$$
\nabla\cdot(\mathbf f\times\mathbf u)=-f\omega
$$

gives

$$
(\nabla\cdot\mathbf u)_t-f\omega=-g\nabla^2\eta.
$$

Differentiate continuity in time and substitute the last two identities to obtain

$$
\boxed{\eta_{tt}-gh_0\nabla^2\eta+f^2\eta=f^2\eta_0}.
$$

Let the [Rossby deformation radius](../../../../../rossby-deformation-radius.md) be

$$
L_R=\frac{\sqrt{gh_0}}{|f|}.
$$

The even, decaying steady solution of

$$
-L_R^2\eta_\infty''+\eta_\infty=\eta_0
$$

with continuous value and [derivative](../../../../../derivative.md) at $x=\pm a$ is

$$
\boxed{
\eta_\infty(x)=
\begin{cases}
\epsilon\left[1-e^{-a/L_R}\cosh(x/L_R)\right],&|x|<a,\\
\epsilon\sinh(a/L_R)e^{-|x|/L_R},&|x|>a.
\end{cases}}
$$

The steady [momentum](../../../../../momentum.md) balance is a [geostrophic balance](../../../../../geostrophic-balance.md):

$$
\boxed{u=0,
\qquad v=\frac g f\frac{d\eta_\infty}{dx}}.
$$

Thus the flow is parallel to the two edges of the raised strip, in opposite $y$-directions on the two sides; for $f>0$, it points toward $+y$ on the left and $-y$ on the right. Its magnitude is concentrated within a few deformation radii of the edges.

## ↑ Ancestors (10)

1. [16D](../16d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
