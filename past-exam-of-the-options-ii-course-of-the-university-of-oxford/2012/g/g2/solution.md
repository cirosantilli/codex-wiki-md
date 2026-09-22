<h1 id="g/g2/solution">Solution</h1>

↑ **Parent:** [G2](../g2.md)

Take a [smooth](../../../../smooth-function.md) variation $u+\varepsilon v$ with $v=0$ on the [boundary](../../../../boundary-of-a-set.md). Differentiating under the [integral](../../../../integral-split.md) gives the [first variation](../../../../first-variation.md)

$$
\delta I[u](v)=\iint_R(F_uv+F_{u_\xi}v_\xi+F_{u_\zeta}v_\zeta)\,d\xi\,d\zeta.
$$

[Integration by parts](../../../../integration-by-parts.md) removes the [derivatives](../../../../derivative.md) of $v$, and the [boundary](../../../../boundary-of-a-set.md) contribution vanishes. The [fundamental lemma of the calculus of variations](../../../../fundamental-lemma-of-the-calculus-of-variations.md) therefore gives

$$
\boxed{F_u-\partial_\xi F_{u_\xi}-\partial_\zeta F_{u_\zeta}=0.}
$$

For a regular [constraint](../../../../constraint-mechanics.md) $J[u]=c$, the [Lagrange multiplier](../../../../lagrange-multiplier.md) rule says that an extremal satisfies $\delta I=\lambda\delta J$ for a constant $\lambda$. Equivalently, apply the preceding Euler–Lagrange equation to $F-\lambda G$. Regularity means that $\delta J$ is not identically zero as a [linear functional](../../../../linear-functional.md) on the admissible variations. For the quadratic [constraint](../../../../constraint-mechanics.md) below this holds at every nonzero admissible $u$; a zero [constraint](../../../../constraint-mechanics.md) leaves only $u=0$.

In [polar coordinates](../../../../polar-coordinates.md) the constrained integrand is

$$
\mathcal L=r u_r^2+\frac1r u_\theta^2-\lambda r u^2.
$$

Its Euler–Lagrange equation is $-2\lambda r u-\partial_r(2ru_r)-\partial_\theta(2u_\theta/r)=0$, or

$$
\boxed{u_{rr}+\frac1r u_r+\frac1{r^2}u_{\theta\theta}+\lambda u=0,\qquad u(a,\theta)=0.}
$$

The [field](../../../../field.md) is single-valued and [periodic](../../../../periodic-function.md) in $\theta$. [Substitution](../../../../substitution-algebra.md) $u=f(r)\cos(n\theta)$ with $n\in\{0,1,2,\ldots\}$ gives

$$
\boxed{f''+\frac1r f'+\left(\lambda-\frac{n^2}{r^2}\right)f=0,\qquad f(a)=0.}
$$

The [centre](../../../../center-geometry.md) is part of the disk, so one must also select the regular radial solution: for $n\geq1$, smoothness gives $f(r)=O(r^n)$ and the regular [derivative](../../../../derivative.md) behaviour; for $n=0$, $f$ is [bounded](../../../../boundedness.md) and $f'(0)=0$. A singular solution at zero does not define an admissible [smooth](../../../../smooth-function.md) [field](../../../../field.md) on the disk.

For fixed $n$, let $c_n=\int_0^{2\pi}\cos^2(n\theta)\,d\theta$, so $c_0=2\pi$ and $c_n=\pi$ for $n\geq1$. The angular [derivative](../../../../derivative.md) term has [integral](../../../../integral-split.md) $n^2c_n$, including zero when $n=0$. Consequently

$$
\widehat I[f]=c_n\int_0^a\left(rf'^2+\frac{n^2}{r}f^2\right)\,dr,\qquad
\widehat J[f]=c_n\int_0^a rf^2\,dr.
$$

The one-dimensional Euler–Lagrange equation for $\widehat I-\lambda\widehat J$ is

$$
-(rf')'+\frac{n^2}{r}f=\lambda rf,
$$

exactly the same radial equation. The common factor $c_n$ cancels.

For two regular solutions with the same $n$ and different multipliers, multiply the equation for $f_1$ by $f_2$, multiply that for $f_2$ by $f_1$, subtract and integrate. The result is

$$
(\lambda_1-\lambda_2)\int_0^a rf_1f_2\,dr
=\left[r(f_1f_2'-f_1'f_2)\right]_0^a=0.
$$

At $a$, both functions vanish; at zero, regularity makes the [boundary](../../../../boundary-of-a-set.md) term tend to zero. Since the multipliers are distinct,

$$
\boxed{\int_0^a rf_1f_2\,dr=0.}
$$

This is weighted Sturm–Liouville [orthogonality](../../../../orthogonal-vectors.md) with weight $r$.

Finally, multiply one radial equation by $f$ and integrate by parts. The same endpoint conditions yield

$$
\int_0^a\left(rf'^2+\frac{n^2}{r}f^2\right)\,dr=\lambda\int_0^a rf^2\,dr.
$$

Multiplication by $c_n$ proves

$$
\boxed{\widehat I[f_i]-\lambda_i\widehat J[f_i]=0.}
$$

For any nonzero admissible solution the [energy](../../../../energy-split.md) on the left before subtraction is positive, so its multiplier is the positive [Rayleigh quotient](../../../../rayleigh-quotient.md) $\lambda=\widehat I/\widehat J$.

## ↑ Ancestors (12)

1. [G2](../g2.md)
2. [G](../../g.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
