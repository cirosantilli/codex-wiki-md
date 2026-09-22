<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The first derivative of a scalar is a covector, so

$$
\varphi_{;lm}=\partial_m\partial_l\varphi-\Gamma^p{}_{lm}\partial_p\varphi.
$$

Commuting partial derivatives and the [torsion-free connection](../../../../../../torsion-free-connection.md) give **$\varphi_{;lm}=\varphi_{;ml}$**, the [symmetric Hessian of a scalar field](../../../../../../symmetric-hessian-of-a-scalar-field.md). Its next [covariant derivative](../../../../../../covariant-derivative.md) is

$$
\varphi_{;lmn}=\partial_n(\varphi_{;lm})-\Gamma^p{}_{ln}\varphi_{;pm}-\Gamma^p{}_{mn}\varphi_{;lp}.
$$

In particular, [tensor index symmetrization](../../../../../../tensor-index-symmetrization.md) over $l,m$ adds nothing: $\varphi_{;(lm)n}=\varphi_{;lmn}$. This does not make the third index interchangeable with the first two. Applying the lower-index [Ricci identity](../../../../../../curvature-commutator-on-a-covariant-tensor.md) to the covector $\varphi_{;l}$ yields the requested [tensor index antisymmetrization](../../../../../../tensor-index-antisymmetrization.md):

$$
\boxed{\varphi_{;l[mn]}=-\frac12R^p{}_{lmn}\varphi_{;p}.}
$$

Parentheses and brackets include the usual averaging factors. To make the remaining symmetry explicit, let $S_{lmn}=\varphi_{;(lmn)}$. Since the first two derivative indices are already symmetric,

$$
S_{lmn}=\frac13(\varphi_{;lmn}+\varphi_{;lnm}+\varphi_{;mnl}).
$$

The two commutator identities give $\varphi_{;lnm}=\varphi_{;lmn}+R^p{}_{lmn}\varphi_{;p}$ and $\varphi_{;mnl}=\varphi_{;lmn}+R^p{}_{mln}\varphi_{;p}$. Thus the [third covariant derivatives of a scalar](../../../../../../third-covariant-derivatives-of-a-scalar.md) can also be written

$$
\boxed{\varphi_{;(lm)n}=S_{lmn}-\frac13\left(R^p{}_{lmn}+R^p{}_{mln}\right)\varphi_{;p}.}
$$

The right-hand side displays exactly the obstruction to total symmetry. At a point where the scalar gradient vanishes, or where these curvature contractions vanish, the third derivative is totally symmetric.

For the final contraction use $R_{ab}=R^c{}_{acb}$. The arbitrary-valence formula gives

$$
T^{ik}{}_{;ik}-T^{ik}{}_{;ki}
=R^i{}_{pik}T^{pk}+R^k{}_{pik}T^{ip}
=R_{pk}T^{pk}-R_{pi}T^{ip}
=R_{pk}(T^{pk}-T^{kp}).
$$

The [Ricci tensor](../../../../../../ricci-tensor.md) of the [Levi-Civita connection](../../../../../../levi-civita-connection.md) is symmetric, whereas the last factor is antisymmetric. Their contraction is zero, proving

$$
\boxed{T^{ik}{}_{;ik}=T^{ik}{}_{;ki}.}
$$

No symmetry of $T^{ik}$ was assumed. This [double divergence of a contravariant tensor](../../../../../../double-divergence-of-a-contravariant-tensor.md) identity uses the metric-compatible connection of [general relativity](../../../../../../general-relativity-split.md): zero torsion alone for an arbitrary affine connection does not guarantee a symmetric [Ricci tensor](../../../../../../ricci-tensor.md) and would not suffice for this final step.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
