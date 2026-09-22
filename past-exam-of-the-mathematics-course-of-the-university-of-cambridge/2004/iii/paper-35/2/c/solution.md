<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use $w$ for current wealth and $\pi=w-B$ for the dollar position in the risky asset. Its controlled dynamics have drift $rw+(\mu-r)\pi$ and diffusion coefficient $\sigma\pi$. Over a short time step $h$, the [dynamic programming principle](../../../../../../dynamic-programming-principle.md) gives

$$
J(w,t)=\sup_\pi\mathbb E\left[\int_t^{t+h}e^{-\rho s}W_s^\gamma ds+J(W_{t+h},t+h)\mid W_t=w\right].
$$

Apply [Itô formula](../../../../../../ito-s-lemma.md) to the second term, divide by $h$, and let $h\downarrow0$. The [Hamilton-Jacobi-Bellman equation](../../../../../../hamilton-jacobi-bellman-equation.md) is

$$
0=e^{-\rho t}w^\gamma+J_t+\sup_\pi\left\{[rw+(\mu-r)\pi]J_w+\frac12\sigma^2\pi^2J_{ww}\right\}.
$$

For the increasing concave value function, $J_w>0$ and $J_{ww}<0$, so the expression is a strictly concave quadratic in the risky position. Its derivative vanishes at

$$
\pi^*=-\frac{\mu-r}{\sigma^2}\frac{J_w}{J_{ww}},\qquad
\boxed{B^*=w+\frac{\mu-r}{\sigma^2}\frac{J_w}{J_{ww}}.}
$$

Substitution of this maximizer yields

$$
\boxed{J_t+rwJ_w-\frac12\left(\frac{\mu-r}{\sigma}\right)^2\frac{J_w^2}{J_{ww}}+e^{-\rho t}w^\gamma=0,\qquad J(w,T)=w^\gamma.}
$$

There is a running utility reward but no consumption withdrawal in the wealth dynamics. The required concavity is also verified explicitly by the positive coefficient in part (d), so this stationary point really is the maximum.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
