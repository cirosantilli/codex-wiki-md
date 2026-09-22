<h1 id="22g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose $A>0$ and set

$$
M=\max_{|x|\leq A}|\phi(x)|.
$$

Take

$$
T_1\leq\frac A{\max\{M,1\}}.
$$

Inductively, if $|f_n(s)|\leq A$ on $[0,T_1]$, then

$$
|f_{n+1}(t)|
\leq\int_0^t|\phi(f_n(s))|\,ds
\leq MT_1\leq A.
$$

Since $f_0=0$, every iterate is bounded by $A$. Moreover,

$$
|f_{n+1}(t)-f_{n+1}(s)|
=\left|\int_s^t\phi(f_n(r))\,dr\right|
\leq M|t-s|.
$$

**Thus $(f_n)_{n\geq1}$ is uniformly bounded and uniformly Lipschitz, hence equicontinuous, on $[0,T_1]$.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [22G](../../22g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
