<h1 id="17a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The normalized [spherical harmonics](../../../../../../spherical-harmonic.md) separate the angular variables. The [Radial Schrodinger equation for the hydrogen atom](../../../../../../radial-schrodinger-equation-for-the-hydrogen-atom.md) is

$$
-\frac{\hbar^2}{2m}\left(R''+\frac2rR'-\frac{l(l+1)}{r^2}R\right)
-\frac{e^2}{4\pi\epsilon_0r}R=ER.
$$

Write $R=Ar^le^{-\kappa r}$. Then

$$
\frac{R''+2R'/r-l(l+1)R/r^2}{R}
=\kappa^2-\frac{2\kappa(l+1)}r.
$$

Substitution separates a constant term and a $1/r$ term. The latter vanishes precisely when $\hbar^2\kappa(l+1)/m=e^2/(4\pi\epsilon_0)$. With $\kappa=1/[a(l+1)]$ this determines the [Bohr radius](../../../../../../bohr-radius.md)

$$
\boxed{a=\frac{4\pi\epsilon_0\hbar^2}{me^2}.}
$$

The constant term determines

$$
\boxed{E=-\frac{\hbar^2}{2ma^2(l+1)^2}
=-\frac{e^2}{8\pi\epsilon_0a(l+1)^2},\qquad D=8(l+1)^2.}
$$

These are the [maximal-angular-momentum hydrogen states](../../../../../../maximal-angular-momentum-hydrogen-state.md), with principal quantum number $n=l+1$.

Because the angular integral is one, normalization requires

$$
1=|A|^2\int_0^\infty r^{2l+2}e^{-2\kappa r}\,dr
=|A|^2\frac{(2l+2)!}{(2\kappa)^{2l+3}}.
$$

Therefore

$$
\boxed{|A|^2=\frac{2^{2l+3}}{a^{2l+3}(2l+2)!(l+1)^{2l+3}},
\quad F=2l+3,\ G=2l+2,\ H=2l+3.}
$$

The phase of $A$ remains arbitrary.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [17A](../../17a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
