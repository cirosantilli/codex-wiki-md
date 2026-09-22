<h1 id="2/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Define the [pointwise representation of one-forms by vector-field functionals](../../../../../../pointwise-representation-of-one-forms-by-vector-field-functionals.md) by

$$
\boxed{\theta(\omega)(X)=\omega(X).}
$$

It is $\mathbb R$-linear, its value is a smooth function, and $X_p=0$ implies $\theta(\omega)(X)(p)=0$. Moreover

$$
\theta(g\omega)=g\,\theta(\omega),
$$

so it is a map of $C^\infty(M)$-modules. This is the properly typed scalar-multiplication property: the same symbol for a form and its associated functional is understood through $\theta$.

To construct its inverse, let $\alpha\in W$ and $v\in T_pM$. Choose a global smooth [vector field](../../../../../../vector-field.md) $X$ with $X_p=v$; a local coordinate field multiplied by a [smooth bump function](../../../../../../smooth-bump-function.md) supplies such an extension. Set

$$
\omega_p(v)=\alpha(X)(p).
$$

This is well-defined: if $X_p=Y_p$, then $X-Y$ vanishes at $p$, so $\alpha(X-Y)(p)=0$. Real linearity of $\alpha$ makes $\omega_p$ a [covector](../../../../../../covector.md). In fact the pointwise vanishing assumption also forces

$$
\alpha(fX)(p)=f(p)\alpha(X)(p),
$$

because $(f-f(p))X$ vanishes at $p$. Thus $\alpha(fX)=f\alpha(X)$ for every smooth $f$, even though only real linearity was initially imposed.

It remains to prove smoothness, rather than assume continuity of an abstract linear map. Near a fixed point, choose global fields $E_1,\ldots,E_n$ equal to the coordinate basis on a smaller neighborhood, using a bump function equal to one there. On that neighborhood,

$$
\omega=\sum_i\alpha(E_i)\,dx^i.
$$

All coefficients are smooth by the definition of $W$, so $\omega$ is a smooth [differential one-form](../../../../../../one-form.md). The construction holds near every point, hence gives $\omega\in\Omega^1(M)$ with $\alpha(X)=\omega(X)$ globally.

Every tangent vector can be realized by a global field, so $\theta(\omega)=0$ forces $\omega=0$. The inverse just constructed gives surjectivity. **The evaluation map is a natural $C^\infty(M)$-module isomorphism $\Omega^1(M)\cong W$.** No auxiliary metric or connection was chosen.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [2](../../2.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
