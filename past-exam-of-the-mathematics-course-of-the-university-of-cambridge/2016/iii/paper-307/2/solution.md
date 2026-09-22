<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

All derivatives below are [left Grassmann derivatives](../../../../../left-grassmann-derivative.md). Decompose the [supersymmetric covariant derivatives](../../../../../supersymmetric-covariant-derivative.md) into odd pieces

$$
D_\alpha=\partial_\alpha+A_\alpha,\qquad
\bar D_{\dot\beta}=\bar\partial_{\dot\beta}+B_{\dot\beta},
\qquad
A_\alpha=i\sigma^\mu_{\alpha\dot\gamma}\bar\theta^{\dot\gamma}\partial_\mu,
\quad B_{\dot\beta}=i\theta^\gamma\sigma^\mu_{\gamma\dot\beta}\partial_\mu.
$$

When these operators act on an arbitrary [superfield](../../../../../superfield.md), the [graded Leibniz rule](../../../../../graded-leibniz-rule.md) gives

$$
\{\partial_\alpha,B_{\dot\beta}\}=i\sigma^\mu_{\alpha\dot\beta}\partial_\mu,
\qquad
\{A_\alpha,\bar\partial_{\dot\beta}\}=i\sigma^\mu_{\alpha\dot\beta}\partial_\mu.
$$

The [anticommutator](../../../../../anticommutator.md) of the two pure Grassmann derivatives vanishes. Also $\{A_\alpha,B_{\dot\beta}\}=0$: the spacetime derivatives commute, while the $\theta$ and $\bar\theta$ coefficients anticommute. Adding these terms proves the [supercovariant derivative algebra with left derivatives](../../../../../supercovariant-derivative-algebra-with-left-derivatives.md),

$$
\boxed{\{D_\alpha,\bar D_{\dot\beta}\}=2i\sigma^\mu_{\alpha\dot\beta}\partial_\mu}.
$$

For two unbarred derivatives, neither $\partial_\alpha$ differentiates the $\bar\theta$ coefficient of the other operator. Their coefficient products anticommute, so $\boxed{\{D_\alpha,D_\beta\}=0}$. The same argument with barred and unbarred coordinates exchanged gives $\boxed{\{\bar D_{\dot\alpha},\bar D_{\dot\beta}\}=0}$. These signs follow the derivatives printed in this paper; a convention replacing $\bar D$ by $-\bar D$ reverses the mixed sign as well.

Set $y^\mu=x^\mu+i\theta^\alpha\sigma^\mu_{\alpha\dot\beta}\bar\theta^{\dot\beta}$. Left differentiation gives

$$
\bar\partial_{\dot\alpha}(\theta\sigma^\mu\bar\theta)
=-\theta^\beta\sigma^\mu_{\beta\dot\alpha},
\qquad\bar D_{\dot\alpha}y^\mu=0.
$$

The [chain rule](../../../../../chain-rule.md) therefore makes $\bar D_{\dot\alpha}$ simply $\bar\partial_{\dot\alpha}$ at fixed $y,\theta$. The [chiral superfield](../../../../../chiral-superfield.md) constraint $\bar D_{\dot\alpha}\Phi=0$ means that $\Phi$ is independent of $\bar\theta$ in these coordinates. Since there are only two independent entries of $\theta$, its [Grassmann algebra](../../../../../grassmann-algebra.md) expansion terminates at degree two. Naming the coefficients gives the [chiral-superfield component expansion](../../../../../chiral-superfield-component-expansion.md)

$$
\boxed{\Phi(y,\theta)=\phi(y)+\sqrt2\theta\psi(y)+\theta\theta F(y)}.
$$

Here $\phi$ is a [complex scalar field](../../../../../complex-scalar-field.md), $\psi$ a [Weyl spinor](../../../../../weyl-spinor.md), and $F$ a nonpropagating [auxiliary field](../../../../../auxiliary-field.md); the $\sqrt2$ is their conventional normalization.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 307](../../paper-307-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
