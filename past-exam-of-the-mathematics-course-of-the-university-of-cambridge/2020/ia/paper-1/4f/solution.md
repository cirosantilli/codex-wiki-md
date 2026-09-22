<h1 id="4f/solution">Solution</h1>

↑ **Parent:** [4F](../4f.md)

Let $Z_n$ be the size of generation $n$. This is a [Galton-Watson process](../../../../../galton-watson-process.md) with offspring mean

$$
m=0\cdot\frac1{12}+1\cdot\frac12
+2\cdot\frac13+3\cdot\frac1{12}
=\frac{17}{12}.
$$

The [expected generation size in a Galton-Watson process](../../../../../expected-generation-size-in-a-galton-watson-process.md) is therefore

$$
\boxed{\mathbb E Z_n=\left(\frac{17}{12}\right)^n}.
$$

Its [probability generating function](../../../../../probability-generating-function.md) is

$$
G(s)=\frac1{12}+\frac12s+\frac13s^2+\frac1{12}s^3.
$$

By the [Galton-Watson extinction fixed point](../../../../../galton-watson-extinction-fixed-point.md), the extinction probability $q$ is the smallest solution in $[0,1]$ of $G(q)=q$. Factoring gives

$$
q^3+4q^2-6q+1=(q-1)(q^2+5q-1)=0,
$$

so $q=(\sqrt{29}-5)/2$. The probability of production continuing forever is

$$
\boxed{1-q=\frac{7-\sqrt{29}}2}.
$$

## ↑ Ancestors (10)

1. [4F](../4f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
