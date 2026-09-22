# Residual-preserving clipping of an ROF minimizer

↑ **Parent:** [Total variation denoising](total-variation-denoising.md)

If $u$ minimizes scalar [total variation denoising](total-variation-denoising.md) with $f\in BV\cap L^2$, set $w=T_Mu$, $r=u-w$ and $g=f-r$. The [scalar total variation splitting under clipping](scalar-total-variation-splitting-under-clipping.md) gives $\operatorname{TV}(u)=\operatorname{TV}(w)+\operatorname{TV}(r)$. Compare $u$ with $v+r$ and use $\operatorname{TV}(v+r)\le\operatorname{TV}(v)+\operatorname{TV}(r)$; cancelling the tail shows that $w$ minimizes the same model for $g$. It is bounded while $g$ may be unbounded, and $w-g=u-f$ exactly. This reduction concerns the actual [minimizer](global-minimizer.md), rather than convergence of [minimizers](global-minimizer.md) for truncated data.

## ↑ Ancestors (9)

1. [Total variation denoising](total-variation-denoising.md)
2. [Total variation seminorm on a domain](total-variation-seminorm-on-a-domain.md)
3. [Variational regularization](variational-regularization.md)
4. [Regularization of an inverse problem](regularization-of-an-inverse-problem.md)
5. [Inverse problem](inverse-problem-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Jump-amplitude inequality for total variation denoising](jump-amplitude-inequality-for-total-variation-denoising.md)
- [No-new-jumps property of total variation denoising](no-new-jumps-property-of-total-variation-denoising.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-64/2/iii/solution.md)
- [Scalar total variation splitting under clipping](scalar-total-variation-splitting-under-clipping.md)
