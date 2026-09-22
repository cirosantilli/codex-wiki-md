<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a tangential [covector](../../../../../../covector.md), the projected [derivative](../../../../../../derivative.md) is $D_\nu W_\gamma=P^\beta{}_{\nu}P^\delta{}_{\gamma}\nabla_\beta W_\delta$. Its second [derivative](../../../../../../derivative.md) is

$$
D_\mu D_\nu W_\gamma
=P^\alpha{}_{\mu}P^\beta{}_{\nu}P^\delta{}_{\gamma}
\nabla_\alpha\left(P^\eta{}_{\beta}P^\kappa{}_{\delta}\nabla_\eta W_\kappa\right).
$$

Expanding by the [product rule](../../../../../../product-rule.md), the [derivative](../../../../../../derivative.md) of the first inner projector gives $K_{\mu\nu}n^\eta P^\kappa{}_{\gamma}\nabla_\eta W_\kappa$. This contribution cancels on antisymmetrizing $\mu,\nu$, because $K$ is symmetric.

The [derivative](../../../../../../derivative.md) of the second inner projector gives $K_{\mu\gamma}n^\kappa P^\eta{}_{\nu}\nabla_\eta W_\kappa$. Differentiating tangentiality, $n^\kappa W_\kappa=0$, rewrites it as

$$
K_{\mu\gamma}n^\kappa P^\eta{}_{\nu}\nabla_\eta W_\kappa
=-K_{\mu\gamma}K_\nu{}^\kappa W_\kappa.
$$

The remaining term is the projected four-dimensional curvature [commutator](../../../../../../commutator.md). Using the curvature convention of the question,

$$
[\nabla_\alpha,\nabla_\beta]W_\delta
=W_\xi\,{}^{(4)}R^\xi{}_{\delta\beta\alpha},
$$

and replacing the tangential $W_\xi$ by $W_\lambda P^\lambda{}_{\xi}$, we obtain

$$
[D_\mu,D_\nu]W_\gamma
=W_\lambda\left[
P^\lambda{}_{\xi}P^\alpha{}_{\mu}P^\beta{}_{\nu}P^\delta{}_{\gamma}
{}^{(4)}R^\xi{}_{\delta\beta\alpha}
-K_{\mu\gamma}K_\nu{}^\lambda+K_{\nu\gamma}K_\mu{}^\lambda\right].
$$

Since this holds for every tangential [covector](../../../../../../covector.md), the [Gauss equation](../../../../../../gauss-equation.md) follows:

$$
\boxed{{}^{(3)}R^\lambda{}_{\gamma\nu\mu}
=P^\lambda{}_{\xi}P^\alpha{}_{\mu}P^\beta{}_{\nu}P^\delta{}_{\gamma}
{}^{(4)}R^\xi{}_{\delta\beta\alpha}
-K_{\mu\gamma}K_\nu{}^\lambda+K_{\nu\gamma}K_\mu{}^\lambda.}
$$

The signs use a timelike unit normal and the specified [commutator](../../../../../../commutator.md) convention; reversing a curvature convention without changing the [commutator](../../../../../../commutator.md) would change the comparison.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
