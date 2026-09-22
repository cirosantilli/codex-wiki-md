<h1 id="25i/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Again set $h=\sqrt G$ and fix $\theta$. For $0<\alpha<C^{-1/2}$ define

$$
f(r)=h(r,\theta)-\alpha\sin(\sqrt C\,r).
$$

Since $h''=-Kh$ and $K\leq C$,

$$
f''+Cf=(C-K)h\geq0,
\qquad f(0)=0,
\qquad f'(0)=1-\alpha\sqrt C>0.
$$

For $0<r<\pi/\sqrt C$, differentiation gives

$$
\frac d{dr}
\left(f'\sin(\sqrt C r)-\sqrt C f\cos(\sqrt C r)\right)
=(f''+Cf)\sin(\sqrt C r)\geq0.
$$

The expression in parentheses vanishes at zero, and hence

$$
\left(\frac f{\sin(\sqrt C r)}\right)'\geq0.
$$

Its limit at zero is $(1-\alpha\sqrt C)/\sqrt C>0$, so $f>0$. Letting $\alpha\uparrow C^{-1/2}$ yields the [one-dimensional Rauch comparison inequality](../../../../../../one-dimensional-rauch-comparison-inequality.md)

$$
h(r,\theta)\geq\frac{\sin(\sqrt C r)}{\sqrt C}
\qquad(0\leq r<\pi/\sqrt C).
$$

It follows that

$$
\operatorname{Area}B(p,\varepsilon)
\geq\frac{2\pi}{C}\bigl(1-\cos(\sqrt C\,\varepsilon)\bigr).
$$

Now

$$
\frac{2(1-\cos x)}{x^2}\longrightarrow1
$$

as $x\to0$. Given $0<\gamma<1$, choose $x_0\in(0,\pi)$ such that $2(1-\cos x)/x^2\geq\gamma$ for $0<x\leq x_0$, and set $\varepsilon_0=x_0/\sqrt C$. Then every geodesic polar coordinate ball of radius $\varepsilon\leq\varepsilon_0$ satisfies

$$
\boxed{\operatorname{Area}B(p,\varepsilon)\geq\gamma\pi\varepsilon^2.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [25I](../../25i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
