<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix the [quantum enveloping algebra of sl2](../../../../../../quantum-enveloping-algebra-of-sl2.md) convention

$$
KEK^{-1}=q^2E,\qquad KFK^{-1}=q^{-2}F,\qquad
EF-FE=\frac{K-K^{-1}}{q-q^{-1}},\qquad
[j]=\frac{q^j-q^{-j}}{q-q^{-1}}.
$$

The printed pair of matrices contains an error. On its first [basis](../../../../../../basis.md) vector, the printed matrices give $(EF-FE)v_0=\epsilon[2]^2v_0$, whereas the defining commutator gives $\epsilon[2]v_0$. Since $q$ is not a [root of unity](../../../../../../root-of-unity.md), $[2]\ne0,1$: $[2]=0$ would give $q^2=-1$, and $[2]=1$ would give $q^2-q+1=0$. Thus **the two printed matrices cannot represent this algebra**. Keeping the printed $F$ matrix requires exchanging the two nonzero entries of the printed $E$ matrix. We derive that corrected pair rather than assume a classification theorem.

As $q$ is not a [root of unity](../../../../../../root-of-unity.md), successive applications of $E$ multiply $K$ [eigenvalues](../../../../../../eigenvalue.md) by $q^2$. Finiteness of the [spectrum](../../../../../../spectrum-functional-analysis.md) therefore makes $E$ a [nilpotent operator](../../../../../../nilpotent-linear-map.md). Start from a $K$ [eigenvector](../../../../../../eigenvector.md) and apply $E$ until the last nonzero vector $v$; then $Ev=0$ and $Kv=\lambda v$, with $\lambda\ne0$. The defining commutator gives the [highest-weight string for quantum sl2](../../../../../../highest-weight-string-for-quantum-sl2.md)

$$
EF^jv=[j]\frac{\lambda q^{1-j}-\lambda^{-1}q^{j-1}}{q-q^{-1}}F^{j-1}v.
$$

For completeness, at $j=1$ this is the commutator applied to $v$. To advance from $j$ to $j+1$, write $EF^{j+1}v=F(EF^jv)+(K-K^{-1})F^jv/(q-q^{-1})$, use $KF^jv=\lambda q^{-2j}F^jv$, and combine the two coefficients; their sum is the displayed coefficient at $j+1$.

Let $N$ be the first index with $F^Nv=0$. Such an index exists because nonzero $F^jv$ have distinct $K$ [eigenvalues](../../../../../../eigenvalue.md) $\lambda q^{-2j}$. The [linear span](../../../../../../linear-span.md) of $v,Fv,\ldots,F^{N-1}v$ is stable under $K,E,F$, so simplicity makes it all of $V$. The distinct [eigenvalues](../../../../../../eigenvalue.md) make these vectors independent; hence $N=3$. Applying the string formula to $F^3v=0$ gives

$$
0=[3]\frac{\lambda q^{-2}-\lambda^{-1}q^2}{q-q^{-1}}F^2v.
$$

As $[3]\ne0$ and $F^2v\ne0$, $\lambda^2=q^4$, so $\lambda=\epsilon q^2$ with $\epsilon=\pm1$.

Choose the [basis](../../../../../../basis.md) $v_0=v$, $v_1=Fv/[2]$, $v_2=F^2v/[2]$. Then $Fv_0=[2]v_1$, $Fv_1=v_2$, $Ev_1=\epsilon v_0$ and $Ev_2=\epsilon[2]v_1$. The correct matrices in this [basis](../../../../../../basis.md) are

$$
\boxed{E=\epsilon\begin{pmatrix}0&1&0\\0&0&[2]\\0&0&0\end{pmatrix},\quad
F=\begin{pmatrix}0&0&0\\{[2]}&0&0\\0&1&0\end{pmatrix},\quad
K=\epsilon\begin{pmatrix}q^2&0&0\\0&1&0\\0&0&q^{-2}\end{pmatrix}.}
$$

Alternatively, preserving the printed $E$ instead requires $F_{21}=1$, $F_{32}=[2]$. Both corrected pairs are related by a diagonal change of [basis](../../../../../../basis.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
