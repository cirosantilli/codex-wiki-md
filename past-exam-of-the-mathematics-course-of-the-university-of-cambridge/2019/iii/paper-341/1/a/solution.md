<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Expand about $t=t_{n+2}$ and use $y''=f'(y)f(y)$ from the [chain rule](../../../../../../chain-rule.md). The residual of the exact solution is

$$
\begin{aligned}
&y(t)-\frac87y(t-h)+\frac17y(t-2h)-\frac67hy'(t)+\frac27h^2y''(t)\\
&\qquad=\frac1{21}h^4y^{(4)}(t)+O(h^5).
\end{aligned}
$$

The coefficients through $h^3$ vanish, and the displayed fourth-order coefficient does not. Thus the [multiderivative multistep method](../../../../../../multiderivative-multistep-method.md) has **order three**.

At $h=0$, its first characteristic polynomial is

$$
\rho(\xi)=\xi^2-\frac87\xi+\frac17=(\xi-1)(\xi-1/7).
$$

Its roots are $1$ and $1/7$, with the unit-modulus root simple, so it satisfies the [root condition for a multistep method](../../../../../../root-condition-for-a-multistep-method.md) and is [zero-stable](../../../../../../zero-stability.md). Combining this with the defect estimate proves **convergence of order three**, assuming sufficiently smooth $f$, order-three starting values, and the nearby branch of each implicit update.

More explicitly, the right-hand side is $hF_h(y_{n+2})$, where $F_h=6f/7-2hf'f/7$ has a uniform local [Lipschitz continuity](../../../../../../lipschitz-continuity.md) bound for small $h$. A bounded zero-stable impulse response and the [discrete Gronwall inequality](../../../../../../discrete-gronwall-inequality.md) therefore control the accumulated $O(h^4)$ defects by $O(h^3)$ over fixed time intervals. This is [convergence of a zero-stable multiderivative method](../../../../../../convergence-of-a-zero-stable-multiderivative-method.md), rather than a direct application of the first-derivative-only [Dahlquist equivalence theorem](../../../../../../dahlquist-equivalence-theorem.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
