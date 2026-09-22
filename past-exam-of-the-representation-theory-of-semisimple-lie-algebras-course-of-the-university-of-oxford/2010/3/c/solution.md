<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the intended finite-dimensional [irreducible](../../../../irreducible-representation.md) [highest weight](../../../../highest-weight-of-a-representation.md) [module](../../../../module-mathematics.md) $A^\phi$, with dominant integral [highest weight](../../../../highest-weight-of-a-representation.md) $\phi$. Its [highest weight](../../../../highest-weight-of-a-representation.md) multiplicity is one. An arbitrary [direct sum](../../../../direct-sum.md) having that same largest [representation weight](../../../../weight-of-a-representation.md) would not in general satisfy this formula. Set $f=\pi_{A^\phi}$ and use the corrected denominator $D$ of part (a).

Restriction to each [simple root](../../../../simple-root.md) $\mathfrak{sl}_2$ decomposes into symmetric finite [representation weight](../../../../weight-of-a-representation.md) strings, so $f$ is Weyl-invariant. Consequently $Df$ is Weyl-antisymmetric. We prove that no lower Weyl alternants occur, rather than assuming the desired character formula.

First establish the denominator identity itself. The finite sum $D$ has support in $\rho-Q_+$ and coefficient one at $\rho$. Antisymmetry kills all singular [representation weight](../../../../weight-of-a-representation.md) coefficients, since a [reflection](../../../../reflection-mathematics.md) fixing the [representation weight](../../../../weight-of-a-representation.md) reverses their sign. Every remaining Weyl orbit has a unique regular dominant representative $\eta$. If it occurs in $D$, then $\eta\le\rho$. Since $\eta$ is integral and regular dominant, $\eta-\rho$ is dominant integral; it also belongs to $-Q_+$. A dominant vector $v=-\sum n_i\alpha_i$ satisfies $(v,v)=-\sum n_i(v,\alpha_i)\le0$, so it must be zero. Thus the only possible orbit is $W\rho$. The leading coefficient gives

$$
D=\sum_{w\in W}(\det w)e^{w\rho}.
$$

For the formal [Laplacian](../../../../laplacian.md) $\mathscr D(e^\lambda)=\|\lambda\|^2e^\lambda$, this implies $\mathscr D D=\|\rho\|^2D$.

Now choose [root](../../../../root-of-a-root-system.md) vectors dual under an invariant form, so $[E_\alpha,E_{-\alpha}]=H_\alpha$ with $H_\alpha$ corresponding to the vector $\alpha$, and take the quadratic Casimir

$$
C=\sum_iH_i^2+\sum_{\alpha>0}(E_\alpha E_{-\alpha}+E_{-\alpha}E_\alpha)
$$

for an orthonormal Cartan [basis](../../../../basis.md). On a highest vector its scalar is $c_\phi=\|\phi+\rho\|^2-\|\rho\|^2$, hence it has this scalar throughout the cyclic [highest weight](../../../../highest-weight-of-a-representation.md) [module](../../../../module-mathematics.md).

Here is the computation of the weighted [trace](../../../../matrix-trace.md) of its radial identity. For a [positive root](../../../../positive-root.md), let $X$ be the formal weighted [trace](../../../../matrix-trace.md) of $E_{-\alpha}E_\alpha$ and $Y$ that of $E_\alpha E_{-\alpha}$. Cyclicity of [trace](../../../../matrix-trace.md) and [representation weight](../../../../weight-of-a-representation.md) shifting give $Y=e^\alpha X$, while their difference is the weighted [trace](../../../../matrix-trace.md) of $H_\alpha$, namely $(\alpha,\nabla f)$. Thus

$$
X+Y=\frac{1+e^{-\alpha}}{1-e^{-\alpha}}(\alpha,\nabla f).
$$

Taking the [trace](../../../../matrix-trace.md) of $C$ yields

$$
c_\phi f=\mathscr D f+\sum_{\alpha>0}\frac{1+e^{-\alpha}}{1-e^{-\alpha}}(\alpha,\nabla f).
$$

The product expression for $D$ gives

$$
\nabla\log D=\rho+\sum_{\alpha>0}\frac{e^{-\alpha}}{1-e^{-\alpha}}\alpha.
$$

Using $2\rho=\sum_{\alpha>0}\alpha$ and the [product rule](../../../../product-rule.md) for the formal [Laplacian](../../../../laplacian.md) therefore gives

$$
\mathscr D(Df)=c_\phi Df+f\mathscr DD
=\|\phi+\rho\|^2Df.
$$

Hence every [representation weight](../../../../weight-of-a-representation.md) in the support of $Df$ has [norm](../../../../norm.md) $\|\phi+\rho\|$. Its support is also contained in $\phi+\rho-Q_+$, and it is antisymmetric. Any occurring regular [dominant weight](../../../../dominant-weight.md) $\eta$ thus satisfies $\eta\le\phi+\rho$. If the inequality were strict, then

$$
\|\phi+\rho\|^2-\|\eta\|^2
=(\phi+\rho-\eta,\phi+\rho+\eta)>0,
$$

because the first factor is a nonzero nonnegative sum of simple roots and the second is strictly dominant. This contradicts the equal-[norm](../../../../norm.md) condition. Only the orbit $W(\phi+\rho)$ remains. Its leading coefficient is one, proving

$$
\boxed{D*\pi_{A^\phi}=\sum_{w\in W}(\det w)\delta_{w(\phi+\rho)}.}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the representation theory of semisimple Lie algebras course of the University of Oxford](../../../split.md)
5. [Representation theory of semisimple Lie algebras course of the University of Oxford](../../../../representation-theory-of-semisimple-lie-algebras-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
