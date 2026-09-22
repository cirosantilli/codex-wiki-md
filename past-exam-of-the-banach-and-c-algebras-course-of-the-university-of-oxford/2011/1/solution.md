<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A unital **[Banach star-algebra](../../../banach-star-algebra.md)** is a complex unital [Banach algebra](../../../banach-algebra-split.md) with a continuous conjugate-linear [algebra involution](../../../algebra-involution.md) satisfying

$$
(ab)^*=b^*a^*,\qquad(a^*)^*=a,\qquad1^*=1.
$$

The algebra [norm](../../../norm.md) is complete and submultiplicative, with the unit conventionally normalized to [norm](../../../norm.md) one. Many definitions additionally require the involution to be isometric, $\|a^*\|=\|a\|$; the function algebra here satisfies this stronger convention as well. A [Banach star-algebra](../../../banach-star-algebra.md) does not by definition require the extra [C-star identity](../../../c-star-identity.md) $\|a^*a\|=\|a\|^2$.

Here is the lattice proof of the **[Stone-Weierstrass theorem](../../../stone-weierstrass-theorem.md)** in its complex self-adjoint form. Let $B$ be the uniform [closure](../../../closure-topology.md) of the given unital star-subalgebra in $C(\Omega)$, and let $B_{\mathbb R}$ be its real-valued part. [Closure](../../../closure-topology.md) preserves multiplication and [complex conjugation](../../../complex-conjugation.md), so $B$ is still a unital [star-algebra](../../../star-algebra.md). Real and imaginary parts lie in $B_{\mathbb R}$, and separation by the complex algebra implies separation by its real-valued part.

For $h\in B_{\mathbb R}$, [polynomial](../../../polynomial-split.md) approximation of absolute value on a bounded interval gives $|h|\in B_{\mathbb R}$. For example, this [polynomial](../../../polynomial-split.md) approximation follows from the binomial series for the square root, whose coefficients give [uniform convergence](../../../uniform-convergence.md) on the relevant closed interval. Thus

$$
\max(h,k)=\tfrac12(h+k+|h-k|),\qquad
\min(h,k)=\tfrac12(h+k-|h-k|)
$$

also lie in $B_{\mathbb R}$. It is therefore a lattice of functions.

To see how the lattice gives density, fix a real continuous target $f$ and a tolerance $\epsilon>0$. For any two distinct points $x,y$, separation and constants provide $h_{xy}\in B_{\mathbb R}$ with $h_{xy}(x)=f(x)$ and $h_{xy}(y)=f(y)$, by an affine rescaling of a separating function. For $x=y$, use the constant $f(x)$.

Fix $x$. The sets where $h_{xy}>f-\epsilon$ cover $\Omega$ as $y$ varies. A finite subcover and a pointwise maximum give $g_x\in B_{\mathbb R}$ with $g_x>f-\epsilon$ everywhere and $g_x(x)=f(x)$. The neighborhoods where $g_x<f+\epsilon$ now cover $\Omega$ as $x$ varies. A second finite subcover and a pointwise minimum give $h\in B_{\mathbb R}$ satisfying

$$
f-\epsilon<h<f+\epsilon\quad\text{everywhere on }\Omega.
$$

This is [lattice approximation from two-point approximation](../../../lattice-approximation-from-two-point-approximation.md). Using half the desired tolerance gives strict uniform error below the desired bound. Since $B_{\mathbb R}$ is closed, it contains every real [continuous function](../../../continuous-function.md). Splitting a complex function into real and imaginary parts proves $\boxed{B=C(\Omega)}$.

**The annulus test.** For the closed annulus, the family holomorphic in the interior is **not dense** in the full continuous-function algebra. A uniform limit on the annulus is locally uniform in its interior, so [locally uniform convergence of holomorphic functions](../../../locally-uniform-convergence-of-holomorphic-functions.md) makes that limit holomorphic there. Thus the proposed family is closed in $C(\Omega)$. It is proper because $z\mapsto\overline z$ is continuous but not holomorphic on the annulus interior.

There is also an explicit continuous functional detecting the obstruction. Choose a small closed disk of radius $r$ contained in the annulus interior and let $L(h)$ be the integral of $h(z)\,dz$ around its positively oriented boundary. The [Cauchy integral theorem](../../../cauchy-s-integral-theorem.md) gives $L(h)=0$ for every member of the holomorphic family, while parametrizing the circle gives $L(\overline z)=2\pi i r^2\ne0$. Since $|L(h)|\leq2\pi r\|h\|_\infty$, no [uniform approximation](../../../uniform-approximation-split.md) of $\overline z$ by that family is possible.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2011](../../2011-split.md)
3. [Past exam of the Banach and C\*-algebras course of the University of Oxford](../../split.md)
4. [Banach and C\*-algebras course of the University of Oxford](../../../banach-and-c-algebras-course-of-the-university-of-oxford.md)
5. [Year 4 of the mathematics course of the University of Oxford](../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
