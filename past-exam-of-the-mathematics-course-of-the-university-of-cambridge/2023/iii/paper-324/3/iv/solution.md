<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Now try only $k_i=2^i$. Since $n^*=2^N=\Theta(1/\theta)$, the total work through trial $N$ is the [geometric series](../../../../../../geometric-series.md)

$$
\sum_{i=0}^N2^i=2^{N+1}-1=\Theta(n^*).
$$

For $i<N$, the success probabilities scale as

$$
p_i=\sin^2((2^{i+1}+1)\theta)
=O\left(\frac{4^i}{(n^*)^2}\right).
$$

Their sum is $O(1)$, so the product of their failure probabilities stays bounded away from zero: there is a constant probability of reaching the scale $k_N=n^*$. At that trial, the defining property of $n^*$ gives

$$
p_N=\sin^2((2n^*+1)\theta)=1-O(\theta^2),
$$

so almost all surviving runs stop there. Therefore

$$
\boxed{\mathbb E C=\Theta(n^*)=\Theta(1/\theta)}.
$$

The [geometric amplitude-amplification schedule](../../../../../../geometric-amplitude-amplification-schedule.md) is asymptotically better than the sequential schedule's $\Theta((n^*)^{4/3})$ calls and matches the usual Grover scaling up to a constant factor.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
