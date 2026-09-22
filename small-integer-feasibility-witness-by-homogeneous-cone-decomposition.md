# Small integer feasibility witness by homogeneous cone decomposition

↑ **Parent:** [Integer programming](integer-programming.md)

If $Bz=b$, $z\geq0$ has an integer solution, with $N$ variables and all data bounded by $M\geq1$, it has one satisfying the displayed bound. Apply [support-minimal rays of a nonnegative kernel](support-minimal-rays-of-a-nonnegative-kernel.md) to $(z,1)$ in the cone $\{(u,t)\geq0:Bu=bt\}$. Its integer generators have coordinates bounded by $D=(N+1)!M^{N+1}$. Generators with positive last coordinate normalize to feasible points with coordinates at most $D$; their coefficients form a convex combination. The remaining generators are integer recession directions. Subtract the integer parts of their coefficients from the original integer solution. The result remains integral and feasible and has coordinates at most $D+(N+1)D$. Its binary length is polynomial in the input size. Splitting unrestricted integer variables and adding integer slacks reduces general integer linear feasibility to this form, proving its membership in [NP](np-complexity.md).

## ↑ Ancestors (5)

1. [Integer programming](integer-programming.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-40/2/solution.md)
