# Annular harmonic interpolation factor

↑ **Parent:** [Harmonic function](harmonic-function.md)

For an [annulus](annulus-mathematics.md) $a<r<1$ with $0<a<1$, these factors interpolate the two boundary coefficients of a [Fourier harmonic](fourier-harmonic.md) of positive [integer](integer-split.md) order $n$ in a [harmonic function](harmonic-function.md). They obey $H_n(1)=1$, $H_n(a)=0$, $K_n(1)=0$, $K_n(a)=1$. Thus a mode with outer coefficient $v$ and inner coefficient $w$ has radial factor $vH_n+wK_n$.

To derive them, [separation of variables](separation-of-variables.md) in [Laplace's equation](laplace-equation.md) in [polar coordinates](polar-coordinates.md) gives $r^2R''+rR'-n^2R=0$, whose solutions are $r^n,r^{-n}$. Imposing the two [Dirichlet boundary conditions](dirichlet-boundary-condition.md) on $R=\alpha r^n+\beta r^{-n}$ gives $\alpha+\beta=v$ and $a^n\alpha+a^{-n}\beta=w$. Solving yields $\alpha=(v-a^nw)/(1-a^{2n})$ and $\beta=a^n(w-a^nv)/(1-a^{2n})$, proving the formula. For the zero angular mode, the analogous factor is $v+(w-v)\log r/\log a$, since its radial solutions are $1$ and the [logarithm](logarithm.md) $\log r$.

## ↑ Ancestors (6)

1. [Harmonic function](harmonic-function.md)
2. [Partial differential equation](partial-differential-equation-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2021/prelims/mathematics-v-resit/question-5/a/solution.md)
