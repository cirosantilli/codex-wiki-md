<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume the innovations are [independent](../../../../../../independent-random-variables.md) of the previous history and have finite [exponential moments](../../../../../../exponential-moment.md) at every real argument, as required by the finite-valued affine definition. Conditioning on $X_{t-1}=x$ gives

$$
\log\mathbb E[e^{\theta X_t}\mid X_{t-1}=x]=a\theta x+b\theta+\psi(\theta).
$$

Hence the [autoregressive process of order one](../../../../../../autoregressive-process-of-order-one.md) is an [affine process](../../../../../../affine-process.md), with

$$
\boxed{A(\theta)=a\theta,\qquad B(\theta)=b\theta+\psi(\theta).}
$$

Here and in the remaining parts, an [affine process](../../../../../../affine-process.md) uses a time-homogeneous [Markov process](../../../../../../markov-process-split.md): the one-step transform is the same at every time. The displayed definition at time $1$ alone would not determine later transitions of an arbitrary time-inhomogeneous [Markov process](../../../../../../markov-process-split.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
