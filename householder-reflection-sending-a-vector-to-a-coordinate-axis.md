# Householder reflection sending a vector to a coordinate axis

↑ **Parent:** [Householder transformation](householder-transformation.md)

For a nonzero real [vector](vector.md) $x\in\mathbb R^n$, choose $\alpha$ with $|\alpha|=\|x\|_2$ and put $v=x-\alpha e_1$. When $v\ne0$, the [Householder reflection](householder-transformation.md)

$$
H=I-\frac{2vv^T}{v^Tv}
$$

satisfies $Hx=\alpha e_1$: every component except the first becomes zero. Here $e_1$ is the first [Cartesian basis](cartesian-basis.md) [vector](vector.md). The calculation is short:

$$
v^Tv=2(\|x\|_2^2-\alpha x_1),
\qquad
v^Tx=\|x\|_2^2-\alpha x_1,
\qquad
Hx=x-v=\alpha e_1.
$$

If $v=0$, the [vector](vector.md) is already at the selected target, so the [identity matrix](identity-matrix.md) suffices.

In [floating-point arithmetic](floating-point-arithmetic-split.md), a customary choice is

$$
\alpha=
\begin{cases}
-\|x\|_2,&x_1\ge0,\\
\|x\|_2,&x_1<0.
\end{cases}
$$

Then $|v_1|=|x_1|+\|x\|_2$, avoiding subtraction of nearly equal positive quantities in the first component. Either sign can be valid in exact arithmetic; the numerical choice protects the construction from [catastrophic cancellation](catastrophic-cancellation.md). [Olver, Orthogonal Bases and the QR Algorithm: Householder factorization and sign selection](https://math.mit.edu/classes/18.085/summer2016/handouts/qr.pdf)

For $x=(3,4)^T$, this choice gives $\alpha=-5$ and $v=(8,4)^T$. Dividing $v$ by its [Euclidean norm](euclidean-norm.md) gives $u=(2,1)^T/\sqrt5$, exactly the normal in the geometric example.

## ↑ Ancestors (6)

1. [Householder transformation](householder-transformation.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
