<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [symplectic blowup](../../../../../symplectic-blowup.md) replaces a small [symplectic ball](../../../../../symplectic-ball.md) around the point by an [exceptional divisor](../../../../../exceptional-divisor.md) $\mathbb{CP}^{n-1}$, for $\dim_{\mathbb R}X=2n$. One can construct its form by [symplectic reduction](../../../../../symplectic-reduction.md). In a [Darboux chart](../../../../../darboux-chart.md), consider $\mathbb C^n\times\mathbb C$ with the [circle action](../../../../../circle-action.md)

$$
e^{it}\cdot(z,w)=(e^{it}z,e^{-it}w),
\qquad \mu(z,w)=\frac{|z|^2-|w|^2}{2}.
$$

On $\mu^{-1}(R^2/2)$ the action is free because $z\ne0$. Its quotient therefore carries a smooth [symplectic form](../../../../../symplectic-form.md). Where $w\ne0$, choose the representative with $w$ positive real; the reduced form is the original form on $|z|>R$. Where $w=0$, the quotient is the [Hopf fibration](../../../../../hopf-fibration.md) quotient of $|z|=R$, namely $\mathbb{CP}^{n-1}$. The local quotient is the tautological complex line bundle near its zero section, hence the local blowup. Glue this model to the exterior of the ball to obtain a [symplectic form](../../../../../symplectic-form.md) on the blowup.

The area of a projective line in the exceptional divisor is $\varepsilon=\pi R^2$. For a closed $X$, changing this size changes the [symplectic volume](../../../../../symplectic-volume.md):

$$
\operatorname{Vol}(\widetilde X,\widetilde\omega)
=\operatorname{Vol}(X,\omega)-\frac{\varepsilon^n}{n!}.
$$

Consequently **the blowup is not determined up to symplectomorphism without a size choice**. The underlying smooth blowup is fixed, but the symplectic construction has a parameter, as in [symplectic blowup size changes volume](../../../../../symplectic-blowup-size-changes-volume.md).

For the blowdown map $\pi$ and exceptional divisor $E$, the [First Chern class](../../../../../first-chern-class.md) is

$$
\boxed{c_1(T\widetilde X)=\pi^*c_1(TX)-(n-1)\operatorname{PD}[E]}.
$$

In real dimension four this becomes $\pi^*c_1(TX)-\operatorname{PD}[E]$, the [first Chern class formula for a symplectic blowup](../../../../../first-chern-class-formula-for-a-symplectic-blowup.md).

The tangent bundle of the standard four-[torus](../../../../../torus.md) is a trivial complex rank-two bundle, so its [symplectic canonical class](../../../../../symplectic-canonical-class.md) is zero. For a generic fiber $F$ of a symplectic [Lefschetz pencil](../../../../../lefschetz-pencil.md), the [symplectic adjunction formula](../../../../../symplectic-adjunction-formula.md) gives $2g-2=F^2$. Two generic fibers intersect precisely at the base points, each with local [intersection number](../../../../../intersection-number-of-a-cartier-divisor-with-a-curve.md) one in the pencil model $[z_1:z_2]$. Hence

$$
\boxed{\#\{\text{base points}\}=F^2=2g-2}.
$$

This is [base-point count for a Lefschetz pencil on a symplectic four-torus](../../../../../base-point-count-for-a-lefschetz-pencil-on-a-symplectic-four-torus.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
