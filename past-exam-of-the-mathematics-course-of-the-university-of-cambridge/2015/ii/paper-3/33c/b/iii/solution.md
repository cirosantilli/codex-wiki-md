<h1 id="33c/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $n=N/V$ and $B=B_2(T)$. Differentiating the [virial expansion](../../../../../../../virial-expansion.md) $p=k_BT(n+Bn^2)$ at fixed pressure gives

$$
0=(n+Bn^2+TB'n^2)\,dT+T(1+2Bn)\,dn.
$$

Since $dV/V=-dn/n$,

$$
\frac TV\left(\frac{\partial V}{\partial T}\right)_p-1=\frac{n(TB'-B)}{1+2Bn}=n(TB'-B)+O(n^2).
$$

Thus the [virial criterion for Joule-Thomson cooling](../../../../../../../virial-criterion-for-joule-thomson-cooling.md) gives, **for the displayed truncated equation of state**,

$$
\boxed{\mu=\frac N{C_p}\frac{TB_2'-B_2}{1+2B_2n}=\frac N{C_p}(TB_2'-B_2)[1-2B_2n+O(n^2)].}
$$

In particular the first density correction to the ideal-gas thermal-expansion factor gives the leading result $\mu=N(TB_2'-B_2)/C_p$. The heat capacity here is the actual $C_p$ at the state considered; replacing it by an ideal-gas value is a further leading-order approximation. On the low-density mechanically stable branch with $C_p>0$ and $1+2B_2n>0$, **positive cooling coefficient requires**

$$
\boxed{TB_2'-B_2>0\quad\Longleftrightarrow\quad\frac d{dT}\left(\frac{B_2(T)}T\right)>0.}
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [33C](../../../33c.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
