<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An eigenform is understood to be nonzero; the zero form would put no constraint on the alleged [eigenvalues](../../../../../../eigenvalue.md). The coefficient of $q$ in $T_w(n)f$ is $c(n)$, since $\gcd(n,1)=1$. Comparing with the coefficient in $\lambda(n)f$ gives

$$
\boxed{c(n)=c(1)\lambda(n).}
$$

The constant coefficient comparison gives $\lambda(n)c(0)=\sigma_{w-1}(n)c(0)$, so

$$
\boxed{c(0)\ne0\ \Longrightarrow\ \lambda(n)=\sigma_{w-1}(n).}
$$

For completeness derive the operator multiplication law underlying the last relation. On formal [Fourier series](../../../../../../fourier-series-split.md) define

$$
U_p\left(\sum c(r)q^r\right)=\sum c(pr)q^r,\qquad
V_p f(q)=f(q^p),\qquad A=p^{w-1}.
$$

These auxiliary maps need not separately preserve modularity, but coefficient identities are valid and $U_pV_p=I$. Part (a) gives

$$
T_w(p^e)=\sum_{j=0}^e A^jV_p^jU_p^{e-j}.
$$

Multiplication on the left by $U_p+AV_p$ yields the $T_w(p^{e+1})$ sum and, from $U_pV_p^j=V_p^{j-1}$ for $j\geq1$, the remaining sum $A T_w(p^{e-1})$. Hence

$$
T_w(p)T_w(p^e)=T_w(p^{e+1})+A T_w(p^{e-1})\quad(e\geq1).
$$

Induction on the smaller exponent, applying this recurrence and cancelling its two overlapping sums, now gives

$$
T_w(p^r)T_w(p^s)=\sum_{j=0}^{\min(r,s)}A^jT_w(p^{r+s-2j}).
$$

To make the induction explicit, write $T_r=T_w(p^r)$ and assume $2\leq r\leq s$. Substituting the formulas already established for $r-1$ and $r-2$ into $T_rT_s=(T_1T_{r-1}-AT_{r-2})T_s$ gives

$$
\begin{aligned}
T_rT_s&=\sum_{j=0}^{r-1}A^jT_{r+s-2j}
+\sum_{j=0}^{r-1}A^{j+1}T_{r+s-2-2j}
-\sum_{j=0}^{r-2}A^{j+1}T_{r+s-2-2j}\\
&=\sum_{j=0}^{r-1}A^jT_{r+s-2j}+A^rT_{s-r}.
\end{aligned}
$$

The last term is exactly the missing $j=r$ term. The cases $r=0,1$ are the identity operator and the prime recurrence above.

For distinct primes, their $U$ and $V$ maps commute, and the [divisor](../../../../../../divisor.md) formula in (a) factors independently at each prime. It follows that $T_w(m)T_w(n)=T_w(mn)$ for coprime $m,n$. Multiplying the prime-power identities therefore gives the general [Hecke multiplication relations](../../../../../../hecke-multiplication-relations.md)

$$
T_w(m)T_w(n)=\sum_{a\mid\gcd(m,n)}a^{w-1}T_w(mn/a^2).
$$

Apply this identity to the same nonzero eigenform and cancel the [vector](../../../../../../vector.md) $f$, obtaining

$$
\boxed{\lambda(m)\lambda(n)=\sum_{a\mid\gcd(m,n)}a^{w-1}\lambda(mn/a^2).}
$$

This reasoning does not silently divide by $c(1)$, which is important when considering noncuspidal weight-zero forms.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
