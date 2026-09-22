# Dirichlet Green function for a radial power operator on an interval

↑ **Parent:** [Dirichlet Green function](dirichlet-green-function.md)

Let $0<a<b$ and impose zero [Dirichlet boundary conditions](dirichlet-boundary-condition.md) at $a,b$. With the convention $L_xG(x,s)=\delta(x-s)$ for the [Dirac delta distribution](dirac-delta-function.md), the [Green's function](green-s-function-split.md) is continuous and its first [derivative](derivative.md) has jump one. For $n\ne0$ choose $\ell(x)=x^{-n}-a^{-n}$ and $r(x)=x^{-n}-b^{-n}$. Their [Wronskian](wronskian.md) is $n(a^{-n}-b^{-n})s^{-n-1}$, so

$$
G(x,s)=\frac{s^{n+1}(x_<^{-n}-a^{-n})(x_>^{-n}-b^{-n})}{n(a^{-n}-b^{-n})},\qquad x_<=\min(x,s),\quad x_>=\max(x,s).
$$

For $n=0$, take the continuous limit or use $\ell=\log(x/a)$ and $r=\log(x/b)$ to obtain

$$
G(x,s)=\frac{s\log(x_</a)\log(x_>/b)}{\log(b/a)}.
$$

The solution is $u(x)=\int_a^bG(x,s)f(s)\,ds$. These kernels use ordinary measure $ds$. The factor $s^{n+1}$ comes from the nonconstant [Wronskian](wronskian.md) and must not be discarded by confusing the original operator with its multiplied [divergence form](divergence-form.md) $(x^{n+1}u')'$.

## ↑ Ancestors (6)

1. [Dirichlet Green function](dirichlet-green-function.md)
2. [Green's function](green-s-function-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
