<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $(\phi_j)$ be a smooth [orthonormal eigenbasis](../../../../../../orthonormal-eigenbasis.md) of the [positive Laplace-Beltrami operator](../../../../../../positive-laplace-beltrami-operator.md), with [eigenvalues](../../../../../../eigenvalue.md) $(\lambda_j)$. The [orthonormal eigenbasis](../../../../../../orthonormal-eigenbasis.md) defines

$$
e^{-t\Delta}f=\sum_j e^{-t\lambda_j}\langle f,\phi_j\rangle\phi_j.
$$

The large-$j$ lower bound of part (c), valid also after the finitely many zero modes of a disconnected [compact manifold](../../../../../../compact-manifold.md), gives $\lambda_j\geq a j^{2/n}$ for sufficiently large $j$. Hence

$$
\sum_j e^{-t\lambda_j}<\infty\qquad(t>0),
$$

by comparison with $\int_0^\infty e^{-ta x^{2/n}}\,dx$. The operator is positive and diagonal with these summable coefficients, so it is a [trace-class operator](../../../../../../trace-class-operator.md) and its [operator trace](../../../../../../operator-trace.md) is their sum.

Its proposed [heat kernel](../../../../../../heat-kernel.md) is

$$
K_t(x,y)=\sum_j e^{-t\lambda_j}\phi_j(x)\overline{\phi_j(y)}.
$$

We verify smoothness and the kernel action. The [elliptic regularity](../../../../../../elliptic-regularity.md) estimate established in Question 4(d) gives, by induction,

$$
\|\phi_j\|_{H^{2r}}\leq C_r(1+\lambda_j)^r.
$$

The [Sobolev embedding theorem](../../../../../../sobolev-embedding-theorem.md) therefore gives, for every derivative order $a$, constants $C_a$, $r_a$ with $\|\phi_j\|_{C^a}\leq C_a(1+\lambda_j)^{r_a}$. Every differentiated term of the kernel series is bounded by $C_{a,b}e^{-t\lambda_j}(1+\lambda_j)^{r_a+r_b}$. An exponential absorbs any fixed power: for $t\geq\tau>0$ this is at most $C_{a,b,\tau}e^{-\tau\lambda_j/2}$, a summable bound. Time derivatives merely introduce more powers of $\lambda_j$. Thus the series converges uniformly with all spatial and time derivatives on $[\tau,\infty)\times M\times M$. In particular $K_t$ is smooth for every $t>0$.

Integrating its uniformly convergent series against $f\in L^2(M)$ is legitimate since the [compact manifold](../../../../../../compact-manifold.md) has finite volume and $L^2(M)\subseteq L^1(M)$. It gives exactly the spectral expression above, so

$$
(e^{-t\Delta}f)(x)=\int_MK_t(x,y)f(y)\,d\mathrm{vol}_g(y).
$$

Finally $K_t(x,x)=\sum_j e^{-t\lambda_j}|\phi_j(x)|^2$ is nonnegative. Integrating term by term, either by uniform convergence or by [Tonelli theorem](../../../../../../tonelli-theorem.md), and using $\|\phi_j\|_2=1$ proves the [heat kernel trace formula](../../../../../../heat-kernel-trace-formula.md)

$$
\boxed{\operatorname{Tr}e^{-t\Delta}=\sum_j e^{-t\lambda_j}=\int_MK_t(x,x)\,d\mathrm{vol}_g(x),\qquad t>0.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
