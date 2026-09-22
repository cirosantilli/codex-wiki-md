<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The possible singular points are $i,-i,1$. Near $i$, put $h(z)=1/((z+i)(z-1)^2)$; then

$$
f(z)=\frac{h(z)-1/4}{z-i},\qquad h(i)=\frac14.
$$

The numerator vanishes at $i$, so the apparent pole cancels and **$i$ is removable**. Its extension value is $h'(i)=1/4+3i/8$, obtained from $h'/h=-1/(z+i)-2/(z-1)$.

At $-i$, the first term has a simple [pole](../../../../pole.md) with nonzero [residue](../../../../residue.md)

$$
\lim_{z\to-i}(z+i)f(z)=\frac1{(-2i)(-i-1)^2}=\frac14.
$$

The subtracted term is holomorphic there, so **$-i$ is a simple pole**. At $1$,

$$
\lim_{z\to1}(z-1)^2f(z)=\frac1{1^2+1}=\frac12\ne0,
$$

so **$1$ is a double pole**. There are no other finite singularities.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
