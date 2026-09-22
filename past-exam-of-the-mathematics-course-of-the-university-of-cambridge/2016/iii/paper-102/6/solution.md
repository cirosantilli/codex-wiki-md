<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A smooth [vector field](../../../../../vector-field.md) on a [smooth manifold](../../../../../smooth-manifold.md) $M$ is a smooth section of the [tangent bundle](../../../../../tangent-bundle.md): it assigns $v(p)\in T_pM$ to each $p$, smoothly in local coordinates. In a coordinate chart it has the form $v=\sum_i a_i\partial/\partial x_i$, with smooth coefficients $a_i$. Equivalently, it acts on smooth functions as a derivation, $v(fh)=v(f)h+fv(h)$.

For a [Lie group](../../../../../lie-group.md) $G$, write $L_a(h)=ah$ for [Left translation on a Lie group](../../../../../left-and-right-translation-on-a-lie-group.md). A [left-invariant vector field](../../../../../left-invariant-vector-field.md) satisfies

$$
(dL_a)_h v(h)=v(ah)\qquad(a,h\in G).
$$

Thus it is determined by its value at the identity. Given the printed $X\in T_gG$, first translate it to the identity:

$$
\xi=(dL_{g^{-1}})_gX\in T_eG.
$$

The unique [left-invariant vector field](../../../../../left-invariant-vector-field.md) with value $X$ at $g$ is

$$
\boxed{v_X(h)=(dL_h)_e\xi=(dL_{hg^{-1}})_gX.}
$$

The smoothness of multiplication makes this a smooth [vector field](../../../../../vector-field.md), the chain rule proves left invariance, and setting $h=g$ gives $v_X(g)=X$.

We prove the [completeness of left-invariant vector fields](../../../../../completeness-of-left-invariant-vector-fields.md): this [left-invariant vector field](../../../../../left-invariant-vector-field.md) is a [complete vector field](../../../../../complete-vector-field.md). The [Picard-Lindelöf theorem](../../../../../picard-lindelof-theorem.md), applied in a local chart, gives a unique local [integral curve of a vector field](../../../../../integral-curve-of-a-vector-field.md) $u:(-\varepsilon,\varepsilon)\to G$ through $e$. For every $h\in G$, the curve $t\mapsto hu(t)$ is an [integral curve of a vector field](../../../../../integral-curve-of-a-vector-field.md) through $h$, because

$$
\frac{d}{dt}(hu(t))=(dL_h)_{u(t)}v_X(u(t))=v_X(hu(t)).
$$

Crucially, the same interval $(-\varepsilon,\varepsilon)$ works for every initial point.

Let $\gamma$ be the maximal [integral curve of a vector field](../../../../../integral-curve-of-a-vector-field.md) through $g$, with maximal interval $(a,b)$. If $b<\infty$, choose $t_0\in(a,b)$ with $b-t_0<\varepsilon/2$. The curve

$$
t\longmapsto\gamma(t_0)u(t-t_0)
$$

exists on $(t_0-\varepsilon,t_0+\varepsilon)$ and agrees with $\gamma$ on the overlap by uniqueness of the local [ordinary differential equation](../../../../../ordinary-differential-equation.md). It extends $\gamma$ past $b$, a contradiction. The same argument at a finite $a$ excludes that possibility. Thus $(a,b)=\mathbb R$, and uniqueness on overlapping intervals gives uniqueness on all of $\mathbb R$.

After establishing completeness, uniqueness also gives the [one-parameter subgroup](../../../../../one-parameter-subgroup.md) law for the global curve through $e$:

$$
u(s+t)=u(s)u(t).
$$

Both sides, as curves in $t$, are [integral curves of a vector field](../../../../../integral-curve-of-a-vector-field.md) through $u(s)$ at $t=0$. Defining the [Exponential map of a Lie group](../../../../../exponential-map-of-a-lie-group.md) by $u(t)=\exp(t\xi)$, the answer is

$$
\boxed{\gamma_g(t)=g\exp(t\xi),\qquad \xi=(dL_{g^{-1}})_gX,\qquad t\in\mathbb R.}
$$

**The identity component $G^\circ$ is an open normal subgroup, and every open identity neighbourhood generates it.** Let $G^\circ$ be the [connected component](../../../../../connected-component.md) of $e$. The product of connected spaces is connected, so the image of $G^\circ\times G^\circ$ under multiplication is connected and contains $e$. It is therefore contained in $G^\circ$. Inversion has the same property. Thus $G^\circ$ is a [subgroup](../../../../../subgroup.md).

