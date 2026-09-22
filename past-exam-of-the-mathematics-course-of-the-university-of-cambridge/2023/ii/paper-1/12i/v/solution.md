<h1 id="12i/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

First, $\mathbf K\in\Sigma_1$: the partial procedure on input $w$ simulates $f_{w,1}(w)$ and halts exactly when that computation halts.

For hardness, let $A\in\Sigma_1$. Choose a partial computable function $g$ with

$$
w\in A\quad\Longleftrightarrow\quad g(w)\mathbin\downarrow.
$$

For each fixed $w$, define a unary program $P_w$ as follows: on any input $x$, simulate $g(w)$; if that simulation halts, halt and output $x$, and otherwise run forever. The [S-m-n theorem](../../../../../../smn-theorem.md) gives a total computable function $h$ that maps $w$ to a code for $P_w$. Its accepted language is

$$
W_{h(w)}=
\begin{cases}
\mathbb W,&g(w)\mathbin\downarrow,\\
\varnothing,&g(w)\mathbin\uparrow.
\end{cases}
$$

In particular,

$$
w\in A
\quad\Longleftrightarrow\quad
h(w)\in W_{h(w)}
\quad\Longleftrightarrow\quad
h(w)\in\mathbf K.
$$

**Thus $h$ is a [many-one reduction](../../../../../../many-one-reduction.md) $A\leq_m\mathbf K$. Since $A$ was arbitrary, $\mathbf K$ is $\Sigma_1$-hard; together with membership this proves the [many-one completeness of the halting problem](../../../../../../many-one-completeness-of-the-halting-problem.md).**

## ↑ Ancestors (11)

1. [V](../v.md)
2. [12I](../../12i.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
