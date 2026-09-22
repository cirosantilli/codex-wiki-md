<h1 id="32a/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

At $(1,y_0)$ the trajectory initially moves into $x>1$. Suppose $y$ had a first zero at time $t_*>0$. Before that time $y>0$, hence $x(t_*)>1$. Since $U'(x)<0$ for $x>1$,

$$
\dot y(t_*)=-U'(x(t_*))>0,
$$

which is incompatible with crossing from positive values to zero. Thus

$$
y(t)>0,\qquad x(t)>1
$$

for all $t>0$.

The energy from part (b) decreases strictly because

$$
\dot E=-ky^2<0.
$$

Since $U\geq0$,

$$
\frac12y(t)^2
\leq E(t)
<E(0)
=\frac12y_0^2+\frac14.
$$

Therefore

$$
\boxed{0<y(t)<\sqrt{y_0^2+\frac12}}
\qquad(t>0).
$$

Finally, fix $\varepsilon>0$. If the trajectory never entered $0<y<\varepsilon$, positivity would force $y(t)\geq\varepsilon$ for all $t>0$. Then

$$
\dot E(t)=-ky(t)^2\leq-k\varepsilon^2,
$$

so

$$
E(t)\leq E(0)-k\varepsilon^2t,
$$

which becomes negative for large $t$, contradicting $E\geq0$. Hence the trajectory must enter every such strip. This proves [outward escape from the rational potential barrier](../../../../../../outward-escape-from-the-rational-potential-barrier.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [32A](../../32a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
