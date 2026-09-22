# Square-root endpoint integrals by an upper-half-plane contour

↑ **Parent:** [Contour integration](contour-integration.md)

Let $a>0$ and let $R$ be a [rational function](rational-function.md) with $R(z^2)$ finite for real $z$ and $R(u)=O(u^{-1})$ at infinity. Choose the branch $h(z)=\sqrt{z^2-a^2}$ analytic off $[-a,a]$, with $h(z)\sim z$ at infinity. Put $g(z)=zR(z^2)/h(z)$. On the real exterior, $g(-x)=g(x)$; on the upper bank of the cut, $h(x+i0)=i\sqrt{a^2-x^2}$, so $g(x+i0)$ is odd in $x$.

Close a real-axis [contour](complex-integration-contour.md) with a large upper [semicircle](semicircle.md), making clockwise upper indentations at the two [branch points](branch-point.md). The large arc vanishes because $g=O(z^{-2})$. Each small indentation is $O(\sqrt\varepsilon)$ and vanishes. The integral along the upper bank of $[-a,a]$ is zero by oddness; the two exterior pieces sum to twice the required integral. The [residue theorem](residue-theorem.md) therefore gives

$$
\boxed{\int_a^\infty\frac{xR(x^2)}{\sqrt{x^2-a^2}}\,dx=\pi i\sum_{\operatorname{Im}z>0}\operatorname{Res}_z\frac{zR(z^2)}{\sqrt{z^2-a^2}}.}
$$

Residues must use the chosen branch, notably $h(iy)=i\sqrt{y^2+a^2}$ for $y>0$. The substitution $u=\sqrt{x^2-a^2}$ provides an independent real-variable check, converting the integral to $\int_0^\infty R(u^2+a^2)\,du$.

## ↑ Ancestors (6)

1. [Contour integration](contour-integration.md)
2. [Complex analysis](complex-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-2/4/b/ii/solution.md)
