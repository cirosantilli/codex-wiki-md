<h1 id="15c/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Now let $z\ne0^n$ and choose one representative $x$ from each pair $\{x,x\mathbin\oplus z\}$. Since $f(x)=f(x\mathbin\oplus z)$ and

$$
(-1)^{(x\mathbin\oplus z)\cdot y}
=(-1)^{x\cdot y}(-1)^{z\cdot y},
$$

the unnormalized second-register amplitude for outcome $y$ is

$$
\sum_{\text{pairs }[x]}(-1)^{x\cdot y}
\bigl(1+(-1)^{z\cdot y}\bigr)|f(x)\rangle.
$$

If $y\cdot z=1$, every paired contribution cancels, so the probability is zero. If $y\cdot z=0$, every coefficient has magnitude two. The $2^{n-1}$ distinct pair values give orthogonal states, so the squared norm before the overall $2^{-n}$ factor is $4\cdot2^{n-1}=2^{n+1}$. The probability is therefore

$$
2^{-2n}2^{n+1}=2^{-(n-1)}.
$$

**Thus one run samples uniformly from the $2^{n-1}$ strings in the [orthogonal complement over the binary field](../../../../../../../orthogonal-complement-over-the-binary-field.md) $\{y:y\cdot z=0\}$, which is the sampling step in [Simon's algorithm](../../../../../../../simon-s-algorithm.md).**

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [15C](../../../15c.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
