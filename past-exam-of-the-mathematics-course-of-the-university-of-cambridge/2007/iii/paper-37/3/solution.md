<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $\mathcal T$ be the set of three-vertex subsets and let $I_A$ indicate that $A$ forms a triangle. Then

$$
X=\sum_{A\in\mathcal T}I_A,\qquad
p_A=\mathbb EI_A=p^3,\qquad
\mu_n=\binom n3p^3\longrightarrow\alpha.
$$

In particular $p\sim(6\alpha)^{1/3}/n$. We will use the [Stein-Chen method](../../../../../stein-chen-method.md) with edge-sharing dependency neighborhoods, rather than wrongly treating triangle indicators as mutually independent.

Here is the needed [Poisson approximation with dependency neighborhoods](../../../../../poisson-approximation-with-dependency-neighborhoods.md), together with its proof. For indicators $I_A$ with means $p_A$, let $B_A$ contain $A$ and suppose $I_A$ is independent of the entire family of indicators outside $B_A$. With $\mu=\sum_Ap_A$ and $W=\sum_AI_A$, define

$$
b_1=\sum_A\sum_{C\in B_A}p_Ap_C,\qquad
b_2=\sum_A\sum_{C\in B_A\setminus\{A\}}\mathbb E(I_AI_C).
$$

The [total variation distance](../../../../../total-variation-distance.md) convention is $d_{TV}(P,Q)=\sup_E|P(E)-Q(E)|$. We claim

$$
d_{TV}(\mathcal L(W),\operatorname{Poisson}(\mu))\le b_1+b_2.
$$

For an indicator test function $g$ on the nonnegative integers, solve the [Poisson Stein equation](../../../../../poisson-stein-equation.md)

$$
\mu f(k+1)-kf(k)=g(k)-\mathbb Eg(Z),\qquad Z\sim\operatorname{Poisson}(\mu),
$$

with $\|\Delta f\|_\infty\le1$. This elementary Stein factor can be proved as follows. Take the [immigration--death process](../../../../../immigration-death-process.md) with immigration rate $\mu$ and per-particle death rate one. Starting at $k$, its time-$t$ distribution is

$$
Z_t^k\overset d=\operatorname{Binomial}(k,e^{-t})+
\operatorname{Poisson}(\mu(1-e^{-t})),
$$

with independent summands. Its stationary law is that of $Z$. Coupling the initial particles with a stationary Poisson initial population makes the centered [expectations](../../../../../expected-value.md) decay at least as a constant times $(k+\mu)e^{-t}$, so

$$
u(k)=-\int_0^\infty\bigl(\mathbb Eg(Z_t^k)-\mathbb Eg(Z)\bigr)\,dt
$$

is finite. Its generator equation is $\mu(u(k+1)-u(k))+k(u(k-1)-u(k))=g(k)-\mathbb Eg(Z)$, obtained by integrating the semigroup derivative. Set $f(k)=u(k)-u(k-1)$ for $k\ge1$; choose $f(0)=f(1)$, which does not affect the equation. To bound $\Delta f(k)$, couple the processes starting at $k-1,k,k+1$ by adding two independent initial particles. Both survive to time $t$ with probability $e^{-2t}$, and otherwise their second difference cancels in [expectation](../../../../../expected-value.md). Since $|g(j+2)-2g(j+1)+g(j)|\le2$,

$$
|u(k+1)-2u(k)+u(k-1)|\le\int_0^\infty2e^{-2t}\,dt=1.
$$

This proves the Stein factor for $k\ge1$, and the chosen $f(0)$ handles $k=0$.

Put $W_A=W-\sum_{C\in B_A}I_C$. [Independence](../../../../../independent-random-variables.md) gives $\mathbb E[I_Af(W_A+1)]=p_A\mathbb Ef(W_A+1)$. Inserting this identity into the Stein equation yields

$$
\begin{aligned}
\mathbb Eg(W)-\mathbb Eg(Z)
={}&\sum_Ap_A\mathbb E[f(W+1)-f(W_A+1)]\\
&+\sum_A\mathbb E\bigl[I_A(f(W_A+1)-f(W))\bigr].
\end{aligned}
$$

The first sum in absolute value is at most $b_1$, since the two arguments differ by $\sum_{C\in B_A}I_C$. In the second sum, on $I_A=1$ the arguments differ by $\sum_{C\in B_A\setminus\{A\}}I_C$, giving bound $b_2$. Taking the supremum over event indicators $g$ proves the claimed [total variation distance](../../../../../total-variation-distance.md) bound.

For triangle $A$, choose $B_A$ to consist of $A$ itself and all triangles sharing an edge with $A$. There are exactly $1+3(n-3)$ such triangles. Every outside triangle uses none of the three edges of $A$, even if it shares one vertex, so $I_A$ is independent of their entire indicator family. For distinct neighboring triangles, their union has five edges and $\mathbb E(I_AI_C)=p^5$. Therefore

$$
b_1=\binom n3(1+3(n-3))p^6=O(n^{-2}),\qquad
b_2=\binom n3\,3(n-3)p^5=O(n^{-1}).
$$

The [Stein-Chen method](../../../../../stein-chen-method.md) gives $d_{TV}(\mathcal L(X),\operatorname{Poisson}(\mu_n))\to0$. Coupling [Poisson distributions](../../../../../poisson-distribution.md) of two means by adding an independent Poisson variable gives

$$
d_{TV}(\operatorname{Poisson}(\mu_n),\operatorname{Poisson}(\alpha))
\le1-e^{-|\mu_n-\alpha|}\le|\mu_n-\alpha|\longrightarrow0.
$$

This proves the [Poisson limit for triangles in a binomial random graph](../../../../../poisson-limit-for-triangles-in-a-binomial-random-graph.md):

$$
\boxed{d_{TV}(\mathcal L(X),\operatorname{Poisson}(\alpha))\longrightarrow0.}
$$

Applying the same bound to the event $\{1,2,\ldots\}$ gives

$$
\boxed{\mathbb P(X\ge1)\longrightarrow1-e^{-\alpha}.}
$$

For finite $n$ this is an approximation, not an exact formula: the error from $1-e^{-\mu_n}$ is at most $b_1+b_2$, and the error from $1-e^{-\alpha}$ is at most $b_1+b_2+|\mu_n-\alpha|$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 37](../../paper-37-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
