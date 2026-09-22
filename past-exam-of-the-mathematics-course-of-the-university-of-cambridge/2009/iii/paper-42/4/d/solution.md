<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The barred notation denotes the antichiral [supersymmetric covariant derivative](../../../../../../supersymmetric-covariant-derivative.md). Write barred spinor indices as dotted indices, and use the stated plus-sign convention with [left Grassmann derivatives](../../../../../../left-grassmann-derivative.md):

$$
\bar D_{\dot\alpha}=\partial_{\bar\theta^{\dot\alpha}}+i\theta^\beta\sigma^\mu_{\beta\dot\alpha}\partial_\mu,\qquad
D_\alpha=\partial_{\theta^\alpha}+i\sigma^\mu_{\alpha\dot\beta}\bar\theta^{\dot\beta}\partial_\mu.
$$

Their [supercovariant derivative algebra with left derivatives](../../../../../../supercovariant-derivative-algebra-with-left-derivatives.md) gives $\{\bar D_{\dot\alpha},\bar D_{\dot\beta}\}=0$ and $\{D_\alpha,\bar D_{\dot\beta}\}=2i\sigma^\mu_{\alpha\dot\beta}\partial_\mu$. The constraint $\boxed{\bar D_{\dot\alpha}\Phi=0}$ defines a [chiral superfield](../../../../../../chiral-superfield.md), also called an [L-superfield](../../../../../../chiral-superfield.md).

To solve the constraint, put $y^\mu=x^\mu+i\theta\sigma^\mu\bar\theta$. For a [left Grassmann derivative](../../../../../../left-grassmann-derivative.md), $\partial_{\bar\theta^{\dot\alpha}}(\theta\sigma^\mu\bar\theta)=-\theta^\beta\sigma^\mu_{\beta\dot\alpha}$. Therefore $\bar D_{\dot\alpha}y^\mu=0$ and $\bar D_{\dot\alpha}\theta^\beta=0$, so $\bar D$ becomes ordinary differentiation with respect to $\bar\theta$ at fixed $y$. Its general solution is the [chiral-superfield component expansion](../../../../../../chiral-superfield-component-expansion.md)

$$
\boxed{\Phi=\Phi(y,\theta)=A(y)+\sqrt2\theta^\alpha\chi_\alpha(y)+\theta\theta F(y).}
$$

Here $A$ is a complex scalar, $\chi$ a [Weyl spinor](../../../../../../weyl-spinor.md), and $F$ a complex [auxiliary field](../../../../../../auxiliary-field.md). Before imposing field [equations of motion](../../../../../../equation-of-motion.md) this is four real bosonic and four real fermionic components. Chirality means independence of $\bar\theta$ at fixed $y$, rather than at fixed $x$. The differential [supercharges](../../../../../../supersymmetry-generator.md) $Q_\alpha=\partial_{\theta^\alpha}-i\sigma^\mu_{\alpha\dot\beta}\bar\theta^{\dot\beta}\partial_\mu$ and $\bar Q_{\dot\alpha}=\partial_{\bar\theta^{\dot\alpha}}-i\theta^\beta\sigma^\mu_{\beta\dot\alpha}\partial_\mu$ anticommute with both covariant derivatives, so a [supersymmetry](../../../../../../supersymmetry-split.md) transformation preserves the chiral constraint.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
