# Derivative quotient limits on partial domains

↑ **Parent:** [L'Hôpital's rule](l-hopital-s-rule.md)

The usual zero-over-zero [L'Hopital rule](l-hopital-s-rule.md) requires the denominator's [derivative](derivative.md) to be nonzero throughout a sufficiently small deleted neighborhood. A limit taken only where that [derivative](derivative.md) is nonzero is insufficient. An explicit counterexample uses $x_n=2^{-n}$, $h_n=4^{-n}$, $S(u)=3u^2-2u^3$ and $q(u)=16u^2(1-u)^2$. On $[3x_n/4,x_n]$ put $g=h_n$ and $f=h_nq((x-3x_n/4)/(x_n/4))$. On $[x_n/2,3x_n/4]$ put $g=h_{n+1}+(h_n-h_{n+1})S((x-x_n/2)/(x_n/4))$ and $f=0$. Extend $g=1,f=0$ beyond one. Values and first [derivatives](derivative.md) agree at the joins, both functions tend to zero, and $g$ is positive. Where $g'\ne0$, it lies inside a transition interval and $f'=0$. Thus $f'/g'$ has natural-domain limit zero, but $f/g$ equals zero at $x_n$ and one at $7x_n/8$, so has no limit.

## ↑ Ancestors (8)

1. [L'Hôpital's rule](l-hopital-s-rule.md)
2. [Derivative](derivative.md)
3. [Calculus](calculus-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ia/paper-1/11d/solution.md)
