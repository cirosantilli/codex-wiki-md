<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The specified bidegree is the [conjugate-linear Hodge star](../../../../../conjugate-linear-hodge-star.md), not the complex-linear extension of the real star. If the pointwise [Hermitian inner product](../../../../../hermitian-form.md) is linear in its first argument, it is defined by

$$
\alpha\wedge *\beta=\langle\alpha,\beta\rangle\,dV_g,\qquad *:A^{p,q}\longrightarrow A^{n-p,n-q}.
$$

It is the real [Hodge star operator](../../../../../hodge-star-operator.md) extended complex-linearly and composed with complex conjugation; $*^2=(-1)^{p+q}$. On a compact [Hermitian manifold](../../../../../hermitian-manifold.md),

$$
\boxed{(\alpha,\beta)_{L^2}=\int_M\alpha\wedge *\beta}
$$

is a positive definite [Hermitian inner product](../../../../../hermitian-form.md) on smooth forms. The formal adjoint is $\bar\partial^*=-*\bar\partial*$ in this convention; the final star in this identity is present in the PDF but is corrupted in the TeX aid.

State the relevant [Hodge theorem](../../../../../hodge-decomposition-theorem.md) as follows. On a compact manifold without boundary, the [Dolbeault Laplacian](../../../../../dolbeault-laplacian.md) $\Delta_{\bar\partial}=\bar\partial\bar\partial^*+\bar\partial^*\bar\partial$ is elliptic, self-adjoint and nonnegative. Its harmonic kernel $\mathcal H^{p,q}_{\bar\partial}$ is finite-dimensional, and smooth forms split orthogonally as this kernel plus the image of $\Delta_{\bar\partial}$. There are the orthogonal projection $H$ and a smooth Green operator $G$ with

$$
\Delta_{\bar\partial}G=G\Delta_{\bar\partial}=I-H,\qquad GH=HG=0.
$$

For any form $u$, expand the Laplacian term to obtain

$$
u=Hu+\bar\partial\bar\partial^*Gu+\bar\partial^*\bar\partial Gu.
$$

Harmonic forms are both closed and coclosed, since $(\Delta_{\bar\partial}v,v)=\|\bar\partial v\|^2+\|\bar\partial^*v\|^2$. They are orthogonal to both other terms; the two images are orthogonal because $(\bar\partial a,\bar\partial^*b)=(\bar\partial^2a,b)=0$. This proves the [Dolbeault Hodge decomposition](../../../../../dolbeault-hodge-decomposition-on-a-compact-hermitian-manifold.md)

$$
\boxed{A^{p,q}=\mathcal H^{p,q}_{\bar\partial}\oplus\bar\partial A^{p,q-1}\oplus\bar\partial^*A^{p,q+1}.}
$$

The closed forms are exactly the first two summands: if $\bar\partial u=0$, then $u$ is orthogonal to the adjoint image, and conversely the first two summands are closed. It follows that every [Dolbeault cohomology](../../../../../dolbeault-cohomology.md) class has a unique harmonic representative. Negative or out-of-range bidegrees mean zero spaces. Compactness and the absence of boundary are necessary for this stated global decomposition.

Now assume a [Kähler metric](../../../../../kahler-metric.md). Set $L=\omega\wedge-$ and $\Lambda=L^*$. The permitted [Kähler identities](../../../../../kahler-identities.md), stated with signs, are

$$
[\Lambda,\partial]=i\bar\partial^*,\qquad[\Lambda,\bar\partial]=-i\partial^*,
$$

with ordinary commutators because $\Lambda$ has even degree. Thus $\bar\partial^*=-i[\Lambda,\partial]$, and

$$
\partial\bar\partial^*+\bar\partial^*\partial=-i\{\partial(\Lambda\partial-\partial\Lambda)+(\Lambda\partial-\partial\Lambda)\partial\}=0
$$

by $\partial^2=0$. The companion identity gives $\bar\partial\partial^*+\partial^*\bar\partial=0$ in the same way.

Define $\Delta_d=dd^*+d^*d$ and $\Delta_\partial=\partial\partial^*+\partial^*\partial$. Expanding $d=\partial+\bar\partial$ and $d^*=\partial^*+\bar\partial^*$ makes the two mixed anticommutators vanish, so $\Delta_d=\Delta_\partial+\Delta_{\bar\partial}$. To prove equality of the latter two, substitute the same commutator formulas and use $\partial\bar\partial=-\bar\partial\partial$:

