<h1 id="19h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $D,E,F$ be the midpoints of $AB,AC,BC$. Write

$$
a=\mathbb E_A T_{BC},\qquad
d=\mathbb E_D T_{BC}=\mathbb E_E T_{BC},\qquad
f=\mathbb E_F T_{BC}.
$$

[First-step analysis](../../../../../../first-step-analysis.md) for the [simple random walk](../../../../../../simple-random-walk.md) gives

$$
a=1+d,
$$

because $A$ has neighbours $D,E$;

$$
d=1+\frac{a+d+f}{4},
$$

because $D$ has neighbours $A,B,E,F$; and

$$
f=1+\frac d2,
$$

because $F$ has neighbours $B,C,D,E$. Solving,

$$
d=4,\qquad f=3,\qquad
\boxed{\mathbb E_A T_{BC}=a=5}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [19H](../../19h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
