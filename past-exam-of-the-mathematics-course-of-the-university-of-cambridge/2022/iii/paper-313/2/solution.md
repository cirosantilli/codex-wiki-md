<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Finite energy requires $|\phi|\to1$ and $D\phi\to0$ on the circle at spatial infinity. Writing $\phi\sim e^{i\chi}$ there gives $A\sim d\chi$. The [vortex number](../../../../../vortex-number.md) is the [winding number](../../../../../winding-number.md)

$$
N=\frac1{2\pi}\oint_{S_\infty^1}d\chi\in\mathbb Z.
$$

By [Stokes theorem](../../../../../stokes-theorem.md), the [magnetic flux](../../../../../magnetic-flux.md) is quantized:

$$
\boxed{\int_{\mathbb R^2}B\,dx^1\wedge dx^2
=\oint_{S_\infty^1}A=2\pi N}.
$$

For the rotationally symmetric [Abelian Higgs vortex](../../../../../nielsen-olesen-vortex.md) ansatz, $A=f(r)d\theta$ and $\phi=h(r)e^{ik\theta}$ give

$$
B=\frac{f'}r,
\qquad
|D\phi|^2=(h')^2+\frac{(k-f)^2h^2}{r^2}.
$$

After the angular integration, the [Abelian Higgs model](../../../../../abelian-higgs-model.md) energy becomes

$$
\mathcal E(f,h)=\pi\int_0^\infty
\left[
\frac{(f')^2}{r}+r(h')^2
+\frac{(k-f)^2h^2}{r}
+\frac r4(1-h^2)^2
\right]dr.
$$

[Completing the square](../../../../../completing-the-square.md) in the two pairs of terms gives

$$
\begin{aligned}
\frac{\mathcal E}{\pi}
={}&\int_0^\infty\left[
r\left(h'-\frac{k-f}{r}h\right)^2
+\frac1r\left(f'-\frac r2(1-h^2)\right)^2
\right]dr\\
&-\left[(k-f)(1-h^2)\right]_{0}^{\infty}.
\end{aligned}
$$

Regularity at the origin and approach to the vacuum at infinity require

$$
\boxed{f(0)=0,\quad h(0)=0,\qquad
f(\infty)=k,\quad h(\infty)=1}.
$$

More precisely, $h(r)=O(r^k)$ and $f(r)=O(r^2)$ near the origin. The boundary term is $k$, so

$$
\boxed{\mathcal E\geq k\pi}.
$$

The bound is saturated exactly when both squares vanish, giving the radial [Bogomolny vortex equations](../../../../../bogomolny-vortex-equation.md)

$$
\boxed{
h'=\frac{k-f}{r}h,
\qquad
f'=\frac r2(1-h^2)}.
$$

The asymptotic value $f(\infty)=k$ also makes the flux $2\pi k$, so the ansatz has vortex number $N=k$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 313](../../paper-313-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
