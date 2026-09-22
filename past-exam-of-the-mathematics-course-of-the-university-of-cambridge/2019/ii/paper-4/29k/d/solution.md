<h1 id="29k/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Given the present state $(S_t^1,M_t)=(x,m)$, take an independent fresh copy of the stock path and denote its initial value, terminal value after $T-t$ steps, and running maximum by $(y,z,w)=(S_0^1,S_{T-t}^1,M_{T-t})$. Scaling the fresh path to start at $x$ makes its terminal value $xz/y$ and its future running maximum $xw/y$. Including the maximum already attained gives

$$
M_T=\max\left\{m,\frac{xw}{y}\right\}.
$$

Hence define

$$
\boxed{g(x,m,y,z,w)=h\left(\frac{xz}{y},
\max\left\{m,\frac{xw}{y}\right\}\right).}
$$

Independent increments then give the [Running-maximum state reduction in the Cox--Ross--Rubinstein model](../../../../../../running-maximum-state-reduction-in-the-cox-ross-rubinstein-model.md)

$$
\boxed{V_t(\omega)=v_t(S_t^1(\omega),M_t(\omega)),}
$$

with

$$
\boxed{v_t(x,m)=\mathbb E_Q[g(x,m,S_0^1,S_{T-t}^1,M_{T-t})].}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [29K](../../29k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
