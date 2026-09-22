<h1 id="19j/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Mackey restriction formula](../../../../../../../mackey-restriction-formula.md) says that for subgroups $H,K\leq G$ and a $K$-representation $W$,

$$
\operatorname{Res}_H^G\operatorname{Ind}_K^GW
\cong
\bigoplus_{x\in H\backslash G/K}
\operatorname{Ind}_{H\cap xKx^{-1}}^H
\operatorname{Res}_{H\cap xKx^{-1}}^{xKx^{-1}}({}^xW),
$$

where ${}^xW(xkx^{-1})=W(k)$.

For $H=K=B$, the [Bruhat decomposition of SL2 over a finite field](../../../../../../../bruhat-decomposition-of-sl2-over-a-finite-field.md) gives

$$
G=B\sqcup BwB,
\qquad
w=\begin{pmatrix}0&-1\\1&0\end{pmatrix}.
$$

Thus $B\backslash G/B$ has representatives $1,w$. The identity double coset contributes $\theta$, while

$$
B\cap wBw^{-1}=T
$$

contributes an induced representation from the diagonal subgroup. Therefore

$$
\boxed{
\operatorname{Res}_B^G\operatorname{Ind}_B^G\theta
\cong
\theta\oplus\operatorname{Ind}_T^B(\theta^w|_T),
}
$$

where

$$
\theta^w(t)=\theta(w^{-1}tw).
$$

For $t(a)=\operatorname{diag}(a,a^{-1})$, one has $w^{-1}t(a)w=t(a^{-1})$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [19J](../../../19j.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
