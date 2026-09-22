<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [Gillespie algorithm](../../../../../../gillespie-algorithm.md), start from $t=0$ and an integer [molecular copy number](../../../../../../molecular-copy-number.md) $x\ge0$. At each step use the current state, without the mean approximation in parts (a)–(b). The [reaction propensity functions](../../../../../../reaction-propensity-function.md) are $a_+(x)=\lambda$ and $a_-(x)=\beta\sqrt x$, and their sum is $a_0(x)=\lambda+\beta\sqrt x$. Draw two independent [uniform random variables](../../../../../../uniform-random-variable.md) $U_1,U_2$ on $(0,1)$ and set

$$
\Delta t=-\frac{\log U_1}{a_0(x)}.
$$

The waiting time has an [exponential distribution](../../../../../../exponential-distribution.md) with rate $a_0(x)$. Keep the sample path constant on $[t,t+\Delta t)$, advance $t\leftarrow t+\Delta t$, and choose the reaction by

$$
\boxed{x\leftarrow\begin{cases}
x+3,&U_2<\lambda/a_0(x),\\
x-1,&U_2\ge\lambda/a_0(x).
\end{cases}}
$$

Record the post-jump state, recompute both [reaction propensity functions](../../../../../../reaction-propensity-function.md), and repeat with fresh independent uniforms. At $x=0$ the death propensity is zero, so only a birth is selected and the trajectory remains nonnegative. For a prescribed terminal time $T$, if the next event would occur after $T$, keep the current state to $T$ and stop. This produces exact piecewise constant sample paths of the specified [continuous-time Markov chain](../../../../../../continuous-time-markov-chain.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
