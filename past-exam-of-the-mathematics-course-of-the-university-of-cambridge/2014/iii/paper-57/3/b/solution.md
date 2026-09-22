<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $\xi=\tanh(z/H)$, so $h=1-\xi^2$ and $d/dz=(1-\xi^2)H^{-1}d/d\xi$. The vertical equation becomes

$$
\frac{1-\xi^2}{H^2}\frac{d}{d\xi}\left[(1-\xi^2)\frac{dF}{d\xi}\right]+k^2(1-\xi^2)F=0.
$$

For $|\xi|<1$, division by the common factor gives the [Legendre differential equation](../../../../../../legendre-differential-equation.md) with eigenvalue $k^2H^2$. Requiring boundedness at both surfaces $\xi=\pm1$ selects

$$
\boxed{F_n(z)=P_n(\tanh(z/H)),\qquad k_n=\frac{\sqrt{n(n+1)}}H,\quad n=0,1,2,\ldots.}
$$

The second independent solution is unbounded at an endpoint. These are the [bounded vertical modes of a sech-squared magnetized disk](../../../../../../bounded-vertical-modes-of-a-sech-squared-magnetized-disk.md). The division by $H$ is outside the square root, as in the original PDF; the converted TeX places it incorrectly. The magnetic perturbation involves $F'_n$, which tends to zero at either surface.

The constant $n=0$ function has $k=0$. The specified magnetic ansatz contains $1/(ik)$ and must not be applied to it. A uniform horizontal velocity with no magnetic perturbation is an [epicyclic motion](../../../../../../epicyclic-motion.md), not a growing magnetic mode; the zero-wavenumber formal degeneracy does not provide growing MRI at arbitrary field strength. Nontrivial magnetically coupled vertical modes have $n\geq1$.

For $A>0$, the [magnetorotational instability](../../../../../../magnetorotational-instability.md) grows when $A<3\Omega^2$. Indeed, the quadratic in $s^2$ then has a negative constant term, and one positive root. For $A\geq3\Omega^2$, the two roots are nonpositive, since their sum is negative, their product nonnegative, and their discriminant is $\Omega^4+16\Omega^2A>0$. The smallest nonzero vertical eigenvalue is $k_1^2=2/H^2$, so all vertical modes are stable if

$$
\frac{2v_A^2}{H^2}\geq3\Omega^2
\quad\Longleftrightarrow\quad
\boxed{\beta=\frac{2\Omega^2H^2}{v_A^2}\leq\frac43.}
$$

The strict inequality requested gives stability, and equality is marginal for $n=1$. A sufficiently strong field increases [magnetic tension](../../../../../../magnetic-tension.md). The unstable MRI needs a sufficiently long vertical wavelength to exchange angular momentum without excessive restoring tension; bounded vertical structure imposes a smallest nonzero effective wavenumber. Beyond the [finite-thickness magnetorotational instability criterion](../../../../../../finite-thickness-magnetorotational-instability-criterion.md), no allowed magnetic mode is long enough to remain unstable.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
