<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [residue theorem](../../../../residue-theorem.md) states that a positively oriented simple closed contour enclosing isolated poles and none on the contour has integral $2\pi i$ times the sum of their [residues](../../../../residue.md), provided the function is holomorphic elsewhere inside. Near a simple zero of $\psi$, $\psi(z)=\psi'(a)(z-a)+O((z-a)^2)$. Hence

$$
\boxed{\operatorname{Res}_{z=a}\frac{\phi(z)}{\psi(z)}=\lim_{z\to a}\frac{(z-a)\phi(z)}{\psi(z)}=\frac{\phi(a)}{\psi'(a)}.}
$$

For $\cot z=\cos z/\sin z$, this gives $\boxed{\operatorname{Res}_{z=k\pi}\cot z=1}$ for every integer $k$.

To evaluate the real integral, integrate $F(z)=\operatorname{Log}z/(z^2+a^2)$ around an upper semicircle, with a small upper semicircular indentation excluding zero. Use the branch real on the positive axis and with argument between zero and $\pi$ in the upper half-plane. The large arc tends to zero as $O(\ln R/R)$ and the small arc as $O(\epsilon|\ln\epsilon|)$. The only enclosed pole is $ia$, whose contribution is

$$
2\pi i\operatorname{Res}_{z=ia}F=\frac\pi a\left(\ln a+\frac{i\pi}{2}\right).
$$

On the negative real axis the upper boundary value is $\operatorname{Log}(-x)=\ln x+i\pi$. The two real segments therefore contribute

$$
2I+i\pi\int_0^\infty\frac{dx}{x^2+a^2}=2I+\frac{i\pi^2}{2a}.
$$

Comparing real parts yields

$$
\boxed{I=\int_0^\infty\frac{\ln x}{x^2+a^2}dx=\frac{\pi\ln a}{2a},\qquad I|_{a=1}=0.}
$$

The integral is absolutely convergent at both zero and infinity, so no principal-value interpretation is needed.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [Paper 2](../../paper-2-split.md)
3. [2004](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
