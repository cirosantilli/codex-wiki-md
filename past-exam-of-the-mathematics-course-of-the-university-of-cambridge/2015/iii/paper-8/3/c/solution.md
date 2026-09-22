<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In the one-dimensional unit-mass setting, put $q=f/\gamma$. Using the convention $0\log0=0$, the [relative entropy](../../../../../../kullback-leibler-divergence.md) is

$$
H(f\mid\gamma)=\int f\log(f/\gamma)\,dv=\int\gamma\,q\log q\,dv.
$$

Because $\int\gamma q=\int f=1=\int\gamma$, we can subtract $q-1$ inside the integral:

$$
\boxed{H(f\mid\gamma)=\int\gamma(v)
[q(v)\log q(v)-q(v)+1]\,dv\geq0.}
$$

This is [relative entropy nonnegativity](../../../../../../relative-entropy-nonnegativity.md) from the given scalar inequality. Its integrand vanishes only at $q=1$, so **zero [relative entropy](../../../../../../kullback-leibler-divergence.md) characterizes $f=\gamma$ almost everywhere**. The nonnegativity remains valid with value $+\infty$ when entropy is not finite.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
