<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use ordinary integer surgery coefficients, so the positive trace has [intersection form](../../../../../../intersection-form.md) $(n)$. Let $\widehat F_0\subset K_0$ be the capped [Seifert surface](../../../../../../seifert-surface.md). Label the [Spin-c structures](../../../../../../spin-c-structure.md) by

$$
\langle c_1(\mathfrak s_i),[\widehat F_0]\rangle=2i,\qquad i\in\mathbb Z.
$$

On the trace $X_n:S^3\to K_n$, let $\widehat F_n^2=n$ and label its structures $\mathfrak r_j$ by $\langle c_1(\mathfrak r_j),[\widehat F_n]\rangle=2j-n$. Restriction identifies $\mathfrak t_k$ with $j\equiv k\pmod n$. In these compatible labels the [Integer-surgery exact triangle in Heegaard Floer homology](../../../../../../integer-surgery-exact-triangle-in-heegaard-floer-homology.md) is

$$
\boxed{\cdots\longrightarrow\mathbf{HF}^-(S^3)\xrightarrow{A_k}\bigoplus_{i\equiv k\ (\mathrm{mod}\ n)}\mathbf{HF}^-(K_0,\mathfrak s_i)\xrightarrow{B_k}\mathbf{HF}^-(K_n,\mathfrak t_k)\xrightarrow{C_k}\mathbf{HF}^-(S^3)\longrightarrow\cdots.}
$$

Here boldface denotes the [U-adic completion of Heegaard Floer homology](../../../../../../u-adic-completion-of-heegaard-floer-homology.md). Only finitely many zero-surgery structures contribute, by the [genus](../../../../../../genus-of-a-surface.md) bound on a capped [Seifert surface](../../../../../../seifert-surface.md), so the middle direct sum causes no difficulty. The infinite sums of trace maps do require completion. The printed minus notation should be understood in this completed sense; with the polynomial version, a sum over every extension need not even have values in $\mathbb Z[U]$. The plus version has the same ordering and needs no completion.

The two ordinary surgery traces give $A_k$ and $C_k$. For $X_0:S^3\to K_0$, $H^2(X_0)=\mathbb Z$, and its [Spin-c structures](../../../../../../spin-c-structure.md) $\mathfrak q_i$ have determinant evaluations $2i$ on the capped [Seifert surface](../../../../../../seifert-surface.md). Their restrictions are the unique structure on $S^3$ and $\mathfrak s_i$ on $K_0$. Thus the component of $A_k$ in the $i$th summand is $F^-_{X_0,\mathfrak q_i}$ for $i\equiv k$. For the orientation-reversed and turned-around trace $V_n:K_n\to S^3$, $H^2(V_n)=\mathbb Z$ and $\widehat F_n^2=-n$. Its structures $\mathfrak r_j$ still have characteristic evaluations $2j-n$, restrict to $\mathfrak t_{j\bmod n}$ on $K_n$ and to the unique structure on $S^3$, and

$$
C_k=\sum_{j\equiv k\ (\mathrm{mod}\ n)}F^-_{V_n,\mathfrak r_j}.
$$

Characteristic parity explains the allowed evaluations; changing a structure by the generator of $H^2$ changes its evaluation by two, and the boundary restriction reduces the label modulo $n$.

For $n>1$, $B_k$ has an auxiliary lens-space input. More precisely, take the three-boundary surgery [cobordism](../../../../../../cobordism.md), or equivalently a two-ended [cobordism](../../../../../../cobordism.md) $Z_n:K_0\#L_n\to K_n$, where $L_n$ is positive $n$-surgery on the unknot. Its incoming lens-space factor is fixed to the distinguished structure $\mathfrak u_0$ and its canonical top Floer generator $\Theta_{L_n}$. Then

$$
B_k(\xi)=\sum_{\substack{\mathfrak v|_{K_0}=\mathfrak s_i, i\equiv k\\\mathfrak v|_{L_n}=\mathfrak u_0, \mathfrak v|_{K_n}=\mathfrak t_k}}F^-_{Z_n,\mathfrak v}(\xi\otimes\Theta_{L_n}).
$$

This describes the boundary restrictions exactly, including the boundary that must not be suppressed. A concrete [Kirby diagram](../../../../../../kirby-diagram.md) for $Z_n$ starts with the split incoming surgeries of coefficients $0$ and $n$, then attaches a zero-framed circle linking each incoming component once. Its full linking matrix is $\left(\begin{smallmatrix}0&0&1\\0&n&1\\1&1&0\end{smallmatrix}\right)$. Quotienting [cohomology](../../../../../../cohomology-split.md) by the two incoming surgery columns gives $H^2(Z_n)=\mathbb Z\oplus\mathbb Z/n$. Accordingly its [Spin-c structures](../../../../../../spin-c-structure.md) may be labeled $(i,q)$ with incoming restrictions $(\mathfrak s_i,\mathfrak u_q)$ and outgoing restriction $\mathfrak t_{i-q}$. In particular, fixing $q=0$ gives exactly one extension for each $i$, and its outgoing class is $i\bmod n$. Thus $B_k$ is a [Heegaard Floer cobordism map](../../../../../../heegaard-floer-cobordism-map.md) with the fixed auxiliary generator, rather than an unqualified map of a trace from $K_0$ to $K_n$. When $n=1$, $L_n=S^3$ and all three arrows become the familiar sums of ordinary two-ended [Heegaard Floer cobordism maps](../../../../../../heegaard-floer-cobordism-map.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
