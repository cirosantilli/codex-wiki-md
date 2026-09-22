<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the preliminary definitions, a block is $Re$ for a primitive central [idempotent](../../../../../../idempotent.md) $e$, and a [module](../../../../../../module-mathematics.md) belongs to it when $eM=M$. For a [semisimple algebra](../../../../../../semisimple-algebra.md), the [Artin–Wedderburn theorem](../../../../../../artin-wedderburn-theorem.md) identifies its blocks with the factors $M_{n_i}(D_i)$ in its product decomposition. Each factor is a [block of a finite-dimensional algebra](../../../../../../block-of-a-finite-dimensional-algebra.md).

We prove [Ext separation of finite-length modules](../../../../../../ext-separation-of-finite-length-modules.md). The extension hypothesis is $\operatorname{Ext}^1(S,T)=\operatorname{Ext}^1(T,S)=0$ for simples in opposite sets. First, for a simple $S\in\mathcal C_1$ and a module $N$ of finite [composition length](../../../../../../composition-length.md) with factors in $\mathcal C_2$, we have $\operatorname{Ext}^1(S,N)=0$. Induct on the length of $N$: for $0\to N'\to N\to T\to0$ with $T$ simple, the long exact sequence of the [Ext functor](../../../../../../ext-functor.md) contains

$$
\operatorname{Ext}^1(S,N')\longrightarrow\operatorname{Ext}^1(S,N)\longrightarrow\operatorname{Ext}^1(S,T),
$$

whose outer groups are zero. The same argument works with the two sets interchanged.

Now induct on the length of $M$, with $M=0$ immediate. Take a simple quotient in $0\to N\to M\to S\to0$. By induction, $N=N_1\oplus N_2$ with factors in the respective sets. Suppose $S\in\mathcal C_1$; the other case is symmetric. Quotienting by $N_1$ gives

$$
0\longrightarrow N_2\longrightarrow M/N_1\longrightarrow S\longrightarrow0.
$$

This splits by the preceding Ext vanishing. Let $U_1$ be the inverse image in $M$ of the chosen complementary copy of $S$. Then $U_1\cap N_2=0$, $U_1+N_2=M$, and $0\to N_1\to U_1\to S\to0$. Thus $U_1$ has only factors in $\mathcal C_1$, while $U_2=N_2$ has only factors in $\mathcal C_2$.

If two finite-length modules have factors in disjoint sets, any homomorphism between them is zero: a nonzero image would, by the [Jordan–Hölder theorem](../../../../../../jordan-holder-theorem.md), have a simple factor belonging to both sets. For any [submodule](../../../../../../submodule.md) $V$ of $M$ with factors in $\mathcal C_1$, projection onto $U_2$ is consequently zero, so $V\subset U_1$. The analogous argument applies to $U_2$. Hence

$$
\boxed{M=U_1\oplus U_2,\quad U_i\text{ is the unique largest submodule with factors in }\mathcal C_i}.
$$

In particular both summands are preserved by every endomorphism of $M$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 138](../../../paper-138-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
