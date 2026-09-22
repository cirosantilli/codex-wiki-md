<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the [joint energy](../../../../../joint-energy-of-a-symmetric-markov-semigroup.md) convention

$$
\mathcal E_\mu(f,g)=\lim_{s\downarrow0}\frac1s\langle f-P_sf,g\rangle_{L^2(\mu)},
\qquad \mathcal E_\mu(f)=\mathcal E_\mu(f,f).
$$

On the [generator domain](../../../../../generator-domain.md) it is $-\langle Lf,g\rangle$. The [symmetric Feller semigroup](../../../../../symmetric-feller-semigroup.md) has symmetric two-point measure $\nu_s(dx,dy)=\mu(dx)P_s(x,dy)$, with both marginals equal to $\mu$. Expanding the product of increments gives the finite-time identity

$$
\mathcal E_{\mu,s}(f,g)
=\frac1{2s}\int(f(x)-f(y))(g(x)-g(y))\,d\nu_s(x,y)
$$

for real functions. This supplies a proof that works for a general symmetric Markov kernel, without assuming a diffusion chain rule.

For $a\geq b\geq0$, [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives

$$
\begin{aligned}
(a^{q/2}-b^{q/2})^2
&=\frac{q^2}{4}\left(\int_b^a r^{q/2-1}\,dr\right)^2\\
&\leq\frac{q^2}{4}(a-b)\int_b^a r^{q-2}\,dr\\
&=\frac{q^2}{4(q-1)}(a^{q-1}-b^{q-1})(a-b).
\end{aligned}
$$

Interchanging $a,b$ gives the same inequality in the other order. Apply it with $a=f(x),b=f(y)$, integrate against $\nu_s$, and take $s\downarrow0$. This proves the [power inequality for symmetric Markov energies](../../../../../power-inequality-for-symmetric-markov-energies.md)

$$
\boxed{\mathcal E_\mu(f^{q/2})
\leq\frac{q^2}{4(q-1)}\mathcal E_\mu(f^{q-1},f).}
$$

Initially take bounded nonnegative functions in the form domain. On their bounded range, the power maps are Lipschitz; their finite-time squared-increment energies are therefore bounded by a constant times that of $f$. This puts the powers in the form domain and makes both [joint energy](../../../../../joint-energy-of-a-symmetric-markov-semigroup.md) limits well defined. Truncation gives the corresponding extended-energy interpretation when needed. In particular the proof applies to the bounded positive functions used below.

Normalize the [logarithmic Sobolev inequality](../../../../../logarithmic-sobolev-inequality.md) as

$$
\operatorname{Ent}_\mu(g^2)\leq c_{\mathrm{LS}}\mathcal E_\mu(g),\qquad
\operatorname{Ent}_\mu(h)
=\int h\log h\,d\mu-\left(\int h\,d\mu\right)\log\left(\int h\,d\mu\right).
$$

Start with a bounded $f$ bounded away from zero, and put $u(t)=P_tf$, $q=q(t)$ and $F(t)=\int u^q\,d\mu$. Positivity and preservation of constants keep $u$ within the same positive bounds. Symmetry realizes $P_t$ as a self-adjoint [contraction semigroup](../../../../../contraction-semigroup.md) on $L^2(\mu)$, so for $t>0$ its orbit lies in the [generator domain](../../../../../generator-domain.md) and $\partial_tu=Lu$; this justifies the following differentiation away from zero.

Differentiate both the evolving function and exponent:

$$
F'=q\int u^{q-1}Lu\,d\mu+q'\int u^q\log u\,d\mu.
$$

Since $\log\|u\|_q=q^{-1}\log F$, it follows that

$$
\frac d{dt}\log\|u\|_q
=-\frac{\mathcal E_\mu(u^{q-1},u)}{F}
+\frac{q'}{q^2F}\operatorname{Ent}_\mu(u^q).
$$

Apply the [logarithmic Sobolev inequality](../../../../../logarithmic-sobolev-inequality.md) to $g=u^{q/2}$, and then the [joint energy](../../../../../joint-energy-of-a-symmetric-markov-semigroup.md) inequality:

$$
\operatorname{Ent}_\mu(u^q)
\leq c_{\mathrm{LS}}\mathcal E_\mu(u^{q/2})
\leq\frac{c_{\mathrm{LS}}q^2}{4(q-1)}
\mathcal E_\mu(u^{q-1},u).
$$

Therefore

$$
\frac d{dt}\log\|u\|_q
\leq\left(\frac{c_{\mathrm{LS}}q'}{4(q-1)}-1\right)
\frac{\mathcal E_\mu(u^{q-1},u)}{F}.
$$

The specified exponent satisfies $q(0)=2$ and $q'=4(q-1)/c_{\mathrm{LS}}$. Thus the right side is zero and the evolving [norm](../../../../../norm.md) is nonincreasing. Integrating from a positive time $\delta$ and letting $\delta\downarrow0$ gives

$$
\|P_tf\|_{q(t)}\leq\|f\|_2.
$$

Here the initial limit follows from strong $L^2$ continuity, boundedness of $f$ and $P_\delta f$, and $q(\delta)\to2$.

For a bounded nonnegative $f$, apply the estimate to $f+\epsilon$ and let $\epsilon\downarrow0$. For arbitrary $f\in L^2(\mu)$, truncate $|f|$ to bounded nonnegative functions. Their images converge in $L^2$ to $P_t|f|$; an almost-everywhere convergent subsequence and [Fatou lemma](../../../../../fatou-s-lemma.md) give the same $L^{q(t)}$ estimate for that limit. Positivity of the Markov kernel gives $|P_tf|\leq P_t|f|$, also for complex $f$, so

$$
\boxed{P_tf\in L^{1+e^{4t/c_{\mathrm{LS}}}}(\mu),\qquad
\|P_tf\|_{1+e^{4t/c_{\mathrm{LS}}}}\leq\|f\|_2.}
$$

This proves that the [logarithmic Sobolev inequality implies hypercontractivity](../../../../../logarithmic-sobolev-inequality-implies-hypercontractivity.md), with the numerical exponent matched to the stated joint-energy normalization.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 8](../../paper-8-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