$$
\begin{aligned}
\Delta_\partial&=i(\partial\Lambda\bar\partial-\partial\bar\partial\Lambda-\Lambda\partial\bar\partial-\bar\partial\Lambda\partial),\\
\Delta_{\bar\partial}&=-i(\bar\partial\Lambda\partial+\partial\bar\partial\Lambda+\Lambda\partial\bar\partial-\partial\Lambda\bar\partial).
\end{aligned}
$$

The displayed operators are identical. Therefore the [Kähler Laplacian identity](../../../../../kahler-laplacian-identity.md) is

$$
\boxed{\Delta_d=\Delta_\partial+\Delta_{\bar\partial}=2\Delta_\partial=2\Delta_{\bar\partial}.}
$$

Let $\eta$ be a $\bar\partial$-exact form. It is closed and orthogonal to harmonic forms. The [Dolbeault Hodge decomposition](../../../../../dolbeault-hodge-decomposition-on-a-compact-hermitian-manifold.md), or the Green identity with $\alpha=G\eta$, therefore gives

$$
\boxed{\eta=\bar\partial\bar\partial^*\alpha,\qquad\alpha\in A^{p,q}.}
$$

For the Green construction, $\bar\partial\alpha=0$ follows since $G$ commutes with $\bar\partial$; equivalently the coexact component of a closed form vanishes. This yields exactly the stated factorization.

If also $\partial\eta=0$, put $\beta=\bar\partial^*\alpha$ and $\xi=\partial\beta$. The identities already proved give

$$
\bar\partial\xi=-\partial\bar\partial\beta=-\partial\eta=0,\qquad \bar\partial^*\xi=-\partial(\bar\partial^*)^2\alpha=0.
$$

Thus $\xi$ is harmonic for $\Delta_{\bar\partial}$ and hence for $\Delta_\partial$. But it is $\partial$-exact, so it is orthogonal to the harmonic summand in the [Hodge decomposition theorem](../../../../../hodge-decomposition-theorem.md). Consequently $\xi=0$, proving that **$\beta=\bar\partial^*\alpha$ is $\partial$-closed**.

Furthermore $\beta$ is orthogonal to the common harmonic space, since $(\beta,h)=(\alpha,\bar\partial h)=0$. Its $\partial$-Hodge decomposition then has neither a harmonic term nor a coexact term: closedness kills the coexact term. Therefore $\beta=\partial\chi$ for a form $\chi\in A^{p-1,q-1}$. It follows that

$$
\eta=\bar\partial\partial\chi=-\partial\bar\partial\chi,\qquad \boxed{\eta=\partial\bar\partial\phi,\quad\phi=-\chi\in A^{p-1,q-1}.}
$$

This proves the requested [ddbar lemma](../../../../../ddbar-lemma.md), including the intermediate harmonicity and orthogonality steps. The hypotheses $p,q\geq1$ ensure that the potential has a valid bidegree.

Finally $\eta=\omega_2-\omega_1$ is a real closed $(1,1)$ form and is $d$-exact. Integration by parts makes it orthogonal to every $d$-harmonic form. By the [Kähler Laplacian identity](../../../../../kahler-laplacian-identity.md) it is also orthogonal to the Dolbeault harmonic space; because it is $\bar\partial$-closed, the [Dolbeault Hodge decomposition](../../../../../dolbeault-hodge-decomposition-on-a-compact-hermitian-manifold.md) makes it $\bar\partial$-exact. Apply the proved [ddbar lemma](../../../../../ddbar-lemma.md) to get $\eta=\partial\bar\partial\phi$ for a smooth complex-valued function. Reality gives $\eta=-\partial\bar\partial\overline\phi$, so averaging yields

$$
\eta=\frac12\partial\bar\partial(\phi-\overline\phi)=i\partial\bar\partial\operatorname{Im}\phi.
$$

With $f=\operatorname{Im}\phi$,

$$
\boxed{\omega_2=\omega_1+i\partial\bar\partial f,\qquad f\in C^\infty(M,\mathbb R).}
$$

The potential is defined up to a real constant on each connected component. This is a statement about cohomologous [Kähler forms](../../../../../kahler-form.md), not about an arbitrary pair of such forms.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
