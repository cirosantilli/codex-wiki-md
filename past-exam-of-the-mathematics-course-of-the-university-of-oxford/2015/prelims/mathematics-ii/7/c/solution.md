<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Again let $G=\int_a^bg(t)\,dt\geq0$ and $I=\int_a^bf(t)g(t)\,dt$. Since $f$ is a nondecreasing [monotonic function](../../../../../../monotonic-function.md), $f(a)\leq f(t)\leq f(b)$ on $[a,b]$. The condition $g\geq0$ and the [monotonicity of the Riemann integral](../../../../../../monotonicity-of-the-riemann-integral.md) give

$$
f(a)G\leq I\leq f(b)G.
$$

Set $H(x)=\int_a^xg(t)\,dt$. By part (a), $H$ is [continuous](../../../../../../continuous-function.md). Therefore the [function](../../../../../../function-split.md)

$$
K(x)=f(a)H(x)+f(b)\bigl(G-H(x)\bigr)
$$

is [continuous](../../../../../../continuous-function.md) on $[a,b]$. Its endpoint values are $K(a)=f(b)G$ and $K(b)=f(a)G$, which enclose $I$. The [intermediate value theorem](../../../../../../intermediate-value-theorem.md) provides $d\in[a,b]$ with $K(d)=I$, so

$$
\boxed{\int_a^bf(t)g(t)\,dt=f(a)\int_a^dg(t)\,dt+f(b)\int_d^bg(t)\,dt.}
$$

If the two endpoint values coincide, the preceding bounds force $I$ to equal that common value and either endpoint works. Thus the proof also covers $G=0$, $f(a)=f(b)$ and $a=b$, without dividing by any possibly zero quantity.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [7](../../7.md)
3. [Mathematics II](../../../mathematics-ii-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
