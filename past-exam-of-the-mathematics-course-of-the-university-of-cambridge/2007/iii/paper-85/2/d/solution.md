<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Assume the $g$ cycle has least period $n$ and nonzero [periodic-orbit multiplier](../../../../../../multiplier-of-a-periodic-orbit-of-an-iteration.md) $P=(g^n)'(\hat x)$. It then avoids zero. Combining the iterate identity with the [periodic-orbit multiplier](../../../../../../multiplier-of-a-periodic-orbit-of-an-iteration.md)-sign formula gives

$$
f_L^n(\hat x)=\operatorname{sgn}(P)\hat x.
$$

Thus $P>0$ makes $\hat x$ return after $n$ iterates, whereas $P<0$ gives $f_L^n(\hat x)=-\hat x$. In the latter case oddness on the noncritical orbit implies

$$
f_L^{2n}(\hat x)=f_L^n(-\hat x)=-f_L^n(\hat x)=\hat x.
$$

To prove the least periods, note that a $g$ cycle cannot contain two distinct points $x$ and $-x$: evenness would give them the same image, but $g$ permutes its distinct cycle points bijectively. Therefore the $n$ absolute values in the cycle are distinct. Since $|f_L^k(\hat x)|=|g^k(\hat x)|$, any return under $f_L$ must occur at a multiple of $n$. For $P<0$ the first such return fails because $\hat x\ne0$, so $2n$ is minimal. Hence the [period transfer from a quadratic map to its Lorenz sign lift](../../../../../../period-transfer-from-a-quadratic-map-to-its-lorenz-sign-lift.md) is

$$
\boxed{P>0:\text{ least period }n;\qquad P<0:\text{ least period }2n.}
$$

There are two symmetry-related $f_L$ cycles in the positive case and one cycle containing both signs in the negative case. Away from zero $f_L'(x)=2|x|$, so their [periodic-orbit multipliers](../../../../../../multiplier-of-a-periodic-orbit-of-an-iteration.md) are $|P|$ and $|P|^2$, respectively. A stable $g$ cycle therefore gives stable lifted cycles in both cases.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 85](../../../paper-85-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
