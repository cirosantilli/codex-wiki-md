<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a compactly supported variation $\phi\mapsto\phi+\varepsilon\eta$, the first variation of the [energy functional](../../../../../energy-functional.md) is

$$
\delta E=\int_{\mathbb R}\{\phi'\eta'+U'(\phi)\eta\}\,dx=\int_{\mathbb R}\{-\phi''+U'(\phi)\}\eta\,dx.
$$

Integration by parts has no endpoint term. Since $\eta$ is arbitrary, the static [Euler-Lagrange field equation](../../../../../euler-lagrange-field-equation.md) is

$$
\boxed{\phi''=U'(\phi).}
$$

Integrating the specified polynomial derivative gives $U(\phi)=\phi^2/2-\phi^4+\phi^6/2+C$. The polynomial factors as a nonnegative square times $\phi^2$; its global minimum is zero when $C=0$. Therefore

$$
\boxed{U(\phi)=\tfrac12\phi^2(1-\phi^2)^2,\qquad \phi_{\rm vac}=-1,0,1.}
$$

These are the three constant [scalar-field vacua](../../../../../scalar-field-vacuum.md). For a localized finite-energy [kink](../../../../../scalar-field-kink.md), the two ends approach vacua and the derivative tends to zero. Multiplying the field equation by $\phi'$ gives the first integral

$$
\tfrac12(\phi')^2-U(\phi)=0.
$$

A nonconstant kink must stay within one interval between neighboring vacua. A proposed direct connection from $-1$ to $1$ would reach $\phi=0$ at some finite point, where the first integral forces $\phi'=0$. Uniqueness for the smooth second-order differential equation then forces the identically zero solution, a contradiction. This is the [intermediate-vacuum obstruction to a kink](../../../../../intermediate-vacuum-obstruction-to-a-kink.md); two elementary kinks can span the outer vacua only in an infinite-separation limit, not as one finite-width static kink.

There are consequently **four oriented elementary sectors: $-1\to0$, $0\to-1$, $0\to1$ and $1\to0$**. If opposite orientations are grouped together, there are two kink families and their antikinks. Spatial reflection reverses orientation, and $\phi\mapsto-\phi$ exchanges the two adjacent intervals; both preserve the energy. All four therefore have the same rest [mass](../../../../../mass.md), even though the central and outer vacua have different fluctuation curvatures.

For the sector $0\to1$, define $W(\phi)=\phi^2/2-\phi^4/4$, so $U=(W')^2/2$ and $W'=\phi(1-\phi^2)$. The [Bogomolny bound](../../../../../bogomolny-bound.md) follows by [completing the square](../../../../../completing-the-square.md):

$$
E=\frac12\int_{\mathbb R}[\phi'-W'(\phi)]^2dx+W(1)-W(0)\ge\frac14.
$$

It is saturated by the [Bogomolny equation](../../../../../bogomolny-equations.md)

$$
\boxed{\phi'=\phi(1-\phi^2),\qquad M_{\rm kink}=\frac14.}
$$

Let $y=\phi^2$ on this positive branch. Then $y'=2y(1-y)$, so $\log[y/(1-y)]=2(x-x_0)$. Thus the explicit [kink in a phi-six model](../../../../../kink-in-a-phi-six-model.md) is

$$
\boxed{\phi_{0\to1}(x)=\frac1{\sqrt{1+e^{-2(x-x_0)}}}.}
$$

It has the required limits and satisfies the first integral. The translated center $x_0$ is arbitrary. All oriented elementary solutions are

$$
\phi_{\sigma,\eta}(x)=\sigma[1+e^{-2\eta(x-x_0)}]^{-1/2},\qquad\sigma,\eta\in\{1,-1\}.
$$

For $\eta=1$ the endpoints are $0\to\sigma$, and for $\eta=-1$ they are $\sigma\to0$. Direct evaluation $\int_0^1\sqrt{2U(\phi)}\,d\phi=\int_0^1\phi(1-\phi^2)d\phi=1/4$ independently gives their common [mass](../../../../../mass.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 52](../../paper-52-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
