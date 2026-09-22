# Radial Sobolev profile on an annulus

↑ **Parent:** [Sobolev space](sobolev-space-split.md)

Let $0<a<b<\infty$ and $1\leq p<\infty$. A [radial function](radial-function.md) in $W^{1,p}(\{a<|x|<b\})$ has a [radial profile](radial-profile.md) in $W^{1,p}(a,b)$; its first [weak derivative](weak-derivative.md) is the profile of the [radial derivative](radial-derivative.md). To see the identity, sum the [weak derivative](weak-derivative.md) tests against the components of $\phi(r)x/r$ to obtain $\int g\phi r^{n-1}=-\int\bar u(\phi r^{n-1})'$. Substitute $\phi=\zeta/r^{n-1}$ for arbitrary $\zeta\in C_c^\infty(a,b)$. The weighted [Lp norms](lp-norm.md) and $a>0$ give the displayed bound. Radiality of the [radial derivative](radial-derivative.md) follows by applying a rotation to the [weak derivative](weak-derivative.md) identity: if $u(Qx)=u(x)$, then $\nabla u(Qx)=Q\nabla u(x)$ [almost everywhere](almost-everywhere.md), so the radial scalar product is invariant.

For $p>1$, the [one-dimensional Sobolev representative](one-dimensional-sobolev-representative.md) obeys $|\bar u(r)-\bar u(s)|\leq|r-s|^{1-1/p}\|\bar u'\|_p$. The [reverse triangle inequality](reverse-triangle-inequality.md) transfers this to $u$, giving a [continuous embedding](continuous-embedding.md) of this radial [Sobolev space](sobolev-space-split.md) into $C^{0,1-1/p}$ on the [annulus](annulus-mathematics.md). The two [Hölder seminorms](holder-seminorm.md) are equal: one inequality follows from $\bigl||x|-|y|\bigr|\leq|x-y|$, and the reverse follows by putting both points on the same ray. The restriction $a>0$ is essential for the unweighted profile bound.

## ↑ Ancestors (6)

1. [Sobolev space](sobolev-space-split.md)
2. [Functional analysis](functional-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-functional-analytic-methods-for-partial-differential-equations-course-of-the-university-of-oxford/2023/1/c/i/solution.md)
