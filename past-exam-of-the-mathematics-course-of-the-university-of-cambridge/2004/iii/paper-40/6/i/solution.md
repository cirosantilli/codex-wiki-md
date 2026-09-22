<h1 id="6/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The parameter range is $0\leq\theta\leq1$. Omitting data-only constants from the [multinomial distribution](../../../../../../multinomial-distribution.md) [likelihood](../../../../../../likelihood-function.md), its log is

$$
\ell(\theta)=(x_1+x_2)\log(1-\theta)+x_3\log\theta
+x_4\log(7+4\theta)+\mathrm{constant}.
$$

For an interior maximizer, the [likelihood](../../../../../../likelihood-function.md) score must vanish:

$$
-\frac{x_1+x_2}{1-\theta}+\frac{x_3}{\theta}
+\frac{4x_4}{7+4\theta}=0.
$$

Multiply by $\theta(1-\theta)(7+4\theta)$ and collect powers to obtain

$$
\boxed{-4(x_1+x_2+x_3+x_4)\theta^2
+(-7x_1-7x_2-3x_3+4x_4)\theta+7x_3=0.}
$$

The [likelihood](../../../../../../likelihood-function.md) is [concave](../../../../../../concave-function.md): its second [derivative](../../../../../../derivative.md) in the interior is

$$
\ell''(\theta)=-\frac{x_1+x_2}{(1-\theta)^2}
-\frac{x_3}{\theta^2}-\frac{16x_4}{(7+4\theta)^2}<0.
$$

Therefore an admissible interior root is the unique maximum. Endpoints must also be handled if some counts vanish. If $x_3>0$ and $x_1+x_2>0$, both endpoints have zero [likelihood](../../../../../../likelihood-function.md) and the root is interior. If the maximum is at zero then $x_3=0$, and zero also satisfies the displayed polynomial; a maximum at one requires $x_1+x_2=0$, and one likewise satisfies it. Multiplying the score can introduce other endpoint roots, so not every polynomial root is an MLE: evaluate the actual [likelihood](../../../../../../likelihood-function.md) on the feasible candidates.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [6](../../6.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
