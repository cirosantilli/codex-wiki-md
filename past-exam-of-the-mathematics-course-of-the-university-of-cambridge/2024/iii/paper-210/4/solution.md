<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

One form of [Assouad's lemma](../../../../../assouad-s-lemma.md) is as follows. Let $\{P_\omega:\omega\in\{0,1\}^m\}$ be a statistical experiment and suppose parameters satisfy

$$
d(\theta_\omega,\theta_{\omega'})^2
\geq\rho^2d_H(\omega,\omega').
$$

If adjacent vertices of the hypercube satisfy

$$
\lVert P_\omega-P_{\omega\oplus e_j}\rVert_{\mathrm{TV}}\leq\alpha<1,
$$

then every estimator obeys

$$
\sup_\omega\mathbb E_\omega
d(\widehat\theta,\theta_\omega)^2
\geq\frac{m\rho^2}{8}(1-\alpha),
$$

up to the inessential convention-dependent universal constant.

Construct a hypercube inside the convex cone. Start from $f_*(x)=x^2$. Partition most of $[0,1]$ into $m=\lfloor n/k\rfloor$ consecutive blocks of $k$ grid intervals. On block $j$, let $\phi_j$ be the chord joining the two endpoint values of $f_*$ minus $f_*$ inside the block, and zero outside. For $\omega\in\{0,1\}^m$, set

$$
f_\omega=f_*+\sum_{j=1}^m\omega_j\phi_j,
\qquad
\theta_{\omega,i}=f_\omega(i/n).
$$

Replacing a convex arc by its chord leaves a convex, nondecreasing function. Its values remain in $[0,1]$, so every $\theta_\omega$ belongs to $C_n\cap M_n\cap[0,1]^n$, and hence also to the larger parameter set in the first claim.

The perturbations have disjoint supports. For neighboring hypercube vertices their squared Euclidean separation is independent of the block and, using the supplied sum, satisfies

$$
\rho^2
=\sum_{\ell=0}^{k-1}
\frac{\ell^2(k-1-\ell)^2}{n^4}
=\frac{k(k-1)(k-2)(k^2-2k+2)}{30n^4}
\asymp\frac{k^5}{n^4}.
$$

The observations have identity covariance, so the [Kullback-Leibler divergence between normal distributions](../../../../../kullback-leibler-divergence-between-normal-distributions.md) for neighboring vertices is $\rho^2/2$. Choose

$$
k=\lfloor c_0n^{4/5}\rfloor
$$

with a sufficiently small universal $c_0>0$. Then $\rho^2$ is bounded above by a small constant and below by another positive constant for all sufficiently large $n$. [Pinsker's inequality](../../../../../pinsker-s-inequality.md) makes every neighboring total-variation distance at most some fixed $\alpha<1$.

Assouad's lemma, with squared Euclidean loss divided by $n$, now gives

$$
\inf_{\widehat\theta}\sup_{\theta\in C_n\cap[0,1]^n}
\frac1n\mathbb E_\theta\lVert\widehat\theta-\theta\rVert_2^2
\geq c\,\frac mn
\asymp c\,\frac1k
\asymp c\,n^{-4/5}.
$$

The same hypercube already lies in $C_n\cap M_n\cap[0,1]^n$. Therefore that smaller class has the same $cn^{-4/5}$ minimax lower bound. An upper bound $Cn^{-\gamma}$ with $\gamma>4/5$ would eventually be smaller, which is impossible. Thus no estimator with the proposed uniform rate can exist.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 210](../../paper-210-split.md)
3. [Iii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
