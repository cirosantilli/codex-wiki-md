<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $w(x)=(\sin x/x)^2$, with $w(0)=1$, and $M=\sup_r|A_r|<\infty$. Since $0\le w\le1$, the finite-prefix bound is $\left|\sum_{r=1}^n A_rw(rk)\right|\le nM$. For $k\ne0$, $w(rk)\le1/(r^2k^2)$ gives [absolute convergence](../../../../../../absolute-convergence.md) of the tail and the correct estimate

$$
\boxed{\left|\sum_{r=n+1}^\infty A_r\left(\frac{\sin rk}{rk}\right)^2\right|\le\frac{2}{nk^2}\sup_{r\ge n+1}|A_r|.}
$$

**The PDF omits the factor $k^{-2}$ from this bound.** Its printed version is false: choose $A_4=1$ and all other $A_r=0$, take $n=3$, and let $k\to0$. The left side tends to one while the printed right side is $2/3$. Thus the intended bound must be qualified as above. At $k=0$, even [absolute convergence](../../../../../../absolute-convergence.md) need not hold for a general sequence tending to zero.

For each fixed $n$, the displayed finite-prefix limit follows immediately: $|k\sum_{r=1}^n A_rw(rk)|\le |k|nM\to0$. The stronger statement needed for part (ii) is

$$
\boxed{k\sum_{r=1}^\infty A_rw(rk)\longrightarrow0\quad(k\to0).}
$$

Here is a proof, so the fixed-prefix formula is not silently substituted for an infinite-series result. Set $N=\lfloor1/|k|\rfloor$ for small nonzero $k$. The multiplied tail is at most $2\sup_{r>N}|A_r|/(N|k|)$, which tends to zero because $N|k|\to1$. For the prefix, choose $J$ with $|A_r|<\eta$ for $r>J$. Then

$$
|k|\sum_{r=1}^{N}|A_r|w(rk)\le |k|\sum_{r=1}^{J}|A_r|+|k|N\eta.
$$

Its upper limit is at most $\eta$, and $\eta$ is arbitrary. This proves [sinc-squared summation of a sequence tending to zero](../../../../../../sinc-squared-summation-of-a-sequence-tending-to-zero.md), including approach from either sign of $k$.

For the unheaded piecewise-affine continuation, [continuity](../../../../../../continuous-function.md) gives $Ac+B=A'c+B'$. Evaluate the asserted symmetric quotient at $t=c$. For sufficiently small positive $h$,

$$
\frac{F(c+h)-2F(c)+F(c-h)}h=A'-A.
$$

Its zero limit forces $\boxed{A=A'}$, and the [continuity](../../../../../../continuous-function.md) relation then forces $\boxed{B=B'}$. Only the condition at the corner is needed; at points away from it such a quotient is automatically zero even for unequal slopes.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
