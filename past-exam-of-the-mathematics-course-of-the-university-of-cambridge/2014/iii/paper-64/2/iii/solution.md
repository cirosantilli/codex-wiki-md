<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The literal assumptions suffice for the scalar [quadratic fidelity](../../../../../../quadratic-fidelity.md) problem. One can avoid regularity of level-set boundaries by moving only a clipped part of the [minimizer](../../../../../../global-minimizer.md). We prove the stronger [jump-amplitude inequality for total variation denoising](../../../../../../jump-amplitude-inequality-for-total-variation-denoising.md):

$$
\boxed{[u]_{\nu_u}\bigl([f]_{\nu_u}-[u]_{\nu_u}\bigr)\ge0\quad\mathcal H^{n-1}\text{-a.e. on }J_u.}
$$

Comparison with the zero function gives finite energy and hence $u\in L^2$. Here $u=\hat u$, and both differences use the same oriented [BV traces on a hypersurface](../../../../../../bv-trace-on-a-hypersurface.md). Reversing the normal reverses both differences and leaves the inequality unchanged. Outside $J_f$, the two traces of $f$ agree, so the inequality would read $-[u]^2\ge0$ at a jump of $u$. It therefore gives the requested [no-new-jumps property of total variation denoising](../../../../../../no-new-jumps-property-of-total-variation-denoising.md) in every dimension.

First use [residual-preserving clipping of an ROF minimizer](../../../../../../residual-preserving-clipping-of-an-rof-minimizer.md). For an integer $M>0$, put

$$
w=T_Mu=\max(-M,\min(M,u)),\qquad r=u-w,\qquad g=f-r=f-u+w.
$$

The [coarea formula for BV functions](../../../../../../coarea-formula-for-bv-functions.md) gives [scalar total variation splitting under clipping](../../../../../../scalar-total-variation-splitting-under-clipping.md):

$$
\operatorname{TV}(u)=\operatorname{TV}(w)+\operatorname{TV}(r).
$$

Indeed the levels in $(-M,M)$ contribute to $w$, while the levels outside that interval contribute to $r$. This uses the full signed coarea formula. For any $z\in BV(\Omega)\cap L^2(\Omega)$, minimality of $u$ and the [triangle inequality](../../../../../../triangle-inequality.md) for the [total variation seminorm](../../../../../../total-variation-seminorm-on-a-domain.md) give

$$
\alpha\operatorname{TV}(w)+\alpha\operatorname{TV}(r)+\tfrac12\|w-g\|_2^2
\le\alpha\operatorname{TV}(z+r)+\tfrac12\|z-g\|_2^2
\le\alpha\operatorname{TV}(z)+\alpha\operatorname{TV}(r)+\tfrac12\|z-g\|_2^2.
$$

Cancel the tail variation. Thus $w$ is a bounded [ROF denoising](../../../../../../total-variation-denoising.md) [minimizer](../../../../../../global-minimizer.md) for $g\in BV(\Omega)\cap L^2(\Omega)$. The data $g$ may still be unbounded. This is an exact reduction preserving $w-g=u-f$; it does not truncate the data and then pass to a limit of different reconstructions.

We next prove the [jump-amplitude inequality for a bounded ROF minimizer](../../../../../../jump-amplitude-inequality-for-a-bounded-rof-minimizer.md), allowing its data to be unbounded. Fix a coordinate $j$, a nonnegative $\varphi\in C_c^\infty(\Omega)$, and let $\Phi_t$ be the [local flow](../../../../../../local-flow.md) of the smooth [vector field](../../../../../../vector-field.md) $Y=\varphi e_j$. The flow is the identity near the domain boundary, preserves each line parallel to $e_j$, and satisfies $\Phi_{-t}=\Phi_t^{-1}$. Write

$$
T_ta=a\circ\Phi_t,\qquad \delta_ta=T_ta-a,\qquad J_t=\det D\Phi_t.
$$

These maps are [diffeomorphisms](../../../../../../diffeomorphism.md), with $J_{\pm t}=1+O(t)$ and $J_t+J_{-t}-2=O(t^2)$ uniformly.

