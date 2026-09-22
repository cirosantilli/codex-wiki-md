# Sliding-window upper bound for Sidon sets

↑ **Parent:** [Sidon set](sidon-set.md)

For a [Sidon set](sidon-set.md) $A\subseteq[1,N]$, put $m=|A|$ and let $A_i$ count points in a window of $u$ consecutive integers. Each point occurs in $u$ windows, so $\sum A_i=um$. [Cauchy-Schwarz](cauchy-schwarz-inequality.md) gives $\sum\binom{A_i}2\geq[u^2m^2/(N+u)-um]/2$. Each positive difference occurs at most once and contributes $u-d$ windows, giving the upper bound $u(u-1)/2$. Thus $m^2\leq(N+u)(1+(m-1)/u)$. Taking $u=\lfloor N^{3/4}\rfloor$ gives the displayed estimate, which combines with the [Bose-Chowla Sidon construction](bose-chowla-sidon-construction.md) to determine the asymptotic maximum.

## ↑ Ancestors (6)

1. [Sidon set](sidon-set.md)
2. [Additive combinatorics](additive-combinatorics-split.md)
3. [Combinatorics](combinatorics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-7/6/ii/solution.md)
