<h1 id="12i/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

Membership is immediate from the supplied characterization of $\Pi_2$. Define the partial computable function

$$
F(v,x)=f_{v,1}(x).
$$

Then

$$
v\in\mathbf{Tot}
\quad\Longleftrightarrow\quad
W_v=\mathbb W
\quad\Longleftrightarrow\quad
(\forall x\in\mathbb W)\ F(v,x)\mathbin\downarrow,
$$

so $\mathbf{Tot}\in\Pi_2$.

Now let $P\in\Pi_2$. There is a partial computable $f$ such that

$$
w\in P
\quad\Longleftrightarrow\quad
(\forall x\in\mathbb W)\ f(w,x)\mathbin\downarrow.
$$

For each $w$, define a unary partial function

$$
g_w(x)=
\begin{cases}
x,&f(w,x)\mathbin\downarrow,\\
\text{undefined},&f(w,x)\mathbin\uparrow.
\end{cases}
$$

Operationally, its program simulates $f(w,x)$ and returns $x$ if that computation halts. By the [S-m-n theorem](../../../../../../smn-theorem.md), a total computable map $h$ produces an index $h(w)$ for $g_w$. Therefore

$$
\begin{aligned}
w\in P
&\Longleftrightarrow
(\forall x)\ g_w(x)\mathbin\downarrow\\
&\Longleftrightarrow W_{h(w)}=\mathbb W
\Longleftrightarrow h(w)\in\mathbf{Tot}.
\end{aligned}
$$

**Thus every [Pi-2 set](../../../../../../pi-2-set.md) many-one reduces to $\mathbf{Tot}$. Combined with membership, this proves that the [totality problem](../../../../../../totality-problem.md) is $\Pi_2$-complete.**

## ↑ Ancestors (11)

1. [Vi](../vi.md)
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
