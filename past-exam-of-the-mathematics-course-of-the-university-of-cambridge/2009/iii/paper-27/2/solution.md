<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A weight-$2n$ [meromorphic modular form](../../../../../meromorphic-modular-form.md) satisfies $f(\gamma z)=(cz+d)^{2n}f(z)$, while $d(\gamma z)=(cz+d)^{-2}dz$. The factors cancel in $f(z)(dz)^n$, giving a $\Gamma$-invariant [meromorphic n-differential](../../../../../meromorphic-n-differential.md) on the [complex upper half-plane](../../../../../upper-half-plane-complex-analysis.md).

Away from elliptic points and cusps, descend this differential through local inverse branches of the quotient map. At an elliptic point of effective stabilizer order $e$, choose a coordinate $t$ in which the stabilizer acts by $t\mapsto\zeta t$, and use $w=t^e$ downstairs. If the lifted coefficient has order $r$, invariance forces $r+n$ to be divisible by $e$. The descended differential has integer order

$$
\boxed{\operatorname{ord}_{w}\omega(f)=\frac{r+n}{e}-n.}
$$

Indeed $F(w)(dw)^n$ pulls back to $e^nt^{n(e-1)}F(t^e)(dt)^n$. At a [modular cusp](../../../../../cusp-of-a-modular-group.md) of width $h$, the coordinate $q_c=e^{2\pi iz/h}$ gives $dz=(h/(2\pi i))dq_c/q_c$. Therefore

$$
\boxed{\operatorname{ord}_{c}\omega(f)=v_c(f)-n.}
$$

Both formulas provide meromorphic extensions over the omitted points, producing the unique differential with the prescribed pullback on the [compactified modular curve](../../../../../compactified-modular-curve.md).

For the character-valued question, write $X=X_0(N)$ and let $f$ be the chosen nonzero meromorphic form. The quotient of two forms with the same weight and [Dirichlet character](../../../../../dirichlet-character.md) is a meromorphic function on $X$. At an interior point $P$ with effective elliptic order $e_P$ (one at ordinary points), let $r_P$ be the vanishing order of the lifted $f$. At a cusp let $v_c$ be its order in the width coordinate; this can be fractional because of the character multiplier. Multiplying by a meromorphic function $\varphi$ changes these orders by $e_P\operatorname{ord}_P\varphi$ and $\operatorname{ord}_c\varphi$, respectively. Interior holomorphy requires a nonnegative order, while cusp vanishing requires a strictly positive order. The exact [divisor](../../../../../divisor.md) is consequently

$$
D(f)=\sum_{P\text{ interior}}\left\lfloor\frac{r_P}{e_P}\right\rfloor P
+\sum_{c\text{ cusp}}(\lceil v_c\rceil-1)c.
$$

Only finitely many coefficients are nonzero. The order inequalities are equivalent to $\operatorname{div}(\varphi)+D(f)\ge0$. Division by $f$ proves the reverse inclusion, so the [Riemann-Roch space](../../../../../riemann-roch-space.md) gives

$$
\boxed{S_k(\Gamma_1(N),\chi)=fL(D(f)).}
$$

This extends the [cusp-form divisor presentation](../../../../../cusp-form-divisor-presentation.md) to elliptic points and character multipliers.

Choose a nonzero meromorphic one-differential on $X$, and let $g$ be its weight-two pullback. For $f_t=fg^t$, the interior order is $r_P(f)+t r_P(g)$ and the cusp order is $v_c(f)+t v_c(g)$. The elliptic orders are one, two or three, so adding six to $t$ changes each interior floor by $6r_P(g)/e_P$, and each cusp ceiling by $6v_c(g)$. The [valence formula for the modular group](../../../../../valence-formula-for-the-modular-group.md) for $g$ says $\sum_P r_P(g)/e_P+\sum_c v_c(g)=d/6$, where $d=[SL_2(\mathbb Z):\Gamma_0(N)]$. Thus

$$
\deg D(f_{t+6})-\deg D(f_t)=d,\qquad
\deg D(f_t)=dt/6+B(t\bmod6).
$$

The degrees tend to infinity. For sufficiently large $t$, the [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md) therefore gives

$$
\boxed{\dim S_{k+2t}(\Gamma_1(N),\chi)=\frac{dt}{6}+A(t\bmod6)>0,\qquad A=B+1-g(X).}
$$

The periodic formula obtained this way is an eventual formula. For small $t$, the exact answer includes the Riemann-Roch correction $\ell(K_X-D(f_t))$; it should not silently be discarded without the large-degree hypothesis.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
