<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $\operatorname{TV}(u)=|Du|(\Omega)$ for the [total variation seminorm on a domain](../../../../../total-variation-seminorm-on-a-domain.md). For a [locally integrable](../../../../../locally-integrable-function.md) real function its dual definition is

$$
|Du|(\Omega)=\sup\left\{\int_\Omega u\,\operatorname{div}\varphi\,dx:\varphi\in C_c^1(\Omega;\mathbb R^2),\ |\varphi(x)|\le1\right\}.
$$

The [bounded-variation space](../../../../../function-of-bounded-variation-on-a-domain.md) consists of functions $u\in L^1(\Omega)$ with finite $|Du|(\Omega)$, equipped with $\|u\|_{BV}=\|u\|_1+|Du|(\Omega)$. In the equivalent [distributional derivative](../../../../../distributional-derivative.md) description, $Du$ is a finite vector-valued [Radon measure](../../../../../radon-measure.md) and $|Du|$ is its [total variation measure](../../../../../variation-measure.md).

To establish [completeness of the bounded-variation space](../../../../../completeness-of-the-bounded-variation-space.md), let $(u_n)$ be [Cauchy](../../../../../cauchy-sequence.md) in this [norm](../../../../../norm.md). Completeness of $L^1$ gives $u_n\to u$ in $L^1$. Given $\varepsilon>0$, choose $N$ so that $\|u_n-u_m\|_{BV}<\varepsilon$ whenever $m,n\ge N$. For fixed $n\ge N$, the given [lower semicontinuity](../../../../../lower-semicontinuity.md) yields

$$
|D(u_n-u)|(\Omega)\le\liminf_{m\to\infty}|D(u_n-u_m)|(\Omega).
$$

Since $\|u_n-u_m\|_1\to\|u_n-u\|_1$, we obtain $\|u_n-u\|_1+|D(u_n-u)|(\Omega)\le\varepsilon$. In particular $u_n-u$ has finite variation; the [triangle inequality](../../../../../triangle-inequality.md) then puts $u$ in the [BV space](../../../../../function-of-bounded-variation-on-a-domain.md). The same bound proves convergence in the full [norm](../../../../../norm.md), so this is a [Banach space](../../../../../banach-space-split.md).

For the disk data, put $B=B(0,R)$ and assume $\alpha>0$. The exact [total variation denoising of a disk](../../../../../total-variation-denoising-of-a-disk.md) is

$$
\boxed{u_*=(1-2\alpha/R)_+\chi_B.}
$$

Here $(s)_+=\max(s,0)$ is the [positive part](../../../../../positive-part-of-a-real-valued-function.md). A [total variation calibration](../../../../../total-variation-calibration.md) certifies global optimality, including competitors that are not radial or piecewise constant. Define the bounded [vector field](../../../../../vector-field.md)

$$
z(x)=\begin{cases}x/R,&|x|\le R,\\Rx/|x|^2,&|x|>R.\end{cases}
$$

It has $|z|\le1$. Its normal component is [continuous](../../../../../continuous-function.md) across the circle, so the [distributional divergence](../../../../../distributional-divergence.md) has no extra boundary measure. Direct differentiation gives $q=\operatorname{div}z=(2/R)\chi_B$. The dual definition implies $\int vq\le\operatorname{TV}(v)$: for the standard $BV\cap L^2$ domain one can cut $z$ off at radius $L$, with the error bounded by $C L^{-1}\int_{L<|x|<2L}|v|\to0$, and then smooth the test field. In the larger [homogeneous bounded-variation space](../../../../../homogeneous-bounded-variation-space.md), the same error is bounded by $C\|v\|_{L^2(L<|x|<2L)}\to0$. Thus both usual whole-plane formulations give the same certificate.

Use the [perimeter](../../../../../perimeter.md) identity $\operatorname{TV}(\chi_B)=2\pi R$ and $|B|=\pi R^2$. If $c=1-2\alpha/R>0$, then $\int c\chi_Bq=2\pi Rc=\operatorname{TV}(c\chi_B)$ and $u_*-g+\alpha q=0$. Consequently every competitor $v$ satisfies

$$
\begin{aligned}
E(v)-E(u_*)&\ge\alpha\langle q,v-u_*\rangle+\langle u_*-g,v-u_*\rangle+\tfrac12\|v-u_*\|_2^2\\
&=\tfrac12\|v-u_*\|_2^2\ge0.
\end{aligned}
$$

If $\alpha\ge R/2$, replace $z$ by $z_\alpha=(R/(2\alpha))z$. Its [norm](../../../../../norm.md) is still at most one, its divergence is $q_\alpha=\chi_B/\alpha$, and equality in the calibration holds at $u_*=0$. The identical comparison proves optimality and uniqueness of zero, including the threshold $\alpha=R/2$. The only general results used are completeness of $L^1$, [lower semicontinuity](../../../../../lower-semicontinuity.md) of variation, the indicator-perimeter identity, the distributional integration-by-parts/dual variation formula and the quadratic [norm](../../../../../norm.md) identity. For $\alpha=0$, the unique squared-error [minimizer](../../../../../global-minimizer.md) is simply $g$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 64](../../paper-64-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
