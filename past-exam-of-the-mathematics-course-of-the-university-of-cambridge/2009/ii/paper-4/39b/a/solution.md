<h1 id="39b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Interpolate through the $s+1$ values at $t_n,\ldots,t_{n+s}$, and differentiate the interpolation [polynomial](../../../../../../polynomial-split.md) at its newest node. In the backward coordinate $\tau=(t-t_{n+s})/h$, the Newton form is

$$
P(\tau)=\sum_{j=0}^s\frac{\tau(\tau+1)\cdots(\tau+j-1)}{j!}\,\nabla^j y_{n+s},
$$

with the $j=0$ factor interpreted as one and $\nabla y_m=y_m-y_{m-1}$. For $j\ge1$, the derivative of the factor at zero is $(j-1)!/j!=1/j$. Thus the [backward differentiation formula](../../../../../../backward-differentiation-formula.md) is

$$
\sum_{j=1}^s\frac1j\nabla^j y_{n+s}=h f_{n+s}.
$$

If $w$ denotes the forward-shift variable, $\nabla^j y_{n+s}$ corresponds to $w^{s-j}(w-1)^j$. Consequently the requested [polynomial](../../../../../../polynomial-split.md) is

$$
\boxed{\rho(w)=\sum_{j=1}^s\frac1j w^{s-j}(w-1)^j
=w^s\sum_{j=1}^s\frac{(1-w^{-1})^j}{j}.}
$$

The first form is a [polynomial](../../../../../../polynomial-split.md) valid also at $w=0$. The second form is convenient for relating it to the truncated series of $\log w$. Differentiation of the degree-$s$ interpolant has local derivative error $O(h^s)$, giving order $s$ for smooth solutions.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [39B](../../39b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
