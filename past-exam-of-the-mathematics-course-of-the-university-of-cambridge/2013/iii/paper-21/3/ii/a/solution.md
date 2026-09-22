<h1 id="3/ii/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $\zeta=\zeta_{p^n}$, with $n\geq1$. The shifted [cyclotomic polynomial](../../../../../../../cyclotomic-polynomial.md) $\Phi_{p^n}(1+X)$ is [Eisenstein](../../../../../../../eisenstein-criterion.md) at $p$: its constant term is $p$, and modulo $p$ it is $X^{p^{n-1}(p-1)}$. Therefore $L/\mathbb Q_p$ is [totally ramified](../../../../../../../totally-ramified-extension.md) of degree $p^{n-1}(p-1)$ and $\pi=\zeta-1$ is a [uniformiser](../../../../../../../uniformizer.md).

The [Galois group](../../../../../../../galois-group.md) is $(\mathbb Z/p^n\mathbb Z)^\times$, with $\sigma_a(\zeta)=\zeta^a$. For $a\ne1$, let $r=v_p(a-1)$, $0\leq r<n$. Then $\zeta^{a-1}$ is a primitive $p^{n-r}$th root. Its difference from one is a [uniformiser](../../../../../../../uniformizer.md) in the corresponding smaller cyclotomic field, and the relative [ramification index](../../../../../../../ramification-index.md) is $p^r$. Hence

$$
v_L(\sigma_a(\pi)-\pi)=v_L(\zeta^{a-1}-1)=p^r.
$$

The [uniformizer criterion for lower ramification groups](../../../../../../../uniformizer-criterion-for-lower-ramification-groups.md) now determines every group. Write $U_j=\{a\in(\mathbb Z/p^n\mathbb Z)^\times:a\equiv1\pmod{p^j}\}$, with $U_n=\{1\}$. Then the [lower ramification filtration of a prime-power cyclotomic extension](../../../../../../../lower-ramification-filtration-of-a-prime-power-cyclotomic-extension.md) is

$$
\boxed{\begin{aligned}
G_{-1}=G_0&=(\mathbb Z/p^n\mathbb Z)^\times,\\
G_i&=U_j&&\text{if }1\leq j\leq n-1,\quad p^{j-1}\leq i\leq p^j-1,\\
G_i&=\{1\}&&\text{if }i\geq p^{n-1}.
\end{aligned}}
$$

For $n=1$ the middle range is empty and the extension is tame. The formula also includes $p=2$; then $U_1$ is already the whole group, so the first possible drop is later than in the odd-prime case. For $p=2,n=1$, the entire extension is trivial.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [Ii](../../ii.md)
3. [3](../../../3.md)
4. [Paper 21](../../../../paper-21-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
