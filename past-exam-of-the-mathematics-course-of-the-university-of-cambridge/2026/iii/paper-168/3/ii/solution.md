<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

If $\alpha>1/2$, [monotonicity](../../../../../../monotone-boolean-function.md) already gives $\mathbb E f^{(1/2)}\geq\alpha>1/2$, so assume $\alpha\leq1/2$. Suppose for a contradiction that $\mathbb E f^{(1/2)}\leq1/2$. By the [mean value theorem](../../../../../../mean-value-theorem.md), some $s\in(p,1/2)$ satisfies

$$
\frac d{ds}\mathbb E f^{(s)}
\leq\frac{1/2-\alpha}{1/2-p}
\leq\frac1\zeta.
$$

The [Margulis–Russo formula](../../../../../../margulis-russo-formula.md) identifies this derivative with the appropriately normalized [total influence](../../../../../../total-influence.md), so $\mathbf I_s(f)$ is bounded solely in terms of $\zeta$. The $p$-biased [Friedgut junta theorem](../../../../../../friedgut-junta-theorem.md) then supplies, for any small $\eta>0$, a Boolean $J$-[junta](../../../../../../junta.md) $h$ with $|J|\leq r(\zeta,\eta)$ and

$$
\mathbb P_s[f\ne h]\leq\eta.
$$

Because $f$ is monotone, $\mathbb P_s(f=1)\leq1/2$, hence $\mathbb P_s(h=0)\geq1/2-\eta\geq1/4$ when $\eta\leq1/4$. It follows that

$$
\mathbb P_s[f=1\mid h=0]\leq4\eta.
$$

For some assignment $u$ on $J$ with $h(u)=0$, therefore, $\mathbb E_s f_u\leq4\eta$. Monotonicity and $p<s$ imply $\mathbb E_p f_u\leq4\eta$. Choose $\eta<\alpha/5$, set $\varepsilon=\eta$, and take $r\geq|J|$. Then

$$
|\mathbb E_p f_u-\mathbb E_p f|\geq\alpha-4\eta>\eta,
$$

contradicting $(\varepsilon,p,r)$-quasirandomness. Thus $\mathbb E f^{(1/2)}>1/2$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 168](../../../paper-168-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
