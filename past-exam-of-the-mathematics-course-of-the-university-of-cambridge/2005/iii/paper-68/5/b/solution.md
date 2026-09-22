<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the order of the three [Bernstein basis](../../../../../../bernstein-basis.md) functions given in this part. Endpoint evaluation gives

$$
a_1=p(1),\qquad a_3=p(0),
$$

so both endpoint coefficients have absolute value at most one. At the midpoint,

$$
p(1/2)=\frac14a_1+\frac12a_2+\frac14a_3,
\qquad
a_2=2p(1/2)-\frac12[p(0)+p(1)].
$$

The [triangle inequality](../../../../../../triangle-inequality.md) therefore gives the [quadratic Bernstein coefficient bound](../../../../../../quadratic-bernstein-coefficient-bound.md)

$$
\boxed{|a_1|\leq1,\qquad |a_2|\leq3,\qquad |a_3|\leq1.}
$$

All three bounds are sharp. Indeed $p(x)=8x^2-8x+1=T_2(2x-1)$ has [uniform norm](../../../../../../supremum-norm.md) one and coefficient vector $(1,-3,1)$ in this basis. The reversed ordering of endpoint Bernstein functions does not affect these symmetric endpoint bounds.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 68](../../../paper-68-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
