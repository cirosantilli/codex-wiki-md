<h1 id="1/3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the [scalar conservation law](../../../../../../../scalar-conservation-law.md), put $v_0(\xi)=f'(u_0(\xi))$ and $m=\min_\xi v_0'(\xi)=\min_\xi f''(u_0(\xi))u_0'(\xi)$. The [concave-flux characteristic lifespan](../../../../../../../concave-flux-characteristic-lifespan.md) and [characteristic flow map](../../../../../../../characteristic-flow-map.md) are

$$
\boxed{t^*=\begin{cases}-1/m,&m<0,\\ \infty,&m\ge0,\end{cases}\qquad X_t(\xi)=\xi+t f'(u_0(\xi)),\qquad u(t,X_t(\xi))=u_0(\xi).}
$$

For $t<t^*$, $X_t'=1+t v_0'>0$, and $X_t(\xi)=\xi+ct$ outside the support of $u_0$. Thus $X_t$ is a global smooth [diffeomorphism](../../../../../../../diffeomorphism.md) and the formula is $u(t,x)=u_0(X_t^{-1}(x))$. The [method of characteristics](../../../../../../../method-of-characteristics.md) proves existence and uniqueness among smooth solutions.

If $m<0$, at a minimizer $\xi_*$ the numerator $u_0'(\xi_*)$ is nonzero, since its product with $f''(u_0(\xi_*))$ is negative. Therefore

$$
u_x(t,X_t(\xi_*))=\frac{u_0'(\xi_*)}{1+t v_0'(\xi_*)}
$$

blows up as $t\uparrow t^*$, showing that this is the maximal smooth lifespan. Strict [concavity](../../../../../../../concave-function.md) alone does not require $f''$ to be negative at every point; the argument uses no such extra hypothesis.

## ↑ Ancestors (12)

1. [A](../a.md)
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
