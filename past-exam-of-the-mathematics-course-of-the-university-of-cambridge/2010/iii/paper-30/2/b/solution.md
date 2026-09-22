<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Index the queue-class pairs by $a=(j,r)$. Let $\nu_a$ be the external [Poisson process](../../../../../../poisson-process.md) arrival rate, let $p_{ab}$ be the routing probability after class $a$ completes service, and put $p_{a0}=1-\sum_b p_{ab}$ for the exit probability. An open network has a transient routing matrix $P$, equivalently [spectral radius](../../../../../../spectral-radius.md) less than one. The effective throughputs solve the [traffic equations for a multiclass queueing network](../../../../../../traffic-equations-for-a-multiclass-queueing-network.md):

$$
\boxed{\lambda_a=\nu_a+\sum_b\lambda_b p_{ba},\qquad \lambda=(I-P^T)^{-1}\nu.}
$$

At each queue use the ordered [multiclass single-server queue](../../../../../../multiclass-single-server-queue.md) model of part (a), with parameters $\mu_{jr},\gamma_{ji},\delta_{ji}$. An external class-$a$ customer is inserted at position $i$ with rate $\nu_a\delta_{ji}(N_j+1)$. A customer of class $a$ in position $i$ completes at rate $\mu_a\gamma_{ji}(N_j)$: it exits with probability $p_{a0}$ or changes to class $b$ and is inserted at its destination with probability $p_{ab}\delta_{k\ell}(N_k'+1)$. Here $N_k'$ is the destination population after the origin deletion, so this also defines routes returning to the same queue. At each node, either service rates are common to its classes or insertion and service fractions form a [symmetric service discipline](../../../../../../symmetric-service-discipline.md).

Let $\rho_j=\sum_r\lambda_{jr}/\mu_{jr}<1$. The [product-form stationary distribution of a multiclass queueing network](../../../../../../product-form-stationary-distribution-of-a-multiclass-queueing-network.md) is

$$
\boxed{\pi((x_j)_j)=\prod_j(1-\rho_j)\prod_{i=1}^{N_j}\frac{\lambda_{j,c_{ji}}}{\mu_{j,c_{ji}}}.}
$$

To prove it by [time reversal of a continuous-time Markov chain](../../../../../../time-reversal-of-a-continuous-time-markov-chain.md), interchange each node's insertion and service fractions, and use

$$
\nu_a^*=\lambda_a p_{a0},\qquad
p_{ba}^*=\frac{\lambda_a p_{ab}}{\lambda_b},\qquad
p_{b0}^*=\frac{\nu_b}{\lambda_b}.
$$

Pairs with $\lambda_b=0$ can be deleted. The [traffic equations for a multiclass queueing network](../../../../../../traffic-equations-for-a-multiclass-queueing-network.md) ensure $\sum_a p_{ba}^*+p_{b0}^*=1$. The ratio of the product weights for an insertion is $\lambda_a/\mu_a$; for a deletion it is its reciprocal. Consequently every routing, entrance, and exit transition satisfies $\pi(x)q(x,x')=\pi(x')q^*(x',x)$. The symmetric or common-rate hypothesis makes each node's total service rate identical forward and backward. Summing the [traffic equations for a multiclass queueing network](../../../../../../traffic-equations-for-a-multiclass-queueing-network.md) also gives $\sum_a\nu_a^*=\sum_a\nu_a$. Thus the total transition rates match, proving [global balance for a continuous-time Markov chain](../../../../../../global-balance-for-a-continuous-time-markov-chain.md); each factor is normalized by part (a).

For the class counts the equilibrium law is

$$
\boxed{\pi((n_{jr})_{jr})=\prod_j(1-\rho_j)N_j!\prod_r\frac{(\lambda_{jr}/\mu_{jr})^{n_{jr}}}{n_{jr}!},\qquad N_j=\sum_r n_{jr}.}
$$

Under [processor sharing](../../../../../../processor-sharing.md) these counts have explicit transition rates $\nu_a$ for $n\to n+e_a$, $\mu_a n_a/N_j\,p_{a0}$ for $n\to n-e_a$, and $\mu_a n_a/N_j\,p_{ab}$ for $n\to n-e_a+e_b$. Under a closed network, remove external entrances and exits and normalize the same product weights on the conserved customer populations, using a positive solution of the homogeneous [traffic equations for a multiclass queueing network](../../../../../../traffic-equations-for-a-multiclass-queueing-network.md). That finite-state normalization does not require the open-network conditions $\rho_j<1$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
