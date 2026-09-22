<h1 id="20h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let the common initial state be $x$ and the robber's final state be $y$. Part (a) gives their joint distribution as

$$
\pi(x)P^*(x,y)=\pi(y)P(y,x).
$$

Let $\tau_y=\min\{n\geq0:X_n=y\}$ be the cop's [hitting time](../../../../../../first-passage-time.md) of $y$ when starting from $x$. For a chain started from $y$, condition on its first step to obtain

$$
\mathbb E_yT_y^+=1+\sum_xP(y,x)\mathbb E_x\tau_y.
$$

Hence the expected catch time, averaged over the displayed joint law, is

$$
\sum_{x,y}\pi(y)P(y,x)\mathbb E_x\tau_y
=\sum_y\pi(y)\left(\mathbb E_yT_y^+-1\right).
$$

Using [Kac's lemma](../../../../../../kac-s-lemma.md) once more gives

$$
\boxed{\mathbb E[\text{catch time}]
=\sum_y\pi(y)\left(\frac1{\pi(y)}-1\right)=N-1}.
$$

The convention $\tau_y=0$ correctly counts an immediate catch when the robber's reverse step leaves it at the common starting state.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [20H](../../20h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