The useful trace calculation is the [BV jump-product limit with one bounded factor](../../../../../../bv-jump-product-limit-with-one-bounded-factor.md). For $a\in BV(\Omega)$ and $b\in BV(\Omega)\cap L^\infty(\Omega)$,

$$
\lim_{t\downarrow0}\frac1t\int_\Omega\delta_ta\,\delta_tb\,dx
=\int_{J_b}[a]_{\nu_b}[b]_{\nu_b}\,\varphi|\nu_b\cdot e_j|\,d\mathcal H^{n-1}.
$$

The right side is integrable: $|[b]|\le2\|b\|_\infty$ and only the common jump part of $a$ contributes. The same limit holds with both increments replaced by their negative-time increments, still dividing by positive $t$.

Here is why this calculation needs only one bounded factor. By the [BV slicing theorem](../../../../../../bv-slicing-theorem.md), almost every coordinate slice of $a$ and $b$ has one-sided representatives. On one such interval let $\mu=Da$ and use its right-continuous representative. Since $\varphi\ge0$,

$$
\delta_ta(x)=\mu((x,\Phi_t(x)]).
$$

[Fubini's theorem](../../../../../../fubini-s-theorem.md) rewrites the slice integral as

$$
\frac1t\int\delta_ta\,\delta_tb\,dx
=\int\left(\frac1t\int_{\Phi_{-t}(s)}^s\delta_tb(x)\,dx\right)d\mu(s).
$$

At each interior $s$, the inner expression tends to $\varphi(s)(b(s+)-b(s-))$; if $\varphi(s)=0$, it is zero. Its absolute value is at most $2\|b\|_\infty\|\varphi\|_\infty$. [Dominated convergence](../../../../../../dominated-convergence-theorem.md) against $|\mu|$ therefore leaves just the [measure atoms](../../../../../../atom-measure-theory.md) common to the two slices. The bound $2\|b\|_\infty\|\varphi\|_\infty|Da|$ is also integrable over the transverse coordinates, by the [BV slicing theorem](../../../../../../bv-slicing-theorem.md). Integrating the slice jump sums gives the surface integral and its factor $|\nu_b\cdot e_j|$. Negative-time increments give the same product, because both slice differences reverse sign. At no point is a uniform bound on $a$ across the slices required.

For $0<\theta<1$, use the mixed competitors

$$
w_t=(1-\theta)w+\theta T_tw.
$$

The [total variation under opposite smooth flows](../../../../../../total-variation-under-opposite-smooth-flows.md) satisfies

$$
\operatorname{TV}(T_tw)+\operatorname{TV}(T_{-t}w)-2\operatorname{TV}(w)=O(t^2).
$$

To see this for the entire [vector Radon measure](../../../../../../vector-radon-measure.md) $Dw=\sigma_w|Dw|$, the [change of variables formula](../../../../../../change-of-variables-formula.md) gives

$$
\operatorname{TV}(T_tw)=\int_\Omega|\operatorname{cof}(D\Phi_{-t})\sigma_w|\,d|Dw|.
$$

For $\operatorname{cof}A=(\det A)A^{-T}$, the two [cofactor matrices](../../../../../../cofactor-matrix.md) expand as $I\pm tB+O(t^2)$, with the same $B$ and opposite signs. Their [norm](../../../../../../norm.md) expansions on $|\sigma_w|=1$ have cancelling linear terms. Integrating proves the estimate, including the absolutely continuous, jump and Cantor parts. The BV transformation formula is also given in [Lemma 4.2 on differentiable regularizers](https://arxiv.org/html/2312.01900v2); that lemma does not assume bounded data. The [total variation seminorm](../../../../../../total-variation-seminorm-on-a-domain.md) is a [convex function](../../../../../../convex-function.md), so

$$
\operatorname{TV}(w_t)+\operatorname{TV}(w_{-t})-2\operatorname{TV}(w)\le O(t^2).
$$

Thus minimality forces the sum of the two fidelity changes to have nonnegative limit after division by $t$.

It remains to evaluate that sum without bounding $g$. Put $F_g(v)=\tfrac12\|v-g\|_2^2$. Exact expansion of the [quadratic fidelity](../../../../../../quadratic-fidelity.md), together with [change of variables](../../../../../../change-of-variables-formula.md), gives the [opposite-flow fidelity identity for quadratic data](../../../../../../opposite-flow-fidelity-identity-for-quadratic-data.md):

$$
F_g(w_t)+F_g(w_{-t})-2F_g(w)
=-\frac{\theta(1-\theta)}2\bigl(\|\delta_tw\|_2^2+\|\delta_{-t}w\|_2^2\bigr)
+\theta\int\delta_tg\,\delta_tw\,dx+o(t).
$$

For completeness, the cross-term identity fixing its sign is

$$
\int g(\delta_tw+\delta_{-t}w)\,dx
=-\int\delta_tg\,\delta_tw\,dx+\int g(1-J_{-t})\delta_{-t}w\,dx.
$$

The last integral is $o(t)$: $\|1-J_{-t}\|_\infty=O(t)$, while

$$
\int|g|\,|\delta_{-t}w|\,dx
\le K\|\delta_{-t}w\|_1+2\|w\|_\infty\int_{\{|g|>K\}}|g|\,dx\longrightarrow0.
$$

Take $t\to0$ first, then $K\to\infty$. Here $g\in L^1$ and the [local flow](../../../../../../local-flow.md) is strongly continuous in $L^1$. The remaining Jacobian mass term is $O(t^2)\|w\|_2^2$. This argument avoids multiplying an unbounded fidelity derivative by an uncontrolled derivative measure.

Apply the [BV jump-product limit with one bounded factor](../../../../../../bv-jump-product-limit-with-one-bounded-factor.md) with $(a,b)=(g,w)$ and $(w,w)$, and use minimality. For every nonnegative $\varphi$ and every coordinate $j$,

$$
0\le\int_{J_w}\left([g][w]-(1-\theta)[w]^2\right)\varphi|\nu_w\cdot e_j|\,d\mathcal H^{n-1}.
$$

Let $\theta\downarrow0$. These are inequalities for finite signed [Radon measures](../../../../../../radon-measure.md), so arbitrary nonnegative smooth tests imply nonnegativity of their densities. Since at least one coordinate of a unit normal is nonzero,

$$
[w]([g]-[w])\ge0\quad\mathcal H^{n-1}\text{-a.e. on }J_w.
$$

This proves the bounded-minimizer lemma with arbitrary $BV\cap L^2$ data.

Finally return to $w=T_Mu$ and $g=f-u+w$. At almost every finite [approximate jump point](../../../../../../approximate-jump-point.md) of $u$, choose an integer $M>\max(|u^+|,|u^-|)$. The [BV traces on a hypersurface](../../../../../../bv-trace-on-a-hypersurface.md) commute with clipping, so $w^\pm=u^\pm$, $r^\pm=0$ and $g^\pm=f^\pm$ there. It is consequently a jump point of $w$, and its inequality is exactly $[u]([f]-[u])\ge0$. A countable union over $M$ removes all exceptional surface-null sets. Outside $J_f$, the [BV traces on a hypersurface](../../../../../../bv-trace-on-a-hypersurface.md) of $f$ agree almost everywhere. We conclude

$$
\boxed{\mathcal H^{n-1}(J_{\hat u}\setminus J_f)=0\qquad\text{for }f\in BV(\Omega)\cap L^2(\Omega),\ \Omega\subset\mathbb R^n.}
$$

The mechanism is exact scalar coarea splitting, paired smooth-flow variations, a one-bounded-factor BV trace limit, and localization through integer clipping levels. It works in every dimension under the printed hypotheses, without essential boundedness of $f$ or $u$ and without regularity of their level-set boundaries.

In [total variation calibration](../../../../../../total-variation-calibration.md) notation, $\operatorname{div}z=(u-f)/\alpha$. Since this divergence is itself in the [BV space](../../../../../../function-of-bounded-variation-on-a-domain.md), the proved inequality equivalently reads

$$
[u]_{\nu_u}[\operatorname{div}z]_{\nu_u}\le0.
$$

Thus an upward output jump forces the appropriate nonpositive jump of the calibrated divergence. This is a consequence of the variational argument above, with common oriented [BV traces on a hypersurface](../../../../../../bv-trace-on-a-hypersurface.md); no curvature of the rectifiable interface or differentiability of its normal is assumed.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
