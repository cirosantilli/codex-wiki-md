<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

After the sudden parameter change, the [functional derivative](../../../../../../functional-derivative.md) is

$$
\frac{\delta F}{\delta\mathbf p}
=a_F\mathbf p-\kappa\nabla^2\mathbf p.
$$

Each Cartesian component of each [Fourier mode](../../../../../../fourier-transform.md) consequently obeys

$$
\dot p_{\mathbf q,i}
=-r(q)p_{\mathbf q,i}+f_{\mathbf q,i},
\qquad
r(q)=\Gamma(a_F+\kappa q^2).
$$

This is an [Ornstein-Uhlenbeck process](../../../../../../ornstein-uhlenbeck-process.md). The integrating-factor method gives

$$
p_{\mathbf q,i}(t)
=p_{\mathbf q,i}(t_1)e^{-r(q)(t-t_1)}
+\int_{t_1}^{t}dt'\,
f_{\mathbf q,i}(t')e^{-r(q)(t-t')}.
$$

Because both coefficients are positive, every mode has positive decay rate.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
