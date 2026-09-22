# Lee interpolation identity

↑ **Parent:** [B-spline](b-spline.md)

For distinct increasing knots, let $\ell_i(\cdot,t)$ interpolate $(\cdot-t)_+^{k-1}$ on $t_i,\ldots,t_{i+k-1}$ and let $\omega_i(x)=\prod_{r=1}^{k-1}(x-t_{i+r})$. Adjacent interpolants share $k-1$ values; their difference is a multiple of $\omega_i$. Its leading coefficient, by the [divided difference](divided-difference.md) recurrence, is the order-$k$ [B-spline](b-spline.md) $N_i(t)$. Thus $\ell_{i+1}(x,t)-\ell_i(x,t)=\omega_i(x)N_i(t)$. Telescoping proves the [Marsden identity](marsden-identity.md). Repeated knots require the well-defined confluent or limiting convention.

## ↑ Ancestors (8)

1. [B-spline](b-spline.md)
2. [Spline approximation](spline-approximation.md)
3. [Spline (mathematics)](spline-mathematics.md)
4. [Uniform approximation](uniform-approximation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-61/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-68/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-69/5/a/solution.md)
