<h1 id="31c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The substitution $u=e^{-x}$ changes the [beta function](../../../../../../beta-function.md) to

$$
B(s,t)=\int_0^\infty e^{-sx}(1-e^{-x})^{t-1}\,dx.
$$

For fixed $t>0$, its factor near zero expands as

$$
(1-e^{-x})^{t-1}=x^{t-1}\left[1-\frac{t-1}{2}x+O(x^2)\right].
$$

Away from zero the factor is bounded, so the extension from the finite-interval [Watson lemma](../../../../../../watson-s-lemma.md) to this exponentially damped tail is immediate. Therefore

$$
\boxed{B(s,t)=\frac{\Gamma(t)}{s^t}
\left[1-\frac{t(t-1)}{2s}+O(s^{-2})\right]\quad(s\to\infty).}
$$

The change $u\mapsto1-u$ gives $B(s,t)=B(t,s)$, so, with $s>0$ fixed,

$$
\boxed{B(s,t)=\frac{\Gamma(s)}{t^s}
\left[1-\frac{s(s-1)}{2t}+O(t^{-2})\right]\quad(t\to\infty).}
$$

These expansions hold with the other parameter fixed; the first does not claim uniformity when $t$ grows with $s$. The printed gamma-integral hint has inconsistent variable labels: the integration differential is $dx$ and the positive parameter is $y$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [31C](../../31c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
