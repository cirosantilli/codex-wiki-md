<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For each sample point put $A_n=\max_{0\leq k<2^n}|X_{(k+1)2^{-n}}-X_{k2^{-n}}|$. First take $s<t$ in the [dyadic rationals](../../../../../../../dyadic-rational.md), set $h=t-s$, and choose $N\geq0$ with $2^{-N}\leq h<2^{1-N}$. The left grid approximations $s_N=2^{-N}\lfloor2^Ns\rfloor$ and $t_N=2^{-N}\lfloor2^Nt\rfloor$ are at most two grid steps apart, so $|X_{t_N}-X_{s_N}|\leq2A_N$.

For either endpoint $r$, successive left approximations $r_n,r_{n+1}$ are equal or one step apart on the level-$(n+1)$ grid. Since $r$ is dyadic these approximations eventually equal $r$ exactly. The [triangle inequality](../../../../../../../triangle-inequality.md) therefore gives

$$
|X_t-X_s|\leq2\sum_{n\geq N}A_n
\leq2^{-N\alpha}\,2\sum_{n\geq N}2^{n\alpha}A_n
\leq h^\alpha K_\alpha.
$$

The second inequality is valid also for $\alpha=0$. Thus **the required bound holds simultaneously for every dyadic pair** whenever $K_\alpha$ is finite; if it is infinite the inequality holds in the extended sense. For $s=t$ the left side is zero. This is [dyadic increment chaining](../../../../../../../dyadic-increment-chaining.md), with the stated constant two.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 34](../../../../paper-34-split.md)
5. [Iii](../../../../split.md)
6. [2005](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
