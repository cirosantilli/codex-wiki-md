<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For $\lambda\ne0$, suppose $R=(\lambda1-ba)^{-1}$ exists. The identities $(\lambda1-ab)a=a(\lambda1-ba)$ and $b(\lambda1-ab)=(\lambda1-ba)b$ show, by multiplication on either side, that

$$
\boxed{(\lambda1-ab)^{-1}=\lambda^{-1}(1+aRb).}
$$

For example, multiplying on the left gives $1-\lambda^{-1}ab+\lambda^{-1}a(\lambda1-ba)Rb=1$, and the right product gives the same cancellation. Thus invertibility of $\lambda1-ba$ implies invertibility of $\lambda1-ab$. Interchanging $a,b$ proves the converse. The [nonzero spectra of products in opposite orders](../../../../../nonzero-spectra-of-products-in-opposite-orders.md) are therefore equal:

$$
\boxed{\sigma_A(ab)\setminus\{0\}=\sigma_A(ba)\setminus\{0\}.}
$$

In particular the requested inclusion follows. The exclusion of zero matters: for the [unilateral shift operator](../../../../../unilateral-shift-operator.md) $S$, $S^*S=1$ has [Banach algebra spectrum](../../../../../spectrum-of-an-element.md) $\{1\}$, whereas $SS^*=1-P_0$ has [Banach algebra spectrum](../../../../../spectrum-of-an-element.md) $\{0,1\}$.

Use the spectral definition of a [Positive element of a C-star algebra](../../../../../positive-element-of-a-c-star-algebra.md): $h$ is positive if $h=h^*$ and $\sigma_A(h)\subseteq[0,\infty)$. We use the standard [continuous functional calculus](../../../../../continuous-functional-calculus.md) for a [Hermitian element of a C-star algebra](../../../../../hermitian-element-of-a-c-star-algebra.md), including its real [Banach algebra spectrum](../../../../../spectrum-of-an-element.md) and the equality of its [norm](../../../../../norm.md) with its [spectral radius](../../../../../spectral-radius.md). To prove $a^*a$ positive without assuming this as part of the definition, first establish two elementary cone facts.

If $p,q$ are positive and $s=\|p\|+\|q\|$, the [continuous functional calculus](../../../../../continuous-functional-calculus.md) gives $\|\|p\|1-p\|\leq\|p\|$ and the corresponding bound for $q$, hence

$$
\|s1-p-q\|\leq s.
$$

Since $p+q$ is self-adjoint, every spectral value $t$ is real and satisfies $|s-t|\leq s$, so $t\geq0$. Thus the [positive cone of a C-star algebra](../../../../../positive-cone-of-a-c-star-algebra.md) is closed under addition. It is proper: if both $h$ and $-h$ are positive, their [Banach algebra spectra](../../../../../spectrum-of-an-element.md) force $\sigma(h)\subseteq\{0\}$, and the self-adjoint [norm](../../../../../norm.md) equality gives $h=0$. It is also [norm](../../../../../norm.md) closed: if $p_n\geq0$ converges to $p$, choose $r\geq\sup_n\|p_n\|$; then $\|r1-p_n\|\leq r$ passes to the limit and forces every spectral value of $p$ to be nonnegative.

Now put $h=a^*a$, and form its negative part $d=\max(-h,0)$ by [continuous functional calculus](../../../../../continuous-functional-calculus.md). Let $c=ad^{1/2}$. Because $d$ is a function of $h$, the scalar identity $t\max(-t,0)=-\max(-t,0)^2$ gives

$$
c^*c=d^{1/2}hd^{1/2}=-d^2.
$$

This has nonpositive [Banach algebra spectrum](../../../../../spectrum-of-an-element.md). The previously proved equality of nonzero product [Banach algebra spectra](../../../../../spectrum-of-an-element.md) shows that $cc^*$ also has nonpositive [Banach algebra spectrum](../../../../../spectrum-of-an-element.md); it is self-adjoint, so both $c^*c$ and $cc^*$ are negative elements. Write $c=u+iv$, where $u=(c+c^*)/2$ and $v=(c-c^*)/(2i)$ are self-adjoint. Direct multiplication gives

$$
c^*c+cc^*=2(u^2+v^2).
$$

By the [spectral mapping theorem](../../../../../spectral-mapping-theorem.md), the squares $u^2,v^2$ are positive, so their sum is positive by the cone fact above. But the same sum is negative, since both its original summands are negative. Properness forces $c^*c+cc^*=0$. Then $c^*c=-cc^*$ is both negative and positive, so $c^*c=0$, whence $d^2=0$. The [C-star identity](../../../../../c-star-identity.md) applied to the self-adjoint $d$ gives $\|d\|^2=\|d^2\|=0$. Thus $d=0$, proving

