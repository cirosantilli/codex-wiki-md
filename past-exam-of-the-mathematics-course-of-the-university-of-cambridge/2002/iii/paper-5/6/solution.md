<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Treat $F$ as a [vector](../../../../../vector.md)-valued solution; matrix solutions are handled columnwise. It is important to distinguish the coefficient convention from the indicial exponent. In a fixed Fuchsian frame, a finite singularity at $a$ means

$$
A(z)=\frac{R_a}{z-a}+B_a(z),
$$

where $B_a$ is [holomorphic](../../../../../complex-differentiability-at-a-point.md) near $a$. The [residue](../../../../../residue.md) is $R_a$, equivalently the residue of the matrix-valued one-form $A(z)\,dz$. Such a [Fuchsian linear differential system](../../../../../fuchsian-linear-differential-system.md) has a [regular singular point](../../../../../regular-singular-point.md): on sectors, its solutions have at most power and logarithmic growth. Intrinsically a regular singular system can be made Fuchsian by a meromorphic change of frame; a higher coefficient pole in some other frame does not itself prove irregularity. Residues here refer to the displayed fixed coefficient one-form.

At infinity use $w=1/z$ and $\widetilde F(w)=F(1/w)$. The equation becomes

$$
\widetilde F'(w)+\widetilde A(w)\widetilde F(w)=0,\qquad
\widetilde A(w)=-w^{-2}A(1/w).
$$

A Fuchsian singularity at infinity means $\widetilde A$ has at most a simple pole at $w=0$, and $R_\infty=\operatorname{Res}_{w=0}\widetilde A(w)$. The [residue theorem](../../../../../residue-theorem.md) applied entrywise on the [Riemann sphere](../../../../../riemann-sphere.md) gives

$$
\boxed{\sum_{a\in\widehat{\mathbb C}}R_a=0.}
$$

For a direct calculation when all coefficient poles are simple, write $A(z)=P(z)+\sum_jR_j/(z-a_j)$ by rational partial fractions. Regularity at infinity in this frame requires $A(z)=O(1/z)$, so $P=0$. Transforming coordinates gives $R_\infty=-\sum_jR_j$. More generally the entrywise residue theorem remains valid even when a different meromorphic frame has higher-order poles.

**The printed nonconstant-solution claim is false.** A counterexample satisfying its spectral hypothesis is

$$
A(z)=\frac1z\begin{pmatrix}0&0\\0&-1/3\end{pmatrix}.
$$

Its residue has eigenvalues $0,-1/3$, with zero of largest real part. The equations are $u'=0$ and $v'-v/(3z)=0$. If $v$ is analytic at zero, coefficient comparison gives $(n-1/3)v_n=0$ for every nonnegative integer $n$, so $v=0$. Hence every analytic solution is $(c,0)^T$, which is constant. This disproves nonconstancy, rather than silently replacing it with a weaker conclusion.

A useful correct conclusion is that a nonzero analytic solution exists under the stated hypotheses. Write $A=R/z+\sum_{j\geq0}B_jz^j$, and let $m$ be the largest nonnegative integer with $-m\in\operatorname{spec}R$; such an $m$ exists because $0\in\operatorname{spec}R$. Choose a nonzero $h_0\in\ker(mI+R)$ and seek

$$
F(z)=z^mH(z),\qquad H(z)=\sum_{n\geq0}h_nz^n.
$$

The [Frobenius method](../../../../../frobenius-method.md) gives

$$
((m+n)I+R)h_n=-\sum_{j=0}^{n-1}B_jh_{n-1-j}\qquad(n\geq1).
$$

All left-hand matrices are invertible by maximality of $m$. For large $n$ their inverse norm is $O(1/n)$ by a geometric-series inverse; enlarging the constant bounds every $n\geq1$ by $C/n$. If $\|B_j\|\leq Mr^{-j}$ on a smaller disc, the scalar majorant with generating function

$$
v(t)=\|h_0\|(1-t/r)^{-CMr}
$$

satisfies $v'=CM(1-t/r)^{-1}v$ and dominates the recurrence coefficientwise. It converges for $|t|<r$, proving convergence of $H$. Thus the [analytic solution at a maximal integer Fuchsian exponent](../../../../../analytic-solution-at-a-maximal-integer-fuchsian-exponent.md) is nonzero, and is nonconstant if $m>0$. When $m=0$, nonconstancy requires additional information, as the counterexample shows.

There is also a sign problem in the printed exponent terminology. Substitution of $F=z^\mu H$ with $H(0)\neq0$ into the actual equation gives

$$
(\mu I+R)H(0)=0.
$$

Thus **the indicial exponents are eigenvalues of $-R$, not $R$**. With the printed sign, an exponent of maximal real part admits a pure [Frobenius solution](../../../../../frobenius-solution.md), because the corresponding coefficient matrices are invertible at all subsequent positive integer steps. Lesser exponents can meet resonance.

The supplied example does not demonstrate such failure. Solving it directly gives

$$
\boxed{F(z)=\begin{pmatrix}c_1-c_2z^2/2\\c_2z\end{pmatrix}.}
$$

Every solution is analytic. The residue eigenvalue $-1$ corresponds to the true exponent $1$, and setting $c_1=0$ gives $F=z(-c_2z/2,c_2)^T$ with nonzero leading coefficient. Even with the literal printed factor $z^{-1}$, every displayed solution has the form $z^{-1}H$ with $H=zF$ analytic, though $H(0)=0$.

Nevertheless the last existence-of-a-counterexample request, read literally, can be fulfilled by the diagonal counterexample above. For its nonmaximal residue eigenvalue $\lambda=-1/3$, substitution of $F=z^{-1/3}H$ yields

$$
\left((n-1/3)I+\operatorname{diag}(0,-1/3)\right)h_n=0
$$

for every integer $n\geq0$. Neither diagonal entry, $n-1/3$ or $n-2/3$, vanishes, so $H=0$. Therefore **there is no nonzero solution of that literal form**, even without imposing $H(0)\neq0$.

For the intended logarithmic resonance phenomenon with correctly signed exponents, take instead

$$
\widetilde A(z)=\begin{pmatrix}0&-1\\0&1/z\end{pmatrix}.
$$

Its equation gives $v=c_2/z$ and $u=c_1+c_2\operatorname{Log}z$ on a chosen branch. The exponent $-1$ would require $H(0)=(0,c_2)^T\neq0$, but $z\operatorname{Log}z$ prevents $H=zF$ from being analytic when $c_2\neq0$. The exponent zero has the constant solution $(1,0)^T$. This supplies an explicit resonance obstruction under the correct convention and completes the qualified resolution of the printed defects.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 5](../../paper-5-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