A [smooth manifold](../../../../../smooth-manifold.md) is locally connected. In particular, a coordinate neighbourhood of $e$ can be chosen homeomorphic to an open ball, so there is a connected open neighbourhood $O$ of $e$ contained in $G^\circ$. Its translates $hO$, $h\in G^\circ$, are open and lie in $G^\circ$, and cover $G^\circ$. Therefore the [identity component of a Lie group](../../../../../identity-component-of-a-lie-group.md) is open in $G$. Conjugation by any $a\in G$ is a [homeomorphism](../../../../../homeomorphism.md) fixing $e$, so it maps $G^\circ$ into itself; conjugation by $a^{-1}$ gives the reverse inclusion. Hence $G^\circ$ is a [normal subgroup](../../../../../normal-subgroup.md).

If $U$ is an open neighbourhood of $e$ in $G^\circ$, let $H=\langle U\rangle$, allowing inverses in the meaning of generated [subgroup](../../../../../subgroup.md). For each $h\in H$, $hU$ is open and lies in $H$, so $H=\bigcup_{h\in H}hU$ is open in $G^\circ$. Every other left [coset](../../../../../coset.md) of $H$ is also open. Thus $H$ is both open and closed in the connected space $G^\circ$. It is nonempty, so $H=G^\circ$.

A [quadratic form](../../../../../quadratic-form.md) on $V=\mathbb R^n$ is a function $Q(v)=B(v,v)$ for a symmetric [bilinear form](../../../../../bilinear-form.md) $B$. Equivalently, $Q(tv)=t^2Q(v)$ and the polarization

$$
B(u,v)=\frac{Q(u+v)-Q(u)-Q(v)}2
$$

is a [bilinear map](../../../../../bilinear-map.md). In coordinates there is a unique real [symmetric matrix](../../../../../symmetric-matrix.md) $A$ with $Q(v)=v^TAv$. No assumption of nondegeneracy or positive definiteness is needed.

An element $g\in\operatorname{GL}_n(\mathbb R)$ stabilizes $Q$ when $Q(gv)=Q(v)$ for every $v$. By the [polarization identity](../../../../../polarization-identity.md), this is equivalent to preserving $B$, or in coordinates to

$$
G_Q=\{g\in\operatorname{GL}_n(\mathbb R):g^TAg=A\}.
$$

This is a closed [Matrix Lie group](../../../../../matrix-lie-group.md). The [Lie algebra of a quadratic-form stabilizer](../../../../../lie-algebra-of-a-quadratic-form-stabilizer.md) is

$$
\boxed{T_eG_Q=\{X\in M_n(\mathbb R):X^TA+AX=0\}.}
$$

To prove necessity, differentiate $g(t)^TAg(t)=A$ along any smooth curve in $G_Q$ with $g(0)=I$, $g'(0)=X$. The derivative at zero is $X^TA+AX$.

To prove sufficiency, suppose $X^TA+AX=0$ and consider the [matrix exponential](../../../../../matrix-exponential.md) $g(t)=e^{tX}$. Then

$$
\frac{d}{dt}\bigl(e^{tX^T}Ae^{tX}\bigr)=e^{tX^T}(X^TA+AX)e^{tX}=0.
$$

Its value at zero is $A$, so $e^{tX}\in G_Q$ for every real $t$. This curve has derivative $X$ at zero, proving the claimed [tangent space](../../../../../tangent-space.md) description even for a degenerate [quadratic form](../../../../../quadratic-form.md).

Equivalently, the condition is $B(Xu,v)+B(u,Xv)=0$ for all $u,v$. For a nondegenerate [quadratic form](../../../../../quadratic-form.md) it is the corresponding [Special orthogonal Lie algebra](../../../../../special-orthogonal-lie-algebra.md). To see the degenerate case explicitly, choose a [basis](../../../../../basis.md) with

$$
A=\begin{pmatrix}D&0\\0&0\end{pmatrix},\qquad D=\operatorname{diag}(I_r,-I_s).
$$

Writing $X=\begin{pmatrix}P&R\\S&T\end{pmatrix}$, the condition becomes

$$
P^TD+DP=0,\qquad R=0,
$$

while $S,T$ are arbitrary. Thus the nullspace of the [quadratic form](../../../../../quadratic-form.md) is invariant, but arbitrary infinitesimal maps into it are allowed. When $A=0$, the formula correctly gives $G_Q=\operatorname{GL}_n(\mathbb R)$ and $T_eG_Q=M_n(\mathbb R)$.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 102](../../paper-102-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
