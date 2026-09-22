<h1 id="22h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $x\in X$,

$$
\|Tx\|^2=\sum_{n\in\mathbb Z}|x_{n+1}|^2
=\sum_{n\in\mathbb Z}|x_n|^2=\|x\|^2.
$$

The map $S$ defined by $(Sx)_n=x_{n-1}$ satisfies $ST=TS=I$, so $T$ is a surjective isometry and hence a [unitary operator](../../../../../../unitary-operator.md).

If $Tx=\lambda x$, then

$$
x_{n+1}=\lambda x_n.
$$

For $\lambda\ne0$, this gives $x_n=\lambda^nx_0$ for every integer $n$. When $|\lambda|>1$ the positive tail is not square summable, when $|\lambda|<1$ the negative tail is not square summable, and when $|\lambda|=1$ neither tail is square summable unless $x_0=0$. The case $\lambda=0$ also forces every coordinate to vanish. Thus

$$
\boxed{\sigma_p(T)=\varnothing.}
$$

The reverse triangle inequality gives, for every $x$,

$$
\|(T-\lambda I)x\|
\geq\bigl|\|Tx\|-|\lambda|\|x\|\bigr|
=|1-|\lambda||\,\|x\|.
$$

Hence $T-\lambda I$ is bounded below whenever $|\lambda|\ne1$, so such $\lambda$ do not belong to the [approximate point spectrum](../../../../../../approximate-point-spectrum.md).

Now let $|\lambda|=1$ and define the unit vector

$$
x^{(N)}_n=
\begin{cases}
\lambda^n/\sqrt{N+1},&0\leq n\leq N,\\
0,&\text{otherwise}.
\end{cases}
$$

The equation $x^{(N)}_{n+1}=\lambda x^{(N)}_n$ fails only at the two endpoints, so

$$
\|(T-\lambda I)x^{(N)}\|^2=\frac2{N+1}\longrightarrow0.
$$

Therefore the [bilateral shift operator](../../../../../../bilateral-shift-operator.md) has

$$
\boxed{\sigma_{\mathrm{ap}}(T)=\{\lambda\in\mathbb C:|\lambda|=1\}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [22H](../../22h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