$$
\boxed{a^*a\geq0.}
$$

This establishes [positivity of adjoint products from spectral positivity](../../../../../positivity-of-adjoint-products-from-spectral-positivity.md). It also proves positivity under congruence: for $p\geq0$ and any $z$, write $p=r^2$ using its functional-calculus square root; then $z^*pz=(rz)^*(rz)\geq0$.

For the comparison of squares, we first derive [inversion reverses the order of strictly positive elements](../../../../../inversion-reverses-the-order-of-strictly-positive-elements.md). If $0<x\leq y$ with both positive and invertible, then

$$
k=x^{-1/2}yx^{-1/2}\geq1.
$$

The [continuous functional calculus](../../../../../continuous-functional-calculus.md) gives $k^{-1}\leq1$, because the scalar function $1-t^{-1}$ is nonnegative on $\sigma(k)\subseteq[1,\infty)$. Congruence then gives

$$
y^{-1}=x^{-1/2}k^{-1}x^{-1/2}\leq x^{-1}.
$$

No commutation of $x,y$ was assumed.

Next derive the [square-root resolvent integral in a C-star algebra](../../../../../square-root-resolvent-integral-in-a-c-star-algebra.md). For $s\geq0$,

$$
\sqrt{s}=\frac1\pi\int_0^\infty t^{-1/2}\frac{s}{t+s}\,dt.
$$

For $s>0$, substituting $t=su^2$ reduces the integral to $\sqrt{s}\,\pi^{-1}\int_0^\infty2/(1+u^2)\,du=\sqrt{s}$; for $s=0$ it is zero. For a positive element $x$, the [norm](../../../../../norm.md) of $x(t1+x)^{-1}$ is at most $\min(1,\|x\|/t)$. Thus the integral converges in [norm](../../../../../norm.md), with integrable bounds $t^{-1/2}$ near zero and $\|x\|t^{-3/2}$ near infinity, uniform on $\sigma(x)$. The [continuous functional calculus](../../../../../continuous-functional-calculus.md) consequently gives

$$
x^{1/2}=\frac1\pi\int_0^\infty t^{-1/2}x(t1+x)^{-1}\,dt.
$$

Put $\alpha=a^2$ and $\beta=b^2$. The assumption $b^2-a^2\geq0$ says $\alpha\leq\beta$. For every $t>0$, inversion reverses the order of the strictly positive elements $t1+\alpha$ and $t1+\beta$. Subtracting the two square-root formulas therefore yields

$$
b-a=\beta^{1/2}-\alpha^{1/2}
=\frac1\pi\int_0^\infty t^{1/2}\bigl((t1+\alpha)^{-1}-(t1+\beta)^{-1}\bigr)\,dt\geq0.
$$

Here $\alpha^{1/2}=a$ and $\beta^{1/2}=b$ because $a,b$ themselves are positive. Every truncated integral has a positive integrand, so is positive; [norm](../../../../../norm.md) convergence and closedness of the [positive cone of a C-star algebra](../../../../../positive-cone-of-a-c-star-algebra.md) make its limit positive. This proves [order preservation by the positive square root](../../../../../order-preservation-by-the-positive-square-root.md) in the required case:

$$
\boxed{b^2\geq a^2,\ a,b\geq0\Longrightarrow b-a\geq0.}
$$

It is important that this argument does not factor $b^2-a^2$ as $(b-a)(b+a)$, which would be invalid for noncommuting elements.

For $p=b-a\geq0$, apply the continuous function $t\mapsto\sqrt t$ on its nonnegative compact [Banach algebra spectrum](../../../../../spectrum-of-an-element.md). The resulting element $p^{1/2}$ is self-adjoint, has nonnegative [Banach algebra spectrum](../../../../../spectrum-of-an-element.md) by [continuous functional calculus](../../../../../continuous-functional-calculus.md), and satisfies $(p^{1/2})^2=p$. Thus **$b-a$ has a [positive square root in a C-star algebra](../../../../../positive-square-root-in-a-c-star-algebra.md)**.

Finally, if the positive element $a$ is invertible, its compact [Banach algebra spectrum](../../../../../spectrum-of-an-element.md) is bounded away from zero. Let $\varepsilon=\min\sigma(a)>0$; [continuous functional calculus](../../../../../continuous-functional-calculus.md) gives $a\geq\varepsilon1$. Since $b\geq a$, we also have $b\geq\varepsilon1$, so $\sigma(b)\subseteq[\varepsilon,\infty)$. The reciprocal function is continuous on this [Banach algebra spectrum](../../../../../spectrum-of-an-element.md) and supplies $b^{-1}$. Therefore $\boxed{a\text{ invertible}\Longrightarrow b\text{ invertible}}$ under the given positivity assumptions.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
