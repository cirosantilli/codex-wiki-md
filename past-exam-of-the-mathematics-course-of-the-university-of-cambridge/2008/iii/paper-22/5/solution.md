<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For each of the operators $D=d,\partial,\bar\partial,d^c$, define its nonnegative [Laplacian](../../../../../laplacian.md) by $\Delta_D=DD^*+D^*D$ using the $L^2$ [formal adjoint](../../../../../formal-adjoint.md). In particular, $\Delta=dd^*+d^*d$, $\Delta_\partial=\partial\partial^*+\partial^*\partial$, $\Delta_{\bar\partial}=\bar\partial\bar\partial^*+\bar\partial^*\bar\partial$, and $\Delta^c=d^c(d^c)^*+(d^c)^*d^c$. Use the [d c operator](../../../../../d-c-operator.md) convention

$$
d^c=i(\bar\partial-\partial),\qquad dd^c=2i\partial\bar\partial.
$$

This normalization, without an extra factor of one-half, is the one for which the requested equality with $\Delta^c$ holds.

The [Lefschetz operator of a Kähler manifold](../../../../../lefschetz-operator-of-a-kahler-manifold.md) is $L\alpha=\omega\wedge\alpha$, and the [adjoint Lefschetz operator](../../../../../adjoint-lefschetz-operator.md) is its pointwise metric adjoint $\Lambda=L^*$. It lowers type by $(1,1)$ and is a real operator because $\omega$ and the metric are real. Write $P=\partial$ and $B=\bar\partial$, use $[A,D]=AD-DA$, and use $\{A,D\}=AD+DA$ for the anticommutators of the odd-degree operators. The allowed relation among the [Kähler identities](../../../../../kahler-identities.md) and its complex conjugate give

$$
[\Lambda,P]=iB^*,\qquad
[\Lambda,B]=-iP^*,\qquad
B^*=-i[\Lambda,P],\quad P^*=i[\Lambda,B].
$$

These identities alone suffice for the calculation. Since $P^2=B^2=0$,

$$
\{P,B^*\}=-i\{P,[\Lambda,P]\}
=-i(P\Lambda P-P^2\Lambda+\Lambda P^2-P\Lambda P)=0.
$$

Replacing $P$ by $B$ in the same calculation gives $\{B,P^*\}=0$. Thus both mixed terms vanish when expanding the [Hodge Laplacian](../../../../../hodge-laplacian.md) of $d=P+B$:

$$
\Delta=\Delta_P+\Delta_B.
$$

The anticommutation $PB=-BP$ now proves equality of the two summands. Indeed,

$$
\begin{aligned}
\Delta_B&=-i\{B,[\Lambda,P]\}
=-i(B\Lambda P+PB\Lambda+\Lambda PB-P\Lambda B),\\
\Delta_P&=i\{P,[\Lambda,B]\}
=i(P\Lambda B-PB\Lambda-\Lambda PB-B\Lambda P),
\end{aligned}
$$

which are the same expression. Finally, $(d^c)^*=i(P^*-B^*)$, so its [Laplacian](../../../../../laplacian.md) expands as

$$
\Delta^c=\Delta_B+\Delta_P-\{B,P^*\}-\{P,B^*\}=\Delta_B+\Delta_P.
$$

This proves the [Kähler Laplacian identity](../../../../../kahler-laplacian-identity.md), with its real-operator version included:

$$
\boxed{\Delta=2\Delta_{\bar\partial}=2\Delta_\partial=\Delta^c.}
$$

The action of the [almost complex structure](../../../../../almost-complex-manifold.md) on forms is $J\alpha(v_1,\ldots,v_k)=\alpha(Jv_1,\ldots,Jv_k)$. It multiplies a form of type $(p,q)$ by $i^{p-q}$. Since $\Delta=2\Delta_{\bar\partial}$ preserves each bidegree, it commutes with this action of $J$. Thus $\Delta(J\alpha)=J(\Delta\alpha)$; the invertibility of $J$ gives

$$
\boxed{\Delta\alpha=0\quad\Longleftrightarrow\quad\Delta(J\alpha)=0.}
$$

This argument applies to arbitrary sums of types, not only to pure-type forms.

The [ddbar lemma](../../../../../ddbar-lemma.md) for a compact [Kähler manifold](../../../../../kahler-manifold.md) states that a $d$-closed form of pure type is $\partial\bar\partial$-exact if it is $d$-exact, $\partial$-exact, or $\bar\partial$-exact. Conversely, a $\partial\bar\partial$-exact form is $d$-closed and exact for all three operators. In particular a $d$-exact, $d$-closed $(p,q)$-form equals $\partial\bar\partial\beta$ for a form $\beta$ of type $(p-1,q-1)$.

The difference $\gamma=\widetilde\omega-\omega$ of the two [Kähler forms](../../../../../kahler-form.md) is a real $(1,1)$-form, is $d$-closed, and is $d$-exact by equality of their [de Rham cohomology](../../../../../de-rham-cohomology.md) classes. The [ddbar lemma](../../../../../ddbar-lemma.md) therefore gives a smooth complex-valued function $h$ with $\gamma=\partial\bar\partial h$. Reality and anticommutation imply

$$
\gamma=\bar\gamma
=\bar\partial\partial\bar h=-\partial\bar\partial\bar h.
$$

Set $f=(h-\bar h)/(2i)$, which is real. It follows directly that $i\partial\bar\partial f=\gamma$, giving the [global potential for cohomologous Kähler forms](../../../../../global-potential-for-cohomologous-kahler-forms.md)

$$
\boxed{\widetilde\omega=\omega+i\partial\bar\partial f,\qquad f\in C^\infty(X,\mathbb R).}
$$

If $f_1,f_2$ are two real potentials, $u=f_1-f_2$ satisfies $\partial\bar\partial u=0$, so it is a [pluriharmonic function](../../../../../pluriharmonic-function.md). The allowed relation among the [Kähler identities](../../../../../kahler-identities.md) gives $\bar\partial^*\bar\partial u=-i[\Lambda,\partial]\bar\partial u=-i\Lambda\partial\bar\partial u=0$, because $\Lambda\bar\partial u=0$ by degree. The [Kähler Laplacian identity](../../../../../kahler-laplacian-identity.md) then gives $\Delta u=2\bar\partial^*\bar\partial u=0$. Integration by parts on compact $X$ gives

$$
0=\langle\Delta u,u\rangle_{L^2}=\|du\|_{L^2}^2,
$$

so $u$ is constant on each connected component. Consequently **the potential is unique up to one additive constant when $X$ is connected; on a disconnected $X$, one constant per component is the exact conclusion**. Without the usual connectedness convention the printed uniqueness assertion needs this qualification: distinct constants on the components of a disjoint union leave the same pair of [Kähler forms](../../../../../kahler-form.md) unchanged.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
