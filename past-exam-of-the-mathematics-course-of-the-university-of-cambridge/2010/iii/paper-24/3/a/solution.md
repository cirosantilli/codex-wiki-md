<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [strong form of Hensel lemma](../../../../../../strong-form-of-hensel-lemma.md): for $f\in\mathbb Z_p[T]$ and $a\in\mathbb Z_p$, if

$$
v_p(f(a))>2v_p(f'(a)),
$$

there is a unique [polynomial root](../../../../../../root-of-a-polynomial.md) $b$ in the ball $v_p(b-a)>v_p(f'(a))$. In particular, a simple [polynomial root](../../../../../../root-of-a-polynomial.md) modulo $p$ lifts uniquely in its residue class. Newton iteration gives $v_p(b-a)=v_p(f(a))-v_p(f'(a))$ when $f(a)\ne0$.

For odd $p\notin\{5,7,13\}$, the sets

$$
\{5x^2:x\in\mathbb F_p\},
\qquad
\{-13-7y^2:y\in\mathbb F_p\}
$$

each have $(p+1)/2$ elements, so they intersect. This gives a zero modulo $p$ with $z=1$. The derivative with respect to $z$ is $26$, nonzero modulo $p$, so [Hensel's lemma](../../../../../../hensel-s-lemma.md) lifts $z$ while holding $x,y$ fixed. This is the elementary proof of [isotropy of nondegenerate ternary quadratic forms over finite fields](../../../../../../isotropy-of-nondegenerate-ternary-quadratic-forms-over-finite-fields.md) followed by a simple-root lift.

At $p=5$, the residue vector $(0,1,1)$ is a zero, and the derivative $14y$ is nonzero. At $p=13$, use $(3,1,0)$, for which the value is 52 and the derivative $10x=30$ is nonzero modulo 13. Again a single-variable Hensel lift suffices.

At $p=2$, hold $x=2,z=1$ and use $f(Y)=7Y^2+33$. At $Y=1$, $f(1)=40$ has [valuation](../../../../../../valuation.md) 3, while $f'(1)=14$ has [valuation](../../../../../../valuation.md) 1. Since $3>2$, the strong Hensel inequality gives a [polynomial root](../../../../../../root-of-a-polynomial.md) $y\in\mathbb Z_2$, indeed $y\equiv1\pmod4$. This yields a nonzero solution.

At $p=7$, suppose a nonzero solution exists and scale it so that all coordinates are in $\mathbb Z_7$ and at least one is a [unit](../../../../../../unit-in-a-ring.md). Reduction modulo 7 gives $z^2=5x^2$. Since 5 is not a square modulo 7, both $x,z$ are divisible by 7. In the original equation their terms are then divisible by 49, so $7y^2$ is divisible by 49 as well, forcing $y$ divisible by 7. This contradicts the normalization. Thus [local isotropy of the five seven thirteen form](../../../../../../local-isotropy-of-the-five-seven-thirteen-form.md) gives

$$
\boxed{\text{The unique obstructing prime is }p=7.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
