<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Interpret the malformed printed domain inequality as the first quadrant $x>0,y>0$, as indicated by the two axis boundary conditions. There is also a genuine missing hypothesis: decay of the boundary data does not require the [harmonic function](../../../../../harmonic-function.md) itself to be bounded. For zero data, both $q=0$ and $q=xy$ satisfy the [Laplace equation](../../../../../laplace-equation.md) and both edge values, but the [Wirtinger derivative](../../../../../wirtinger-derivatives.md) of the latter is

$$
q_z=\tfrac12(q_x-iq_y)=\tfrac12(y-ix)=-\tfrac i2z\ne0.
$$

Thus **the data do not determine an arbitrary solution's derivative without a growth restriction**. We derive the [integral representation](../../../../../integral-representation.md) for the bounded solution, which is also the standard decaying solution when the continuous edge data decay. Any other admissible unbounded solution can differ by a zero-boundary [harmonic function](../../../../../harmonic-function.md).

The [conformal map](../../../../../conformal-map.md) $w=z^2$ sends the quadrant bijectively to the [complex upper half-plane](../../../../../upper-half-plane-complex-analysis.md): the positive real axis maps to $s>0$, and the positive imaginary axis maps to $s<0$. Define its real-axis boundary function by

$$
f(s)=\begin{cases}g_2(\sqrt s),&s>0,\\g_1(\sqrt{-s}),&s<0,\end{cases}
\qquad f(0)=g_1(0)=g_2(0).
$$

The compatibility at the corner makes $f$ continuous there. The [Dirichlet Poisson integral in a quadrant](../../../../../dirichlet-poisson-integral-in-a-quadrant.md) follows from the upper-half-plane [Poisson kernel](../../../../../poisson-kernel-for-the-upper-half-plane.md):

$$
q(x,y)=\frac1\pi\int_{\mathbb R}
\frac{\operatorname{Im}(z^2)f(s)}{|s-z^2|^2}\,ds.
$$

It is bounded by the supremum of the bounded edge data, and the kernel's [approximate identity](../../../../../approximate-identity.md) property supplies both [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md). More explicitly, for $z^2=a+ic$, where $a=x^2-y^2$ and $c=2xy>0$, this integral is

$$
q(x,y)=\frac{2c}{\pi}\int_0^\infty r\left[
\frac{g_2(r)}{(r^2-a)^2+c^2}
+\frac{g_1(r)}{(r^2+a)^2+c^2}\right]dr.
$$

It displays directly which part of the real-line boundary corresponds to each original axis.

To obtain its derivative, first take real data and use the [Schwarz integral formula](../../../../../schwarz-integral-formula.md). A [holomorphic function](../../../../../holomorphic-function.md) whose [real part](../../../../../real-part.md) is the Poisson solution in the $w$-plane is

$$
F(w)=\frac1{\pi i}\int_{\mathbb R}f(s)
\left[\frac1{s-w}-\frac{s}{1+s^2}\right]ds.
$$

The regularizing subtraction is independent of $w$ and affects only the imaginary normalization; it permits bounded data without an artificial integrability assumption. Then $q=\operatorname{Re}F(z^2)$. By the [chain rule](../../../../../chain-rule.md) and the [Wirtinger derivative](../../../../../wirtinger-derivatives.md),

$$
q_z=zF'(z^2)=\frac z{\pi i}\int_{\mathbb R}\frac{f(s)}{(s-z^2)^2}\,ds.
$$

The factor is $z$, not $2z$: taking the [real part](../../../../../real-part.md) contributes the factor $1/2$ in the complex derivative. [Differentiation under the integral sign](../../../../../differentiation-under-the-integral-sign.md) is justified uniformly on compact interior subsets because the denominator stays away from the real boundary and decays quadratically at infinity. Splitting the real integral at zero and substituting $s=r^2$ or $s=-r^2$ gives the [holomorphic derivative of a quadrant Dirichlet solution](../../../../../holomorphic-derivative-of-a-quadrant-dirichlet-solution.md):

$$
\boxed{q_z(z)=\frac{2z}{\pi i}\int_0^\infty r\left[
\frac{g_2(r)}{(r^2-z^2)^2}
+\frac{g_1(r)}{(r^2+z^2)^2}\right]dr,\qquad x,y>0.}
$$

This converges for bounded data, and in particular for the stated sufficiently decaying data. No interior pole is encountered since $\operatorname{Im}(z^2)=2xy>0$. For complex-valued data the same formula holds by applying the real-data construction separately to their real and imaginary parts and using linearity.

An equivalent form, often convenient when the data's derivatives decay, comes from [integration by parts](../../../../../integration-by-parts.md). Since

$$
\frac{2r}{(r^2-z^2)^2}=-\frac d{dr}\frac1{r^2-z^2},\qquad
\frac{2r}{(r^2+z^2)^2}=-\frac d{dr}\frac1{r^2+z^2},
$$

the two endpoint terms are $-g_2(0)/z^2$ and $+g_1(0)/z^2$. They cancel by the specified compatibility, leaving

$$
\boxed{q_z(z)=\frac z{\pi i}\left[
\int_0^\infty\frac{g_2'(r)}{r^2-z^2}\,dr
+\int_0^\infty\frac{g_1'(r)}{r^2+z^2}\,dr\right].}
$$

This is the [harmonic quadrant solution from tangential boundary derivatives](../../../../../harmonic-quadrant-solution-from-tangential-boundary-derivatives.md) applied to the actual derivatives $g_1',g_2'$; the supplied $g_1,g_2$ in this question are boundary values, not derivatives. Omitting those primes would solve a different boundary problem.

For completeness, [bounded Dirichlet uniqueness in a quadrant](../../../../../bounded-dirichlet-uniqueness-in-a-quadrant.md) selects the solution just constructed. The difference of two bounded solutions is zero on both axes. [Odd reflection](../../../../../odd-reflection.md) across each axis gives a bounded harmonic extension to the punctured plane; the [removable singularity for a bounded harmonic function](../../../../../removable-singularity-for-a-bounded-harmonic-function.md) fills the corner. The [harmonic Liouville theorem](../../../../../harmonic-liouville-theorem.md) makes the extension constant, and oddness makes it zero. Decaying data give a decaying Poisson extension: split the real-axis integral into a fixed compact interval and a tail with arbitrarily small data; the compact contribution tends to zero as $|z^2|\to\infty$, while the tail is bounded by that small supremum.

As literally printed without boundedness or a growth condition, the most one can assert is

$$
\boxed{q_z=(q_{\rm bounded})_z+v_z,\qquad
\Delta v=0,\quad v|_{x=0}=v|_{y=0}=0.}
$$

The [zero-boundary harmonic growth in a quadrant](../../../../../zero-boundary-harmonic-growth-in-a-quadrant.md) includes $v=cxy$ and more generally $v=\operatorname{Im}(z^{2m})$. This is an actual nonuniqueness of the printed problem, not a defect in the integral for the normalized bounded solution.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 328](../../paper-328-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
