<h1 id="5/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $A$ be a register with [orthonormal basis](../../../../../../../orthonormal-basis.md) $\{|x\rangle\}$ for Alice's classical symbol, $Q$ the transmitted system, and $B$ a register initially in a fixed blank state. The initial [classical-quantum state](../../../../../../../classical-quantum-state.md) is

$$
\boxed{\rho_{AQB}=\sum_xp(x)|x\rangle\langle x|_A\otimes\rho_x\otimes|0\rangle\langle0|_B.}
$$

A [POVM](../../../../../../../positive-operator-valued-measure.md) fixes probabilities but not a unique conditional state of $Q$. Choose the [Lüders rule](../../../../../../../luders-rule.md) instrument $M_y=\sqrt{E_y}$, which satisfies $\sum_yM_y^\dagger M_y=I$. Record outcome $y$ in orthogonal states of $B'$ and retain the corresponding quantum output $Q'$. The final nonselective state is

$$
\boxed{\rho_{A'Q'B'}=\sum_{x,y}p(x)|x\rangle\langle x|_{A'}\otimes M_y\rho_xM_y^\dagger\otimes|y\rangle\langle y|_{B'}.}
$$

The positive operators in this sum are unnormalized: their traces already include the outcome probabilities. If $\operatorname{Tr}(E_y\rho_x)>0$, the normalized conditional state of $Q'$ is $M_y\rho_xM_y^\dagger/\operatorname{Tr}(E_y\rho_x)$.

More generally, an instrument may use operators $M_{y\mu}$ with $\sum_\mu M_{y\mu}^\dagger M_{y\mu}=E_y$, replacing $M_y\rho_xM_y^\dagger$ by $\sum_\mu M_{y\mu}\rho_xM_{y\mu}^\dagger$. All subsequent classical information bounds are unchanged. This explicitly accounts for the fact that a [POVM does not determine the post-measurement state](../../../../../../../povm-does-not-determine-the-post-measurement-state.md) of a retained quantum system.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 33](../../../../paper-33-split.md)
5. [Iii](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
