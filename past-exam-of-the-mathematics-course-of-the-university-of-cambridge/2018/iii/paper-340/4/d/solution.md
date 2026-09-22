<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The printed bound is false, even for $s=2$ and zero noise. Let $P=I_7-\mathbf1\mathbf1^T/7$ and choose $A$ with six orthonormal rows spanning $\mathbf1^\perp$, so $A^TA=P$. For a vector supported on at most $s$ entries,

$$
\|Ax\|_2^2=\|x\|_2^2-\frac{|\sum_ix_i|^2}{7},\qquad \delta_s(A)=s/7.
$$

Take $x_0=(0,0,1,1,1,1,1)$, $s=2$, and $\eta=0$. Every feasible vector is $x_0+t\mathbf1$, whose $\ell^1$ objective is $2|t|+5|1+t|$. Its unique minimizer is $\hat x=(-1,-1,0,0,0,0,0)$. Yet

$$
\delta_2=\frac27<\frac13,\qquad
\|\hat x-x_0\|_2=\sqrt7>\frac3{\sqrt2}=\frac{\sigma_2(x_0)}{\sqrt2}.
$$

No choice of the noise constant repairs this example. Also $s=1$ must be excluded: $A=(1,1)$ has $\delta_1=0$, but its two unit-coordinate vectors have identical measurements and both minimize [basis pursuit](../../../../../../basis-pursuit.md).

The corrected conclusion, for $s\ge2$, is

$$
\boxed{\|\hat x-x_0\|_2\le C_1\eta+C_2\frac{\sigma_s(x_0)}{\sqrt s},}
$$

with both constants depending on the [restricted isometry constant](../../../../../../restricted-isometry-constant.md). The order-$s$ threshold itself is valid for $s\ge2$; it need not be replaced by an order-$2s$ threshold. A precise sharp robust recovery theorem gives, for $\delta=\delta_s<1/3$, the admissible constants

$$
C_1=\frac{2\sqrt{2(1+\delta)}}{1-3\delta},\qquad
C_2=\frac{2\sqrt2(2\delta+\sqrt{(1-3\delta)\delta})+2(1-3\delta)}{1-3\delta}.
$$

This is the standard stable recovery result, invoked here explicitly; its order restriction and constants are given in [https://arxiv.org/pdf/1302.1236,](https://arxiv.org/pdf/1302.1236,) Theorem 3.3.

For completeness, the mechanism behind a [robust null space property](../../../../../../robust-null-space-property.md) proof is as follows. Put $h=\hat x-x_0$, let $S$ index the largest $s$ entries of $x_0$, and write $\sigma=\|x_{0,S^c}\|_1$. Feasibility and minimality give the tube and cone inequalities

$$
\|Ah\|_2\le2\eta,\qquad \|h_{S^c}\|_1\le\|h_S\|_1+2\sigma.
$$

If $A$ has the [robust null space property](../../../../../../robust-null-space-property.md) with $0\le\rho<1$ and $\tau>0$, namely $\|h_T\|_2\le\rho\|h_{T^c}\|_1/\sqrt s+\tau\|Ah\|_2$ for every $|T|\le s$, then

$$
\|h\|_1\le\frac{2(1+\rho)}{1-\rho}\sigma+\frac{2\tau}{1-\rho}\sqrt s\,\|Ah\|_2.
$$

Apply that property again to the largest $s$ entries $T$ of $h$. Sorted coefficients satisfy $\|h_{T^c}\|_2\le\|h\|_1/\sqrt s$, because each tail entry is at most $\|h\|_1/s$. Therefore

$$
\|h\|_2\le\frac{2(1+\rho)^2}{1-\rho}\frac{\sigma}{\sqrt s}
+\frac{\tau(3+\rho)}{1-\rho}\|Ah\|_2.
$$

This proves the usual two-constant conclusion under the explicitly stated [robust null space property](../../../../../../robust-null-space-property.md) and explains why a fixed coefficient one is not supplied by that argument. The sharp order-$s$ theorem above supplies the conclusion for the actual printed threshold, after the necessary corrections.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
