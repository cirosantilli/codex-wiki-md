<h1 id="33b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A $j=0$ state exists only when $j_1=j_2=:j$. Since its total magnetic quantum number is zero, every uncoupled basis term must have $m_1+m_2=0$, so

$$
|0,0\rangle=\sum_{m=-j}^j\alpha_m
|j,m\rangle_1|j,-m\rangle_2.
$$

Apply the total raising operator $J_+=J_{1+}+J_{2+}$. The coefficient of  
$|j,m+1\rangle_1|j,-m\rangle_2$ is

$$
\sqrt{(j-m)(j+m+1)}\,(\alpha_m+\alpha_{m+1}).
$$

The [angular momentum singlet state](../../../../../../singlet-state.md) is annihilated by $J_+$, hence

$$
\alpha_{m+1}=-\alpha_m,
\qquad -j\leq m<j.
$$

All coefficients consequently have the same modulus and alternating signs. Normalization fixes that modulus to $(2j+1)^{-1/2}$, and an arbitrary overall phase may be chosen so that

$$
\boxed{
\alpha_m=\frac{(-1)^{j-m}}{\sqrt{2j+1}}
}.
$$

Thus

$$
\boxed{|0,0\rangle=\frac1{\sqrt{2j+1}}
\sum_{m=-j}^j(-1)^{j-m}|j,m\rangle_1|j,-m\rangle_2.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [33B](../../33b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
