# Black-Scholes reflection symmetry

↑ **Parent:** [Black-Scholes equation](black-scholes-equation.md)

For the dividend-free [Black-Scholes equation](black-scholes-equation.md), the displayed transform preserves solutions when $B>0$ and $\sigma>0$. Put $x=\log(S/B)$ and $v(x,t)=V(Be^x,t)$. The equation becomes

$$
v_t+\tfrac12\sigma^2v_{xx}+b v_x-rv=0,\qquad b=r-\sigma^2/2.
$$

Substitution shows that $\widehat v(x,t)=e^{qx}v(-x,t)$ solves the same equation when $q=-2b/\sigma^2=1-2r/\sigma^2$: its first-derivative coefficient becomes $-\sigma^2q-b=b$, and the additional zeroth-order term $\sigma^2q^2/2+bq$ vanishes. Subtracting the reflected solution enforces a zero boundary value at $S=B$. Its use in a killed [barrier option](barrier-option.md) is restricted to the alive side of the barrier; the algebraic extension to the other side is generally not a valid price.

## ↑ Ancestors (7)

1. [Black-Scholes equation](black-scholes-equation.md)
2. [Black-Scholes model](black-scholes-model.md)
3. [Mathematical finance](mathematical-finance-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Down-and-out put](down-and-out-put.md)
- [Solution](past-exam-of-the-mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford/2015/3/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford/2015/3/b/iv/solution.md)
- [Solution](past-exam-of-the-mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford/2017/2/c/solution.md)
- [Solution](past-exam-of-the-mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford/2021/3/a/iii/solution.md)
- [Up-and-out digital put](up-and-out-digital-put.md)
