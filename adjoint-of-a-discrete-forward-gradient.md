# Adjoint of a discrete forward gradient

↑ **Parent:** [Forward difference operator](forward-difference-operator.md)

On an $N$-pixel line with last forward difference zero, $D^*p$ has first entry $-p_1$, interior entries $p_{i-1}-p_i$, and last entry $p_{N-1}$, with $D^*=0$ for $N=1$. On a square grid add these expressions along rows and columns. Unused last-edge components contribute nothing. The identity $\langle Du,p\rangle=\langle u,D^*p\rangle$ fixes every boundary sign. On the unscaled square grid, $\|D\|^2=8\cos^2(\pi/(2N))\le8$ for $N>1$.

## ↑ Ancestors (8)

1. [Forward difference operator](forward-difference-operator.md)
2. [Finite difference method](finite-difference-method.md)
3. [Finite difference](finite-difference-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-340/5/a/solution.md)
