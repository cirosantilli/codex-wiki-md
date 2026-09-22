<h1 id="20h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Because $p\equiv11\pmod{12}$, we have $p\equiv3\pmod4$ and

$$
\mathcal O_K=\mathbb Z\left[\frac{1+\sqrt{-p}}2\right].
$$

For $\theta=(1+\sqrt{-p})/2$, the [minimal polynomial](../../../../../../minimal-polynomial.md) is

$$
f(T)=T^2-T+\frac{p+1}{4}.
$$

Since $p\equiv2\pmod3$, reduction modulo $3$ gives $f(T)\equiv T(T-1)$. Its two roots are distinct, so

$$
(3)=\mathfrak p_1\mathfrak p_2
$$

with distinct prime ideals of norm $3$. Thus $3$ splits completely, as recorded in [splitting of three in Q of square root minus p](../../../../../../splitting-of-three-in-q-of-square-root-minus-p.md).

The [ideal class group](../../../../../../ideal-class-group.md) $\operatorname{Cl}_K$ is the group of nonzero fractional ideals of $\mathcal O_K$ modulo the subgroup of principal fractional ideals. Saying that $\mathfrak p_1$ has order $n$ means that $n$ is the least positive integer for which $\mathfrak p_1^n$ is principal.

Suppose for contradiction that $n$ is odd and $\mathfrak p_1$ has order $n$. Then $\mathfrak p_1^n=(\alpha)$ for some $\alpha\in\mathcal O_K$, and taking [norms](../../../../../../ideal-norm.md) gives

$$
|N_{K/\mathbb Q}(\alpha)|=N(\mathfrak p_1)^n=3^n.
$$

Write $\alpha=(a+b\sqrt{-p})/2$, where $a,b\in\mathbb Z$ have the same parity. Then

$$
4\cdot3^n=a^2+pb^2.
$$

If $b\ne0$, the right-hand side is at least $p$, contradicting $p>3^{n+2}>4\cdot3^n$. Hence $b=0$, so $\alpha$ is a rational algebraic integer and therefore an integer. But then $3^n=N(\alpha)=\alpha^2$, impossible when $n$ is odd. This proves the [odd-order obstruction for a split prime in an imaginary quadratic field](../../../../../../odd-order-obstruction-for-a-split-prime-in-an-imaginary-quadratic-field.md) and shows that the order cannot equal $n$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [20H](../../20h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
