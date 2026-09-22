<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $(x^i)$ and $(y^a)$ be overlapping [local coordinates](../../../../../local-coordinate.md) at $p$. A [tangent vector](../../../../../tangent-vector.md) $v=v_x^i\partial_{x^i}$ has components obeying the [chain rule](../../../../../chain-rule.md)

$$
\boxed{v_y^a=\frac{\partial y^a}{\partial x^i}(p)v_x^i.}
$$

The [Jacobian matrix](../../../../../jacobian-matrix.md) is evaluated at the same point, and is invertible. For a smooth curve $a$ with $a(0)=p$, define $\dot a_x^i(0)=\frac{d}{dt}x^i(a(t))|_{t=0}$. Applying the [chain rule](../../../../../chain-rule.md) to $y(a(t))=y(x(a(t)))$ gives exactly this transformation law. Thus these components determine a well-defined [velocity vector](../../../../../velocity-vector.md) $\dot a(0)\in T_pM$, independent of the chart. Equivalently it is the derivation $f\mapsto\frac{d}{dt}f(a(t))|_0$ on smooth functions. The two curve symbols used in the printed first paragraph refer to this same curve.

For real scalars $\lambda,\mu$, consider

$$
c(t)=\exp(\lambda tB_1)\exp(\mu tB_2).
$$

For sufficiently small positive and negative $t$, both factors belong to $G$, so $c$ is a curve in $G$ with $c(0)=I$. The standard [matrix exponential](../../../../../matrix-exponential.md) properties used here are $\exp(0)=I$, $\frac{d}{dt}\exp(tB)|_0=B$, and $\exp(-tB)=\exp(tB)^{-1}$. The product rule gives $c'(0)=\lambda B_1+\mu B_2$. **Every such linear combination is therefore a velocity at the identity.**

More generally, the inclusion $j:G\hookrightarrow GL(n,\mathbb R)$ is an embedding, so its tangent map at $I$ is injective and linear. The [general linear group](../../../../../general-linear-group.md) is open in the vector space of all matrices; its tangent space at $I$ is consequently $M_n(\mathbb R)$. We identify

$$
\boxed{\mathfrak g=dj_I(T_IG)\subseteq M_n(\mathbb R).}
$$

Every tangent vector is the velocity of a curve in a manifold chart, so this subspace is precisely the set of the corresponding matrix velocities. The product construction is consistent with its vector-space operations.

Now use the stated logarithm-chart assumption. Near zero and $I$, the [matrix exponential](../../../../../matrix-exponential.md) and [matrix logarithm](../../../../../matrix-logarithm.md) are inverse smooth maps, with $d\exp_0=d\log_I=\mathrm{id}$. Hence for any $B\in\mathfrak g$, $\exp(tB)$ belongs to $G$ for small $t$: $tB$ lies in the neighborhood which is the image of the logarithm. For $B_1,B_2\in\mathfrak g$, form the group commutator

$$
C(t)=e^{tB_1}e^{tB_2}e^{-tB_1}e^{-tB_2}\in G.
$$

Multiplying the exponential expansions $e^{tB}=I+tB+\tfrac12t^2B^2+O(t^3)$ gives

$$
C(t)=I+t^2(B_1B_2-B_2B_1)+O(t^3).
$$

The convergent local series $\log(I+Z)=Z-\tfrac12Z^2+\cdots$ therefore gives $\log C(t)=t^2[B_1,B_2]+O(t^3)$. For small nonzero $t$, the matrix $t^{-2}\log C(t)$ belongs to the linear subspace $\mathfrak g$. A finite-dimensional linear subspace is closed, so taking its limit proves

$$
\boxed{[B_1,B_2]=B_1B_2-B_2B_1\in\mathfrak g.}
$$

This is the [matrix commutator from a logarithm chart](../../../../../matrix-commutator-from-a-logarithm-chart.md) argument. It identifies $\mathfrak g$ as the [Lie algebra of a matrix Lie group](../../../../../lie-algebra-of-a-matrix-lie-group.md), with the matrix [commutator](../../../../../commutator.md) as its [Lie bracket](../../../../../lie-bracket.md). In particular, no potentially nonsmooth square-root change of parameter is needed to turn the second-order commutator into a velocity.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
