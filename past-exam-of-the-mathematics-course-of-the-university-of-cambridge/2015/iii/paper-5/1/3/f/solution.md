<h1 id="1/3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

**The printed linear ordering is false for $z<c$.** For example, $f(s)=-s^2/2$, $c=0$, $h(z)=-z$, $k_-=-3/4$, $k_+=-1/4$ satisfy the derivative hypothesis, but at $z=-1$ the printed lower bound would require $3/4\le1/2$.

The correct [inverse-flux quadratic bounds](../../../../../../../inverse-flux-quadratic-bounds.md) are

$$
\boxed{\begin{aligned}
k_-(z-c)&\le h(z)/2\le k_+(z-c)&& (z\ge c),\\
k_+(z-c)&\le h(z)/2\le k_-(z-c)&& (z\le c),\\
k_-(z-c)^2&\le g(z)\le k_+(z-c)^2&& (z\in\mathbb R).
\end{aligned}}
$$

Indeed $h(c)=0$ and $h(z)/2=\int_c^z h'(r)/2\,dr$; reversing the integration limits reverses the linear inequalities. Equivalently, for $z\ne c$, $k_-\le h(z)/(2(z-c))\le k_+$. Since $g(c)=0$ and $g'=h$, integration once more gives the quadratic inequalities on both sides of $c$. A useful sign-independent consequence is $|h(z)|\le-2k_-|z-c|$.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [3](../../3.md)
3. [1](../../../1.md)
4. [Paper 5](../../../../paper-5-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
