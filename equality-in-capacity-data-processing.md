# Equality in capacity data processing

↑ **Parent:** [Channel capacity](channel-capacity.md)

For a finite [discrete memoryless channel](discrete-memoryless-channel.md) and a deterministic output map $T=g(Y)$, the [data processing inequality](data-processing-inequality.md) gives $C_T\leq C_Y$. Equality holds exactly when an original capacity-achieving input law satisfies $I(X;Y\mid T)=0$. Sufficiency follows from the gap identity $I(X;Y)=I(X;T)+I(X;Y\mid T)$. For necessity, take an input law maximizing $I(X;T)$. If this maximum is $C_Y$, both inequalities $I(X;T)\leq I(X;Y)\leq C_Y$ are equalities at that law. [Injectivity](injective-function.md) of $g$ on reachable outputs is a sufficient condition, since $T$ then determines $Y$; it is unnecessary if the discarded distinctions convey no further information about $X$ at some maximizing input law.

## ↑ Ancestors (6)

1. [Channel capacity](channel-capacity.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-information-theory-course-of-the-university-of-oxford/2021/3/b/solution.md)
