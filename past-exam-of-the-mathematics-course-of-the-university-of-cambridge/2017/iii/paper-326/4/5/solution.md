<h1 id="4/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Use the standard [bounded linear operator](../../../../../../continuous-linear-operator.md) setting for $K:U\to V$, so the [adjoint operator](../../../../../../adjoint-operator.md) $K^*:V\to U^*$ in the updates is defined on every datum. Put $q=K^*Ku_\lambda$. The [generalized singular vector](../../../../../../generalized-singular-vector.md) relation is $\lambda q\in\partial J(u_\lambda)$ with $\|Ku_\lambda\|=1$ and $\lambda=J(u_\lambda)\geq0$. For an [absolutely one-homogeneous functional](../../../../../../absolutely-one-homogeneous-functional.md), a [subgradient](../../../../../../subgradient.md) $p$ at $u$ is characterized by $\langle p,u\rangle=J(u)$ and $\langle p,v\rangle\leq J(v)$ for all $v$. Consequently $\lambda q$ is also a [subgradient](../../../../../../subgradient.md) at every positive multiple of $u_\lambda$, and $bq\in\partial J(0)$ for every $0\leq b\leq\lambda$.

Use the initialization $u^0=p^0=0$ and start the first update at $k=0$; the PDF lists $k=1,2,\ldots$ despite specifying only index-zero initial data. Suppose $p^k=b_kq$ with $0\leq b_k\leq\lambda$. Define

$$
c_{k+1}=[\gamma-\alpha(\lambda-b_k)]_+.
$$

If it is positive, $u^{k+1}=c_{k+1}u_\lambda$ and $p^{k+1}=\lambda q$ satisfy the optimality equation and the dual update. If it is zero, take $u^{k+1}=0$ and $p^{k+1}=(b_k+\gamma/\alpha)q\in\partial J(0)$. Thus this compatible branch has

$$
b_{k+1}=\min\{\lambda,b_k+\gamma/\alpha\}.
$$

Induction proves the [finite termination of Bregman iteration on a singular vector](../../../../../../finite-termination-of-bregman-iteration-on-a-singular-vector.md) formulas

$$
\boxed{p^k=\min\{k\gamma/\alpha,\lambda\}q,\qquad u^k=\min\{\gamma,(k\gamma-\alpha\lambda)_+\}u_\lambda\quad(k\geq1).}
$$

Once the dual coefficient reaches $\lambda$, the next reconstruction is $\gamma u_\lambda$. Therefore a guaranteed stopping index for this branch is

$$
\boxed{k_*=\left\lceil\frac{\alpha\lambda}{\gamma}\right\rceil+1.}
$$

The formulas also cover $\lambda=0$, where exact reconstruction occurs at the first update. The [subgradient](../../../../../../subgradient.md) conditions are sufficient for global minimization because each objective is convex.

There is a genuine uniqueness issue in the printed claim about arbitrary iterates. Strict convexity of data fidelity in $Ku$ ensures that any two minimizers at a given step have the same image under $K$. Induction therefore makes every minimizer branch have the same dual variables and attain exact data at the stated finite index. It does not make their states equal to the specified $\gamma u_\lambda$ if $K$ has a [null space](../../../../../../kernel-of-a-linear-map.md).

For a counterexample take $U=\mathbb R^2$, $V=\mathbb R$, $K(x,y)=x$, $J(x,y)=|x|$, $u_\lambda=(1,0)$, and $\lambda=1$. Every step leaves $y$ completely unconstrained. Choosing the minimizing state's second coordinate to be $k$ gives valid updates and [subgradients](../../../../../../subgradient.md) but never reaches $(\gamma,0)$ and does not converge as a state [sequence](../../../../../../sequence.md). Thus **finite exact-data recovery holds for all minimizer branches; exact recovery of the stated vector needs uniqueness or the aligned branch**. If $K$ is injective, equal reconstructed data identify the state, and the literal vector conclusion follows.

## ↑ Ancestors (11)

1. [5](../5.md)
2. [4](../../4.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
