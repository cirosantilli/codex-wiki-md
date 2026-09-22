<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the continuous representative of $\bar u$ furnished by the one-dimensional [Sobolev embedding theorem](../../../../../sobolev-embedding-theorem.md), and define $u^*(x)=\bar u(|x|)$ on $A$. The [one-dimensional Sobolev representative](../../../../../one-dimensional-sobolev-representative.md) is absolutely continuous; [Holder inequality](../../../../../holder-inequality.md) applied to its [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) gives

$$
|\bar u(r)-\bar u(s)|
=\left|\int_s^r\bar u'(t)\,dt\right|
\leq |r-s|^{5/6}\|\bar u'\|_{L^6(1,2)}.
$$

Also $\|\bar u\|_\infty\leq\|\bar u\|_6+\|\bar u'\|_6$: select a point where $|\bar u|$ is no larger than its $L^6$ [norm](../../../../../norm.md) on the unit-length interval and apply the same [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md). Thus the one-dimensional [Hölder norm](../../../../../holder-norm.md) is controlled by $\|\bar u\|_{W^{1,6}(1,2)}$.

The two [Hölder seminorms](../../../../../holder-seminorm.md) must be compared using the correct distances. By the [reverse triangle inequality](../../../../../reverse-triangle-inequality.md),

$$
\frac{|u^*(x)-u^*(y)|}{|x-y|^{5/6}}
\leq[\bar u]_{C^{0,5/6}(1,2)}
\frac{\bigl||x|-|y|\bigr|^{5/6}}{|x-y|^{5/6}}
\leq[\bar u]_{C^{0,5/6}(1,2)}.
$$

Conversely, take $x=re$ and $y=se$ for any fixed unit vector $e$. Then $|x-y|=|r-s|$, so taking suprema yields equality of the two [Hölder seminorms](../../../../../holder-seminorm.md). Their [supremum norms](../../../../../supremum-norm.md) are equal as well. Part (i) now gives

$$
\boxed{\|u^*\|_{C^{0,5/6}(A)}
=\|\bar u\|_{C^{0,5/6}(1,2)}
\leq C\|\bar u\|_{W^{1,6}(1,2)}
\leq C'\|u\|_{W^{1,6}(A)}.}
$$

The representative agrees with $u$ [almost everywhere](../../../../../almost-everywhere.md), and the assignment is linear and injective on the radial [Sobolev space](../../../../../sobolev-space-split.md). This proves the requested [continuous embedding](../../../../../continuous-embedding.md). The inner radius being positive makes the [radial profile](../../../../../radial-profile.md) [Sobolev norm](../../../../../sobolev-norm.md) comparable to its weighted radial version.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the functional analytic methods for partial differential equations course of the University of Oxford](../../../../split.md)
6. [Functional analytic methods for partial differential equations course of the University of Oxford](../../../../../functional-analytic-methods-for-partial-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
