# Cubic eighth-moment proof by differencing

↑ **Parent:** [Hua's lemma](hua-s-lemma.md)

Write $S(\theta)=\sum_{x\le n}e(\theta x^3)$ and $I_j=\int_0^1|S|^j$. [Character orthogonality](character-orthogonality.md) gives $I_2=n$. For $I_4$, fix the difference $D=x^3-y^3$. If $D=0$, there are $n^2$ choices for the two equal pairs. If $D\ne0$, any solution $z^3-w^3=D$ has $z-w\mid D$; fixing this divisor gives a quadratic equation for $w$, hence at most two choices. The [subpower bound for the divisor function](subpower-bound-for-the-divisor-function.md) yields $I_4\ll_\eta n^{2+\eta}$.

The twice-differenced inequality in [Weyl differencing](weyl-differencing.md) reads $|S|^4\le2n\sum_v c_ve(\theta v)$, with $c_v$ counting triples $(h,l,x)$ for which $v=3hl(2x+h+l)$ and all four shifted arguments are in $[1,n]$. Thus $c_0\ll n^2$, and $c_v\ll_\eta n^\eta$ for $v\ne0$: the product $hl$ divides $v$, and the remaining equation determines $x$. The [Fourier coefficients](fourier-coefficient.md) $r(v)$ of $|S|^4$ are nonnegative counts, with $r(0)=I_4$ and $\sum_vr(v)=n^4$. Multiply the inequality by $|S|^4$ and integrate. It follows that $I_8\ll n(n^2I_4+n^\eta n^4)\ll_\eta n^{5+\eta}$, after choosing the divisor-bound exponents small enough.

## ↑ Ancestors (8)

1. [Hua's lemma](hua-s-lemma.md)
2. [Weyl differencing](weyl-differencing.md)
3. [Exponential sum](exponential-sum.md)
4. [Analytic number theory](analytic-number-theory-split.md)
5. [Number theory](number-theory-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-30/5/solution.md)
