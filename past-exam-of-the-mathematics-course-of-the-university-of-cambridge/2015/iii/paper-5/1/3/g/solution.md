<h1 id="1/3/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Write $M=\|u_0\|_{L^1}$. Since $|U(0,y)|\le M$, choosing $y=x-ct$ gives $g((x-y)/t)=g(c)=0$ and $\max_yG_{t,x}(y)\ge-M$. At the maximizing foot $x_0$, the [inverse-flux quadratic bounds](../../../../../../../inverse-flux-quadratic-bounds.md) give

$$
\max_yG_{t,x}(y)=U(0,x_0)+t g\left(\frac{x-x_0}{t}\right)\le M+\frac{k_+}{t}(x-x_0-ct)^2.
$$

Combining the two estimates and dividing by $-k_+>0$ gives

$$
\boxed{\left|\frac{x-x_0}{t}-c\right|\le\sqrt{\frac{2M}{-k_+t}},\qquad |u(t,x)|\le\frac{-2k_-}{\sqrt t}\sqrt{\frac{2M}{-k_+}}.}
$$

The last step uses $u=h((x-x_0)/t)$ and the sign-independent bound on $h$. This is [square-root decay before characteristic crossing](../../../../../../../square-root-decay-before-characteristic-crossing.md); it is proved only for $0<t<t^*$. No continuation past [characteristic crossing](../../../../../../../characteristic-crossing.md) or global-time smoothness is assumed. If $M=0$, the initial function and the solution vanish.

## ↑ Ancestors (12)

1. [G](../g.md)
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
