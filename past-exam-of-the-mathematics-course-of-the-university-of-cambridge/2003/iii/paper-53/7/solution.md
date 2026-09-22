<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Use the [supertranslation-invariant superspace coframe](../../../../../supertranslation-invariant-superspace-coframe.md)

$$
\boxed{\Pi^m=dX^m+i\bar\theta\gamma^m d\theta,
\qquad\Psi^\alpha=d\theta^\alpha.}
$$

It is a basis because the change from $(dX,d\theta)$ is triangular with identity diagonal blocks. Under a rigid [supertranslation](../../../../../supertranslation.md), $\delta\theta=\epsilon$, $\delta X^m=-i\bar\epsilon\gamma^m\theta$ and $d\epsilon=0$. Therefore $\delta\Pi^m=-i\bar\epsilon\gamma^m d\theta+i\bar\epsilon\gamma^m d\theta=0$, and $\delta d\theta=0$.

Writing wedge products explicitly, the three-form is

$$
H_3=\Pi^m\wedge d\bar\theta\gamma_m d\theta.
$$

Both factors are [supertranslation](../../../../../supertranslation.md) invariant. Under a [Lorentz transformation](../../../../../lorentz-transformation.md), $\Pi^m$ and the bilinear in $d\theta$ transform as vectors, so their contraction is invariant. Thus $H_3$ is invariant under the [Super-Poincaré group](../../../../../super-poincare-group.md).

The [Maurer-Cartan equation](../../../../../maurer-cartan-equation.md) is $d\Pi^m=i\,d\bar\theta\gamma^m d\theta$. Since the other factor is closed,

$$
dH_3=i(d\bar\theta\gamma^m d\theta)
\wedge(d\bar\theta\gamma_m d\theta).
$$

The required four-dimensional [Fierz rearrangement](../../../../../fierz-identity.md) identity, which may be stated without proof, is

$$
(C\gamma^m)_{(\alpha\beta}(C\gamma_m)_{\gamma\delta)}=0.
$$

Differentials of odd [Grassmann variables](../../../../../grassmann-variable.md) commute in the graded exterior algebra. Thus the coefficient of the product of four $d\theta$ factors is the fully symmetric spinor-index part appearing in this identity. It vanishes, proving

$$
\boxed{dH_3=0.}
$$

This is the [closed three-form on four-dimensional superspace](../../../../../closed-three-form-on-four-dimensional-superspace.md); it should not be confused with the different closed four-form used for a membrane coupling in Question 10.

## ↑ Ancestors (11)

1. [7](../7.md)
2. [Section A](../section-a.md)
3. [Paper 53](../../paper-53-split.md)
4. [Iii](../../split.md)
5. [2003](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
