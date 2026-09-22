<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

An [Aronszajn tree](../../../../../aronszajn-tree.md) is a [set-theoretic tree](../../../../../set-theoretic-tree.md) of height $\omega_1$, with [countable](../../../../../countable-set.md) levels and no [uncountable](../../../../../uncountable-set.md) [chain in a partial order](../../../../../chain-in-a-partial-order.md), equivalently no [cofinal branch](../../../../../cofinal-branch.md). The strict predecessors of a node are well-ordered, and its height is their [order type](../../../../../order-type.md). **Such trees exist in ZFC**, as the following [rationally labelled Aronszajn tree construction](../../../../../rationally-labelled-aronszajn-tree-construction.md) shows.

We build [countable](../../../../../countable-set.md) nonempty levels $T_\alpha$ for all $\alpha<\omega_1$. A node $t\in T_\alpha$ is a strictly increasing function $t:\alpha\to\mathbb Q\cap(0,1)$, and the tree order is proper initial-segment extension. Every restriction $t\upharpoonright\beta$ must lie in $T_\beta$. Give nonempty $t$ the rational label

$$
\ell(t)=\sup\operatorname{ran}(t)<1,
$$

and give the empty root label $0$. We require labels to increase strictly along the tree. We also maintain the [bounded rational extension property](../../../../../bounded-rational-extension-property.md):

$$
s\in T_\beta,\quad \beta<\alpha,\quad
\ell(s)<q<1,\ q\in\mathbb Q
\quad\Longrightarrow\quad
(\exists t\in T_\alpha)\ s\subset t,\ \ell(t)<q.
$$

Keeping room below every rational cap is what makes the limit step possible.

Start with $T_0=\{\varnothing\}$. At a successor stage, for every $s\in T_\alpha$ and every rational $r$ with $\ell(s)<r<1$, include

$$
s^\frown r=s\cup\{(\alpha,r)\}
$$

in $T_{\alpha+1}$. Its label is $r$, strictly larger than its predecessor's. This level is [countable](../../../../../countable-set.md). To extend an earlier node below a prescribed cap $q$, first extend to $T_\alpha$ below $q$ by the inductive property, if necessary, then choose a new rational label between that label and $q$. Thus the extension property is preserved.

Now let $\lambda<\omega_1$ be a nonzero limit. The whole tree below $\lambda$ is [countable](../../../../../countable-set.md). For each pair $(s,q)$ with $s\in T_\beta$, $\beta<\lambda$, and $\ell(s)<q<1$, construct one node at height $\lambda$ extending $s$ below $q$. There are only countably many such pairs.

Choose a rational $r$ with $\ell(s)<r<q$ and an increasing sequence

$$
\beta=\alpha_0<\alpha_1<\cdots<\lambda,\qquad
\sup_n\alpha_n=\lambda.
$$

Set $s_0=s$. Given $s_n\in T_{\alpha_n}$ with $\ell(s_n)<r$, set

$$
r_n=\frac{r+\max\{\ell(s_n),\,r-1/(n+1)\}}2.
$$

This is rational and satisfies $\max\{\ell(s_n),r-1/(n+1)\}<r_n<r$. The successor rule supplies $u_n=s_n^\frown r_n$ at height $\alpha_n+1$. If $\alpha_{n+1}=\alpha_n+1$, take $s_{n+1}=u_n$; otherwise use the already established extension property below $\lambda$ to extend $u_n$ to $s_{n+1}\in T_{\alpha_{n+1}}$ with label below $r$.

The union $t=\bigcup_n s_n$ has domain $\lambda$ and extends $s$. It is strictly increasing, and every shorter restriction is already in its prescribed level. All its values are below $r$, while it contains the values $r_n>r-1/(n+1)$. Hence

$$
\sup\operatorname{ran}(t)=r\in\mathbb Q,\qquad \ell(t)=r<q.
$$

Every predecessor's label is below the label of some $s_n$, and hence below $r$. Thus strict increase of labels survives at the limit. Include one such $t$ for each pair $(s,q)$ in $T_\lambda$, discarding duplicates. This gives a [countable](../../../../../countable-set.md) level and preserves every bounded extension requirement. In particular applying it to the root makes the level nonempty. The choices here are permitted by the ambient [axiom of choice](../../../../../axiom-of-choice.md); [transfinite recursion](../../../../../transfinite-recursion.md) through the set $\omega_1$ completes the construction.

Put $T=\bigcup_{\alpha<\omega_1}T_\alpha$. A node of domain $\alpha$ has exactly the restrictions of domains $\beta<\alpha$ as predecessors, so its height is $\alpha$. Therefore $T$ has height $\omega_1$ and [countable](../../../../../countable-set.md) levels. Since $\ell:T\to\mathbb Q$ is strictly increasing on comparable nodes, an [uncountable](../../../../../uncountable-set.md) chain would inject into the [countable](../../../../../countable-set.md) set $\mathbb Q$, which is impossible. Each label fiber is a [tree antichain](../../../../../tree-antichain.md), so the tree is even a [special Aronszajn tree](../../../../../special-aronszajn-tree.md):

$$
\boxed{\text{ZFC proves the existence of a special Aronszajn tree}.}
$$

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 83](../../paper-83-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
