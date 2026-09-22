<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $0<\alpha\le1$, uniform Lipschitz-$\alpha$ means that one constant $M$ satisfies $|f(x)-f(y)|\le M|x-y|^\alpha$ for every $x,y\in[0,1]$. The resulting [Hölder space](../../../../../../holder-space.md) has [norm](../../../../../../norm.md)

$$
\|f\|_{C^{0,\alpha}}=\|f\|_\infty+[f]_{C^{0,\alpha}},\qquad[f]_{C^{0,\alpha}}=\sup_{x\ne y}\frac{|f(x)-f(y)|}{|x-y|^\alpha}.
$$

For the subsequent estimates at general $\alpha>0$, use the higher-order [Hölder class](../../../../../../holder-class.md) convention: write $\alpha=r+\beta$ with $r\ge0$ an [integer](../../../../../../integer.md) and $0<\beta\le1$, and require $f\in C^r([0,1])$ with $f^{(r)}$ uniformly Lipschitz-$\beta$. Thus

$$
\boxed{C^\alpha=C^{r,\beta},\qquad\|f\|_{C^\alpha}=\sum_{k=0}^r\|f^{(k)}\|_\infty+[f^{(r)}]_{C^{0,\beta}}.}
$$

At [integer](../../../../../../integer.md) $\alpha=k$, this uses $C^{k-1,1}$; the alternative classical $C^k$ convention is stronger on this [compact](../../../../../../compact-space.md) [closed interval](../../../../../../closed-real-interval.md) and also suffices for the estimates.

**For exponents above one, a first-difference inequality alone forces the [function](../../../../../../function-split.md) to be constant.** Partition $[x,y]$ into $n$ equal pieces and use the [triangle inequality](../../../../../../triangle-inequality.md): $|f(y)-f(x)|\le M|y-x|^\alpha n^{1-\alpha}\to0$. Consequently a nontrivial higher-order definition is needed for the full range of exponents in the later [wavelet](../../../../../../wavelet.md) estimates. Equivalently, higher-order [Hölder class](../../../../../../holder-class.md) gives a local [Taylor polynomial](../../../../../../taylor-polynomial.md) with remainder bounded by $C\|f\|_{C^\alpha}|x-x_0|^\alpha$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
