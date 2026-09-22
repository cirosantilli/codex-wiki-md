<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [local operator](../../../../../lawvere-tierney-topology.md) is an inflationary, idempotent, finite-meet-preserving map $j:\Omega\to\Omega$ with $j(\top)=\top$, expressed in the [internal logic of a topos](../../../../../internal-logic-of-a-topos.md). For a [subterminal object](../../../../../subterminal-object.md) $U$ with truth value $u$, the [closed local operator](../../../../../closed-local-operator.md) and [quasi-closed local operator](../../../../../quasi-closed-local-operator.md) are respectively

$$
c(u)(p)=u\vee p,\qquad q(u)(p)=((p\Rightarrow u)\Rightarrow u).
$$

The first is a [local operator](../../../../../lawvere-tierney-topology.md) by distributivity. For the second put $n(p)=p\Rightarrow u$. Then $p\le n^2p$, $n$ is order-reversing, and $n^3p=np$: the first inequality gives $n^3p\le np$, while its application to $np$ gives the reverse inequality. Thus $q=n^2$ is inflationary and idempotent, and $q(\top)=\top$.

For meet preservation, monotonicity gives $q(p\wedge r)\le qp\wedge qr$. Conversely put $t=(p\wedge r)\Rightarrow u$. From $t\wedge p\le r\Rightarrow u$ and $qr\wedge(r\Rightarrow u)\le u$, we obtain $t\wedge qr\le p\Rightarrow u$. Intersecting with $qp$ gives $qp\wedge qr\wedge t\le u$, hence $qp\wedge qr\le q(p\wedge r)$. This proves all local-operator axioms. Also $q(u)(0)=u$ and $q(u)(u)=u$. Equivalently, it is the largest [local operator](../../../../../lawvere-tierney-topology.md) leaving $u$ fixed: if $k(u)=u$, then

$$
kp\wedge k(p\Rightarrow u)\le u\quad\Longrightarrow\quad kp\le k(p\Rightarrow u)\Rightarrow u\le(p\Rightarrow u)\Rightarrow u.
$$

This explains the quasi-closed terminology as relative double negation above the closed bottom $u$.

The [subobject classifier](../../../../../subobject-classifier.md) of $\mathbf{sh}_j(\mathcal E)$ is the [closed-subobject classifier](../../../../../closed-subobject-classifier.md) $\Omega_j=\{p:jp=p\}$. Its bottom is $j0$, its meet is inherited, its join is $j(p\vee r)$, and implication between closed truth values is the ambient implication. To verify the last claim, if $jv=v$, then

$$
j(p\Rightarrow v)\wedge jp=j((p\Rightarrow v)\wedge p)\le v.
$$

It follows that $j(p\Rightarrow v)\le jp\Rightarrow v\le p\Rightarrow v$; inflationarity gives equality and also $jp\Rightarrow v=p\Rightarrow v$.

Suppose $j=q(u)$. Every closed $p$ lies above $u$, and its complement in $\Omega_j$ is $np=p\Rightarrow u$, also closed because $n^3=n$. We have $p\wedge np=u$. Moreover $n(p\vee np)=np\wedge n^2p=np\wedge p=u$, so $q(p\vee np)=\top$. Thus the fixed truth values form a [Boolean algebra](../../../../../boolean-algebra.md), and the sheaf topos is a [Boolean topos](../../../../../boolean-topos.md).

Conversely suppose the sheaf topos is Boolean and put $u=j0$. Complementation in its classifier is $p\mapsto p\Rightarrow u$. Applying the double-complement identity to $jp$, and using the implication calculation above, gives

$$
jp=((jp\Rightarrow u)\Rightarrow u)=((p\Rightarrow u)\Rightarrow u).
$$

Therefore

$$
\boxed{\mathbf{sh}_j(\mathcal E)\text{ is Boolean}\iff j=q(j0).}
$$

For the cover, work in the [slice category](../../../../../slice-category.md) $\mathcal E/\Omega$. Its generic [subterminal object](../../../../../subterminal-object.md) is $T=(\top:1\hookrightarrow\Omega)$. Form its quasi-closed Boolean subtopos $\mathcal B=\mathbf{sh}_{q(T)}(\mathcal E/\Omega)$, and compose its embedding with the slice projection to obtain $b:\mathcal B\to\mathcal E$. The slice projection has inverse image $X\mapsto X\times\Omega$, and sheafification is left exact, so this is a [geometric morphism](../../../../../geometric-morphism.md).

To prove surjectivity, take a [monomorphism](../../../../../monomorphism.md) $S\hookrightarrow X$ with characteristic predicate $p(x)$, and suppose $b^*$ makes it invertible. Pullback to the slice followed by sheafification makes this exactly the assertion that it is $q(T)$-dense. Internally on $X\times\Omega$, therefore,

$$
((p(x)\Rightarrow u)\Rightarrow u)=\top
$$

for the generic truth value $u$. Substitute $u=p(x)$ by pulling back along the graph $X\to X\times\Omega$. The left side becomes $(\top\Rightarrow p(x))=p(x)$, so $p(x)=\top$ and the original mono is invertible. Thus $b^*$ reflects invertible monos. If it identifies two parallel arrows, their [equalizer](../../../../../equaliser.md) becomes invertible; reflection then shows the arrows were already equal. Hence $b^*$ is faithful, and

$$
\boxed{\mathbf{sh}_{q(T)}(\mathcal E/\Omega)\longrightarrow\mathcal E\text{ is a surjection from a Boolean topos}.}
$$

The generic truth value is essential: substituting only a fixed global value such as $0$ would give a Boolean subtopos, but need not give a surjection onto the original topos.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 24](../../paper-24-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
