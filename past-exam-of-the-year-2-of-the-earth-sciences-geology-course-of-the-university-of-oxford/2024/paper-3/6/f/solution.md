<h1 id="6/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Choose a fixed time increment $h=\Delta t>0$, let $t_n=nh$, and approximate $\mathbf c(t_n)$ by $\mathbf c_n$. The [Backward Euler method](../../../../../backward-euler-method.md) evaluates the transport term at the new time:

$$
\frac{\mathbf c_{n+1}-\mathbf c_n}{h}=A\mathbf c_{n+1}-\mathbf b.
$$

Rearrange to the [linear system](../../../../../system-of-linear-equations.md)

$$
\boxed{B\mathbf c_{n+1}=\mathbf c_n-h\mathbf b,\qquad
B=I-hA=\begin{pmatrix}
1+2h&-h&0&-h\\
-2h&1+2h&0&0\\
0&-h&1+2h&-h\\
0&0&-2h&1+2h
\end{pmatrix}.}
$$

Although $A$ is a [singular matrix](../../../../../singular-matrix.md), $B$ is an [invertible matrix](../../../../../invertible-matrix.md) for every $h>0$. In each row, its diagonal entry is $1+2h$ and the sum of the [absolute values](../../../../../absolute-value.md) of its off-diagonal entries is $2h$; hence it is a [strictly diagonally dominant matrix](../../../../../strictly-diagonally-dominant-matrix.md). Its [Gershgorin discs](../../../../../gershgorin-disc.md) have centre $1+2h$ and radius $2h$, excluding zero. In particular, the zero [eigenvalue](../../../../../eigenvalue.md) of $A$ becomes an [eigenvalue](../../../../../eigenvalue.md) $1$ of $B$.

The algorithm uses [Reusing LU factors for multiple right-hand sides](../../../../../reusing-lu-factors-for-multiple-right-hand-sides.md):

- Form $B$ once. Compute a [Pivoted LU decomposition](../../../../../pivoted-lu-decomposition.md) $PB=L_B U_B$, storing the [permutation matrix](../../../../../permutation-matrix.md) $P$, the unit [lower triangular matrix](../../../../../lower-triangular-matrix.md) $L_B$, and the [upper triangular matrix](../../../../../upper-triangular-matrix.md) $U_B$.
- Set $\mathbf c_0=\mathbf c(0)$.
- At each step form $r_n=\mathbf c_n-h\mathbf b$. Solve $L_B y=Pr_n$ by [forward substitution](../../../../../forward-substitution.md), then solve $U_B\mathbf c_{n+1}=y$ by [back substitution](../../../../../back-substitution.md).
- Advance $n$ and repeat until the desired final time. Choose the fixed increment so the final time is an integer multiple of $h$, or refactor $B$ if a shorter final step is used.

Both triangular solves use the factors of **$I-hA$**. The [LU factorization](../../../../../lu-decomposition.md) of the singular transport [matrix](../../../../../matrix.md) $A$ from part (a) is not a solver for this new [linear system](../../../../../system-of-linear-equations.md). No [matrix inverse](../../../../../matrix-inverse-split.md) needs to be formed. Since $A$ and $h$ are fixed, the same [LU factorization](../../../../../lu-decomposition.md) serves every step; only the right-hand side changes. A varying $\mathbf b(t)$ would give $r_n=\mathbf c_n-h\mathbf b(t_{n+1})$ without changing these factors.

As a check, multiplying the update by $\mathbf1^T$ gives

$$
\mathbf1^T\mathbf c_{n+1}=\mathbf1^T\mathbf c_n-h\mathbf1^T\mathbf b,
$$

exactly reproducing the inventory balance at the sampled times, apart from [roundoff error](../../../../../round-off-error.md). The [Backward Euler method](../../../../../backward-euler-method.md) has temporal [global error](../../../../../global-discretization-error.md) $O(h)$ for smooth solutions, so its [A-stability](../../../../../a-stability.md) does not remove the need to select $h$ for accuracy.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [6](../../6.md)
3. [Paper 3](../../../paper-3-split.md)
4. [2024](../../../split.md)
5. [Past exam of the year 2 of the earth sciences (geology) course of the University of Oxford](../../../../split.md)
6. [Year 2 of the earth sciences (geology) course of the University of Oxford](../../../../../year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford.md)
7. [Earth sciences (geology) course of the University of Oxford](../../../../../earth-sciences-geology-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
