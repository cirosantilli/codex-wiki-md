<h1 id="27j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

After a record of value $v$, the first subsequent observation exceeding it has the original distribution conditioned on $X>v$. Indeed, summing over the number of failed observations gives the density

$$
\sum_{j=0}^\infty F(v)^j f(w)\mathbf1_{w>v}=\frac{f(w)}{1-F(v)}\mathbf1_{w>v}.
$$

Independence makes this conditional transition depend only on the latest record. Multiplying these transitions, starting with the density $f(v_1)$, proves

$$
\boxed{f_{V_1,\ldots,V_n}=\mathbf1_{0<v_1<\cdots<v_n}\,f(v_1)\prod_{j=2}^n\frac{f(v_j)}{1-F(v_{j-1})}.}
$$

The ordering indicator is part of the density; it is zero elsewhere. Continuity of the observation distribution avoids ties.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [27J](../../27j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
