<h1 id="12g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For

$$
g(z)=\frac{e^z-1}{z\log(1+z)},
$$

both $e^z-1$ and $\log(1+z)$ have a simple zero at zero. Hence $g$ has a simple pole, and its [residue](../../../../../../residue.md) is

$$
\operatorname{Res}(g,0)
=\lim_{z\to0}\frac{e^z-1}{\log(1+z)}
=\boxed{1}.
$$

For $h(z)=\sin z\sin(1/z)$, multiplication of the two Laurent series shows that all powers are even:

$$
h(z)=
\sum_{p,q\geq0}
\frac{(-1)^{p+q}}{(2p+1)!(2q+1)!}\,
z^{2(p-q)}.
$$

There are infinitely many negative powers, so zero is an [essential singularity](../../../../../../essential-singularity.md). There is no $z^{-1}$ term, and therefore

$$
\boxed{\operatorname{Res}(h,0)=0}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [12G](../../12g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
