<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $x=u/v\in\mathbb Q$ in lowest terms, the [naive height on the projective line](../../../../../../naive-height-on-the-projective-line.md) is

$$
H(x)=\max\{|u|,|v|\}.
$$

Homogenize the coprime numerator and denominator of $\xi$ to degree $d$. The triangle inequality gives the upper estimate $H(\xi(x))\leq c_2H(x)^d$. Since the two homogenized forms have no common projective zero, their [resultant](../../../../../../resultant.md) is nonzero, and the Bézout identities for the resultant express fixed multiples of $u^{2d-1}$ and $v^{2d-1}$ as combinations of their values with coefficients of degree $d-1$. After cancellation this gives $H(x)^d\leq C H(\xi(x))$, which is the lower estimate with $c_1=C^{-1}$.

Now write $x=u/v$ in lowest terms and put

$$
N=u^3+auv^2+bv^3.
$$

Since $\gcd(N,v)=1$, the equation $y^2=N/v^3$ gives

$$
H(y)^2=\max\{|N|,|v|^3\}=:M.
$$

Clearly $M\leq\gamma H(x)^3$ for $\gamma=1+|a|+|b|$. Homogenizing the supplied polynomial identity gives

$$
u^5=(u^2-av^2)N-(bu^2-a^2uv-abv^2)v^3.
$$

Its coefficient sum is at most $\gamma^2$, so $|u|^5\leq\gamma^2H(x)^2M$. The same lower bound is immediate from $|v|^3\leq M$ when $|v|=H(x)$. Thus

$$
\boxed{\gamma^{-2}H(x)^3\leq H(y)^2\leq\gamma H(x)^3.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
