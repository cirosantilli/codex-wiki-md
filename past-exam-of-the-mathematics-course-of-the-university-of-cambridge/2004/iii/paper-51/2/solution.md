<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the [Minkowski metric](../../../../../minkowski-metric.md) convention $\eta=\operatorname{diag}(1,-1,-1,-1)$. On the [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md), the [adjoint covariant derivative](../../../../../adjoint-covariant-derivative.md) is $D_\mu X=\partial_\mu X+[A_\mu,X]$. Set $a_\mu=\delta A_\mu$ and $\chi=\delta\Phi$. Then

$$
\delta F_{\mu\nu}=D_\mu a_\nu-D_\nu a_\mu,\qquad
\delta(D_\mu\Phi)=D_\mu\chi+[a_\mu,\Phi].
$$

The [trace](../../../../../matrix-trace.md) obeys $\operatorname{Tr}(X[Y,Z])=\operatorname{Tr}([Z,X]Y)$, and covariant [integration by parts](../../../../../integration-by-parts.md) has the ordinary boundary term because the [trace](../../../../../matrix-trace.md) of a [commutator](../../../../../commutator.md) is zero. Thus compactly supported variations give

$$
\begin{aligned}
\delta S=\int d^4x\,\operatorname{Tr}\bigl(&F^{\mu\nu}D_\mu a_\nu
-D^\mu\Phi\,D_\mu\chi-D^\mu\Phi[a_\mu,\Phi]+m^2\Phi\chi\bigr)\\
=\int d^4x\,\operatorname{Tr}\bigl(&[-D_\mu F^{\mu\nu}+[D^\nu\Phi,\Phi]]a_\nu
+[D_\mu D^\mu\Phi+m^2\Phi]\chi\bigr).
\end{aligned}
$$

The [trace](../../../../../matrix-trace.md) pairing on $\mathfrak{su}(2)$ is nondegenerate, so the [Euler-Lagrange field equations](../../../../../euler-lagrange-field-equation.md) are

$$
\boxed{D_\mu F^{\mu\nu}=[D^\nu\Phi,\Phi],\qquad D_\mu D^\mu\Phi+m^2\Phi=0.}
$$

In particular the sign of the scalar mass term follows from the plus sign in the supplied [trace](../../../../../matrix-trace.md) [Lagrangian density](../../../../../lagrangian-density.md); it should not be guessed from a different metric convention. This is the [adjoint Yang-Mills-Higgs trace variation](../../../../../adjoint-yang-mills-higgs-trace-variation.md).

For the static [Bogomolny-Prasad-Sommerfield monopole](../../../../../bogomolny-prasad-sommerfield-monopole.md), take the usual purely magnetic extension $\partial_0A_i=\partial_0\Phi=0$ and [temporal gauge](../../../../../temporal-gauge.md) $A_0=0$. At $m=0$, the equations reduce to

$$
D_jF_{ji}=[\Phi,D_i\Phi],\qquad D_iD_i\Phi=0,
$$

with the $\nu=0$ equation identically zero. We now verify both spatial equations from $B_i=D_i\Phi$ without assuming them. The [gauge-theory Bianchi identity](../../../../../gauge-theory-bianchi-identity.md) gives $D_iB_i=0$, hence immediately $D_iD_i\Phi=0$. Also $F_{ji}=\varepsilon_{jik}B_k$, so

$$
\begin{aligned}
D_jF_{ji}&=\varepsilon_{jik}D_jD_k\Phi
=\frac12\varepsilon_{jik}[D_j,D_k]\Phi\\
&=\frac12\varepsilon_{jik}[F_{jk},\Phi]
=-[B_i,\Phi]=[\Phi,D_i\Phi].
\end{aligned}
$$

Here $\varepsilon_{jik}\varepsilon_{jk\ell}=-2\delta_{i\ell}$. This proves that the [Bogomolny equations](../../../../../bogomolny-equations.md) imply all static zero-mass [Yang-Mills equations](../../../../../yang-mills-equations.md) and the scalar equation. The specification of $A_0$ matters: the spatial [Bogomolny equations](../../../../../bogomolny-equations.md) by themselves do not constrain an arbitrary extra electric potential, so the implication is for their standard purely magnetic static extension.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
