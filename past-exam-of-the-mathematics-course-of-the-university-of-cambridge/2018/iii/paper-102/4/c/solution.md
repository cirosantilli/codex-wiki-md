<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In the defining representation of the [symplectic Lie algebra](../../../../../../symplectic-lie-algebra.md) $\mathfrak{sp}_4$, the weights are $\varepsilon_1,\varepsilon_2,-\varepsilon_1,-\varepsilon_2$. Their [highest weight](../../../../../../highest-weight-of-a-representation.md), for the [root basis](../../../../../../fundamental-system-of-a-root-system.md) of part (b), is therefore

$$
\boxed{\operatorname{highest\ weight}(V)=\varepsilon_1=\omega_1.}
$$

The flip on the [tensor square](../../../../../../tensor-square.md) commutes with the action of $\mathfrak{sp}_4$, giving $V\otimes V=\operatorname{Sym}^2V\oplus\Lambda^2V$ with dimensions $10$ and $6$.

If $v_1$ is a [highest-weight vector](../../../../../../highest-weight-vector.md) of weight $\varepsilon_1$, then $v_1\otimes v_1$ is a [highest-weight vector](../../../../../../highest-weight-vector.md) of weight $2\omega_1$ in the [symmetric square](../../../../../../symmetric-square.md). By [Weyl complete reducibility theorem](../../../../../../weyl-complete-reducibility-theorem.md), this ensures an irreducible summand $V(2\omega_1)$ occurs. Its dimension is $10$ by part (b), exhausting the [symmetric square](../../../../../../symmetric-square.md).

Let $\omega$ denote the preserved [symplectic form](../../../../../../symplectic-form.md). The [symplectic contraction of an exterior square](../../../../../../symplectic-contraction-of-an-exterior-square.md) is the nonzero equivariant map

$$
c:\Lambda^2V\longrightarrow\mathbb C,\qquad c(v\wedge w)=\omega(v,w),
$$

where the target is a [trivial Lie algebra representation](../../../../../../trivial-lie-algebra-representation.md). Thus its [kernel](../../../../../../kernel-of-a-linear-map.md) has dimension $5$. Choose a weight vector $v_2$ of weight $\varepsilon_2$ in a [symplectic basis](../../../../../../symplectic-basis.md), with $\omega(v_1,v_2)=0$. The vector $v_1\wedge v_2$ belongs to this [kernel](../../../../../../kernel-of-a-linear-map.md) and has weight $\varepsilon_1+\varepsilon_2=\omega_2$. It is a [highest-weight vector](../../../../../../highest-weight-vector.md): none of $\omega_2+\alpha$, for $\alpha\in\Phi^+$, is a weight of $\Lambda^2V$, whose weights are $\pm\varepsilon_1\pm\varepsilon_2$ and zero. Hence the [kernel](../../../../../../kernel-of-a-linear-map.md) contains $V(\omega_2)$; its dimension $5$ exhausts the [kernel](../../../../../../kernel-of-a-linear-map.md). [Weyl complete reducibility theorem](../../../../../../weyl-complete-reducibility-theorem.md) supplies a complementary invariant line $V(0)$.

The resulting [tensor-square decomposition of the defining sp4 representation](../../../../../../tensor-square-decomposition-of-the-defining-sp4-representation.md) is

$$
\boxed{V\otimes V\cong V(2\omega_1)\oplus V(\omega_2)\oplus V(0),\qquad16=10+5+1.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 102](../../../paper-102-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
