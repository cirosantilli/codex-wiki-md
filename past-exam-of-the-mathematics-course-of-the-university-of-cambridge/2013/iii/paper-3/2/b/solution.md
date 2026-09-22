<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Here is the [double-coset criterion for a one-point extension](../../../../../../double-coset-criterion-for-a-one-point-extension.md). Let $H=G_\alpha$, and suppose $x$ swaps $\omega$ and $\alpha$. Then $\langle G,x\rangle$ is a one-point extension if and only if

$$
\boxed{x^2\in H,\qquad xHx^{-1}=H,\qquad xgx\in GxG\ \text{for every }g\in G\setminus H.}
$$

For necessity, in an extension $H$ fixes both $\omega$ and $\alpha$, so $x$ normalizes it and $x^2$ lies in it. Since $G$ is transitive on $\Omega$, the extension has exactly two [double cosets](../../../../../../double-coset.md) relative to $G$: $G$ and $GxG$. For $g\notin H$, $xgx$ moves $\omega$ into $\Omega$ and is in the latter [double coset](../../../../../../double-coset.md).

For sufficiency, the displayed conditions make $G\cup GxG$ closed under multiplication. Products with middle element in $H$ reduce using $xhx=(xhx^{-1})x^2\in G$; those with middle element outside $H$ remain in $GxG$. A finite nonempty multiplication-closed set of permutations containing the identity is a group. It contains $G$ and $x$, hence equals $\langle G,x\rangle$. Every element in $GxG$ moves $\omega$, while $G$ fixes it, giving the required [stabilizer subgroup](../../../../../../stabilizer-subgroup.md). The group is transitive because $G$ is transitive on $\Omega$ and $x$ moves the additional point.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
