<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For the $R$-$R$-[bimodule](../../../../../bimodule.md) $M$, the [Hochschild chain complex](../../../../../hochschild-chain-complex.md) is

$$
C_n(R,M)=M\otimes_kR^{\otimes_kn},
$$

with boundary

$$
\begin{aligned}
b(m\otimes r_1\otimes\cdots\otimes r_n)
={}&mr_1\otimes r_2\otimes\cdots\otimes r_n\\
&+\sum_{i=1}^{n-1}(-1)^im\otimes r_1\otimes\cdots\otimes r_ir_{i+1}\otimes\cdots\otimes r_n\\
&+(-1)^nr_nm\otimes r_1\otimes\cdots\otimes r_{n-1}.
\end{aligned}
$$

Then

$$
HH_n(R,M)=H_n(C_\bullet(R,M),b).
$$

The [Hochschild cochain complex](../../../../../hochschild-cochain-complex.md) is $C^n(R,M)=\operatorname{Hom}_k(R^{\otimes_kn},M)$ with

$$
\begin{aligned}
(\delta f)(r_1,\ldots,r_{n+1})
={}&r_1f(r_2,\ldots,r_{n+1})\\
&+\sum_{i=1}^{n}(-1)^if(r_1,\ldots,r_ir_{i+1},\ldots,r_{n+1})\\
&+(-1)^{n+1}f(r_1,\ldots,r_n)r_{n+1},
\end{aligned}
$$

and $HH^n(R,M)=H^n(C^\bullet(R,M),\delta)$.

A [derivation into a bimodule](../../../../../derivation-into-a-bimodule.md) is a $k$-linear map $d:R\to M$ satisfying

$$
d(rs)=r d(s)+d(r)s.
$$

It is an [inner derivation](../../../../../inner-derivation.md) when $d=d_m$ for some $m\in M$, where $d_m(r)=rm-mr$. The degree-one cocycle equation is precisely the [Leibniz rule](../../../../../leibniz-rule.md), and the degree-one coboundaries are the inner derivations. Therefore the [First Hochschild cohomology as outer derivations](../../../../../first-hochschild-cohomology-as-outer-derivations.md) is

$$
\boxed{HH^1(R,M)\cong\operatorname{Der}_k(R,M)/\operatorname{Inn}(R,M).}
$$

Let $\mu:R\otimes_kR\to R$ be multiplication and $\Omega=\ker\mu$, equipped with the outer bimodule structure. The [universal bimodule derivation](../../../../../universal-bimodule-derivation.md)

$$
D:R\longrightarrow\Omega,\qquad D(r)=r\otimes1-1\otimes r
$$

satisfies $D(rs)=rD(s)+D(r)s$. Composition with $D$ defines

$$
\operatorname{Hom}_{R-R}(\Omega,M)\longrightarrow\operatorname{Der}_k(R,M).
$$

For a derivation $d$, its inverse image under this map is

$$
\theta_d\left(\sum_ir_i\otimes s_i\right)=\sum_id(r_i)s_i.
$$

If $\sum_ir_is_i=0$, the Leibniz rule shows that this formula is both left and right $R$-linear. Moreover every element of $\Omega$ is $\sum_iD(r_i)s_i$, proving existence and uniqueness.

For $d_m(r)=rm-mr$, the corresponding map is

$$
\boxed{\theta_m\left(\sum_ir_i\otimes s_i\right)=\sum_ir_ims_i.}
$$

These are exactly the maps $\Omega\to M$ which extend to bimodule maps $R\otimes_kR\to M$.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 148](../../paper-148-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
