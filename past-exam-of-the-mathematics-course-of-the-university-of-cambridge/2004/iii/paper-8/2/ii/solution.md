<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the [formal pseudodifferential composition rule](../../../../../../formal-pseudodifferential-composition-rule.md) on each [coefficient](../../../../../../coefficient.md) $w_i(x)$ and then the exponential eigenfunction convention. For every [integer](../../../../../../integer.md) $n$,

$$
\partial^n\bigl(w_i(x)e^{kx}\bigr)
=e^{kx}\sum_{r\geq0}\binom nr w_i^{(r)}(x)k^{n-r}.
$$

Consequently

$$
Pw=k^\beta e^{kx}\sum_{j,i,r\geq0}
g_j\binom{\alpha-j}{r}w_i^{(r)}k^{\alpha-j-i-r}.
$$

Collecting all terms of a fixed power of the spectral parameter gives the useful answer

$$
\boxed{Pw=k^{\alpha+\beta}e^{kx}\sum_{s\geq0}\frac{v_s(x)}{k^s},\qquad
v_s=\sum_{i+j+r=s}g_j\binom{\alpha-j}{r}w_i^{(r)}.}
$$

The sum defining each $v_s$ is finite. For example,

$$
v_0=g_0w_0,\qquad
v_1=g_0w_1+g_1w_0+\alpha g_0w_0',
$$

and

$$
v_2=g_0w_2+g_1w_1+g_2w_0+\alpha g_0w_1'
+(\alpha-1)g_1w_0'+\binom\alpha2g_0w_0''.
$$

This is the action on a [formal pseudodifferential wave function](../../../../../../formal-pseudodifferential-wave-function.md). It is a formal expansion near $k=\infty$, with $k^\beta$ carried as a formal prefactor. It does not assert convergence for finite $k$, and negative powers are not evaluated at $k=0$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
