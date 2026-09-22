<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $\mathfrak c=2^{\aleph_0}$ and enumerate all nonidentity [order automorphisms](../../../../../../../order-automorphism.md) of the real line as $\langle h_\alpha:\alpha<\mathfrak c\rangle$. We construct sets of points to include and exclude, starting with $I_0=\mathbb Q$ and $E_0=\varnothing$.

At stage $\alpha$, each of $I_\alpha,E_\alpha$ has [cardinality](../../../../../../../cardinality.md) less than $\mathfrak c$. Since $h_\alpha$ is a nonidentity increasing bijection, its moved points contain a nonempty open interval. Indeed if $h_\alpha(u)>u$, points between $u$ and $h_\alpha(u)$ are moved; the other direction is similar. There are therefore $\mathfrak c$ moved points. Choose one, $x_\alpha$, outside

$$
I_\alpha\cup E_\alpha\cup h_\alpha^{-1}[I_\alpha\cup E_\alpha].
$$

Then put $x_\alpha$ into $I$ and $h_\alpha(x_\alpha)$ into $E$. They are different, and the included and excluded sets remain disjoint. Take unions at limit stages. This recursion works even when $\mathfrak c$ is singular: before stage $\alpha$, only countably many initial points and at most $|\alpha|$ chosen pairs have been used.

Let $X=\mathbb Q\cup\{x_\alpha:\alpha<\mathfrak c\}$. It is an [order-dense subset](../../../../../../../order-dense-subset.md) of [cardinality](../../../../../../../cardinality.md) $\mathfrak c$. Any nonidentity [order automorphism](../../../../../../../order-automorphism.md) of $X$ extends uniquely to some $h_\alpha$ of $\mathbb R$, but its value at $x_\alpha\in X$ is the excluded point $h_\alpha(x_\alpha)\notin X$, a contradiction. Thus **the resulting [rigid dense subset of the real line](../../../../../../../rigid-dense-subset-of-the-real-line.md) satisfies**

$$
\boxed{|X|=\mathfrak c,\qquad\operatorname{Aut}(X,<)=\{\mathrm{id}\}.}
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 24](../../../../paper-24-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
