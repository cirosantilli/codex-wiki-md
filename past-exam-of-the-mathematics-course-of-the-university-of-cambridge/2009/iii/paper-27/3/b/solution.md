<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The normalized [Eisenstein series](../../../../../../eisenstein-series.md) satisfy $E_4=1+240\sum_{m\ge1}\sigma_3(m)q^m$ and $E_6=1-504\sum_{m\ge1}\sigma_5(m)q^m$. Their weights are four and six. The [valence formula for the modular group](../../../../../../valence-formula-for-the-modular-group.md) makes the normalized weight-twelve [cusp form](../../../../../../cusp-form.md) $\Delta$ have one simple cusp zero and no zero in $\mathbb H$. Comparing its first coefficient gives $\Delta=(E_4^3-E_6^2)/1728$.

Odd weights vanish because $-I$ acts by $(-1)^k$. Weight two vanishes by the [valence formula for the modular group](../../../../../../valence-formula-for-the-modular-group.md): the forced zero at $i$ alone contributes $1/2>2/12$. For every remaining nonnegative even weight, except two, choose $a,b\ge0$ with $4a+6b=k$. Subtract the constant coefficient of $f$ times $E_4^aE_6^b$. The remainder is a [cusp form](../../../../../../cusp-form.md); division by $\Delta$ produces a holomorphic [modular form](../../../../../../modular-form.md) of weight $k-12$. The cusp and interior orders justify this division. Induction on the weight proves

$$
\boxed{M_*(SL_2(\mathbb Z))=\mathbb C[E_4,E_6].}
$$

The [integral triangular basis of level-one modular forms](../../../../../../integral-triangular-basis-of-level-one-modular-forms.md) is $F_j=\Delta^jE_4^{a_j}E_6^{b_j}$, with $4a_j+6b_j=k-12j\ge0$ and $k-12j\ne2$. The induction just given shows these span, and their distinct leading terms $q^j$ show linear independence. Every coefficient is integral by the hypothesis on $\Delta$ and the displayed Eisenstein expansions. In $f=\sum_jc_jF_j$, compare coefficients successively: $c_0=a_0$, then $c_1$ is $a_1$ minus an integer combination of already integral coefficients, and similarly for every $j$. The largest permitted $j$ is at most $\lfloor(k+1)/12\rfloor$, so the stipulated initial coefficients make every $c_j$ integral. Therefore **all Fourier coefficients of $f$ are integers**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
