<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Choose a nonnegative [mollifier](../../../../../mollifier.md) $\rho\in C_c^\infty(\mathbb R^3)$ with $\int\rho=1$, and put $\rho_\varepsilon(x)=\varepsilon^{-3}\rho(x/\varepsilon)$. [Sobolev approximation by mollifiers](../../../../../sobolev-approximation-by-mollifiers.md) in the [Sobolev space](../../../../../sobolev-space-split.md) under consideration states

$$
\boxed{u_\varepsilon:=\rho_\varepsilon*u\in C^\infty(\mathbb R^3)\cap W^{1,6}(\mathbb R^3),\qquad
\|u_\varepsilon-u\|_{W^{1,6}}\longrightarrow0\quad(\varepsilon\downarrow0).}
$$

In particular, it gives [density of smooth functions in a Sobolev space](../../../../../density-of-smooth-functions-in-a-sobolev-space.md). We prove convergence of both the function and all its first [weak derivatives](../../../../../weak-derivative.md).

The usual smoothing properties of [convolution](../../../../../convolution.md) give $u_\varepsilon\in C^\infty$. For a [test function](../../../../../test-function.md) $\phi\in C_c^\infty(\mathbb R^3)$ and $i\in\{1,2,3\}$, [Fubini's theorem](../../../../../fubini-s-theorem.md) and the definition of a [weak derivative](../../../../../weak-derivative.md) give

$$
\begin{aligned}
\int u_\varepsilon(x)\partial_i\phi(x)\,dx
&=\int\rho_\varepsilon(z)\int u(y)\partial_i\phi(y+z)\,dy\,dz\\
&=-\int\rho_\varepsilon(z)\int\partial_i u(y)\phi(y+z)\,dy\,dz\\
&=-\int(\rho_\varepsilon*\partial_i u)(x)\phi(x)\,dx.
\end{aligned}
$$

The [integrals](../../../../../integral-split.md) are absolutely convergent: the [compact supports](../../../../../compact-support.md) of $\rho_\varepsilon$ and $\phi$ restrict $y$ to a [compact set](../../../../../compact-space.md), on which $u$ and $\partial_i u$ are integrable by [Holder inequality](../../../../../holder-inequality.md). Consequently

$$
\partial_i u_\varepsilon=\rho_\varepsilon*\partial_i u.
$$

The [approximate identity](../../../../../approximate-identity.md) theorem in the [Lp space](../../../../../lp-space.md) $L^6$ applies separately to $u$ and $\partial_i u$. Thus

$$
\|u_\varepsilon-u\|_6\to0,\qquad
\|\partial_i u_\varepsilon-\partial_i u\|_6\to0\quad(i=1,2,3).
$$

Each [convolution](../../../../../convolution.md) belongs to $L^6$ by [Young's convolution inequality](../../../../../young-s-convolution-inequality.md). With the componentwise [Sobolev norm](../../../../../sobolev-norm.md), the sixth power of the required difference is the sum of these four sixth powers, proving the boxed claim. Any equivalent [Sobolev norm](../../../../../sobolev-norm.md) gives the same convergence.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the functional analytic methods for partial differential equations course of the University of Oxford](../../../../split.md)
6. [Functional analytic methods for partial differential equations course of the University of Oxford](../../../../../functional-analytic-methods-for-partial-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
