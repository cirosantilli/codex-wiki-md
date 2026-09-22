<h1 id="1/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $(v_n)$ be a minimizing sequence. The coercive lower bound from part 2 makes it bounded in the [harmonic-oscillator energy space](../../../../../../harmonic-oscillator-energy-space.md) and in $L^4$. After taking a subsequence, $v_n$ converges weakly in both spaces. The [compact embedding of the harmonic-oscillator energy space](../../../../../../compact-embedding-of-the-harmonic-oscillator-energy-space.md) gives strong convergence in $L^2$, while weak lower semicontinuity of the gradient, moment, and $L^4$ terms yields

$$
J(v)\leq\liminf_{n\to\infty}J(v_n).
$$

Thus $v$ attains the infimum. Replacing $v$ by $|v|$ does not increase the gradient norm, so a minimizer may be chosen nonnegative. It is nonzero because the infimum is negative whereas $J(0)=0$.

Taking the first variation against a smooth compactly supported function gives the [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md)

$$
-\Delta v+|x|^2v-\omega v+v^3=0,
$$

which is the [Schrödinger trapped defocusing stationary equation](../../../../../../schrodinger-trapped-defocusing-stationary-equation.md).

## ↑ Ancestors (11)

1. [4](../4.md)
2. [1](../../1.md)
3. [Paper 154](../../../paper-154-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
