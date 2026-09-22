<h1 id="31b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For any fixed $t>0$, the characteristic map $X_t(\xi)=\xi+t u_I(\xi)$ has [derivative](../../../../../../derivative.md) $1+t u_I'(\xi)>1$. It is strictly increasing and onto: for $\xi\geq0$ it is at least $\xi+t u_I(0)$, and for $\xi\leq0$ at most that quantity. Hence the inverse function theorem supplies a global $C^1$ inverse. Define $u(x,t)=u_I(X_t^{-1}(x))$. Differentiating gives

$$
u_x=\frac{u_I'(\xi)}{1+t u_I'(\xi)},\qquad
u_t=-\frac{u_I(\xi)u_I'(\xi)}{1+t u_I'(\xi)}=-uu_x.
$$

The [derivatives](../../../../../../derivative.md) are continuous, and $u_x\leq1/t$ for positive times. Thus **a classical solution exists for all $t>0$**, without any characteristic intersection or shock formation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [31B](../../31b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
