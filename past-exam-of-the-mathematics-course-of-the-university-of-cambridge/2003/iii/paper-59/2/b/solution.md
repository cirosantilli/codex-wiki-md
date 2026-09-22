<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $q=r_\Omega^2$ and $h=\varpi$. The $c,e$ [eigenvalues](../../../../../../eigenvalue.md) at the conductive [equilibrium point](../../../../../../equilibrium-point-of-a-dynamical-system.md) are $-h$ and $-(4-h)\sigma$, both negative since $0<h<4$ and $\sigma>0$. The coupled $(a,b,d)$ [Jacobian matrix](../../../../../../jacobian-matrix.md) has characteristic polynomial

$$
P(s)=(s+\sigma)^2(s+1)-\sigma r(s+\sigma)+\sigma^2q(s+1)
=s^3+A_1s^2+A_2s+A_3,
$$

where

$$
A_1=1+2\sigma,\qquad A_2=\sigma^2+2\sigma-\sigma r+\sigma^2q,\qquad A_3=\sigma^2(1+q-r).
$$

A simple zero [eigenvalue](../../../../../../eigenvalue.md) occurs on $\boxed{r_P=1+q}$. The reflection $(a,b,d)\mapsto(-a,-b,-d)$, with $c,e$ fixed, makes its generic [steady-state bifurcation](../../../../../../steady-state-bifurcation.md) a [pitchfork bifurcation](../../../../../../pitchfork-bifurcation-normal-form.md).

For a nonzero imaginary pair, substitute $s=i\omega$ into $P$: the real and imaginary parts require $A_3=A_1A_2$ and $\omega^2=A_2>0$. Hence

$$
\boxed{r_H=2(1+\sigma)+\frac{2\sigma^2}{1+\sigma}q,\qquad
\omega_H^2=\sigma^2\left(\frac{1-\sigma}{1+\sigma}q-1\right).}
$$

With $0<\sigma<1$, this [Hopf bifurcation](../../../../../../hopf-bifurcation.md) curve is present only for $q>q_{TB}=(1+\sigma)/(1-\sigma)$. At its intersection with the [pitchfork bifurcation](../../../../../../pitchfork-bifurcation-normal-form.md) curve,

$$
\boxed{q_{TB}=\frac{1+\sigma}{1-\sigma},\qquad r_{TB}=\frac2{1-\sigma},}
$$

and $P(s)=s^2(s+1+2\sigma)$. The zero [eigenvalue](../../../../../../eigenvalue.md) has geometric multiplicity one: its [eigenvector](../../../../../../eigenvector.md) has $b=a$, $d=a/\sigma$. Thus this is a reflection-symmetric [Bogdanov–Takens bifurcation](../../../../../../bogdanov-takens-bifurcation.md), rather than two independent zero modes.

The [Routh-Hurwitz stability criterion](../../../../../../routh-hurwitz-stability-criterion.md) gives the stable trivial state below $r_P$ for $q<q_{TB}$ and below $r_H$ for $q>q_{TB}$. The rest of the line $r_P$, beyond $q_{TB}$, is a stationary [bifurcation](../../../../../../bifurcation.md) of an already unstable trivial state. Likewise the extension of $r_H$ below $q_{TB}$ is only an algebraic line, since its putative frequency is not real. The middle panel of the [bifurcation diagram](../../../../../../bifurcation-diagram.md) in part 1(b) distinguishes the actual curves from this extension.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
