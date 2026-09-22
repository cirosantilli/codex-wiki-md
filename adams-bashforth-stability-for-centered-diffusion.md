# Adams-Bashforth stability for centered diffusion

↑ **Parent:** [Adams-Bashforth method](adams-bashforth-method.md)

For centered-space diffusion, a [Fourier mode](fourier-mode.md) gives $z^2-(1-3a/2)z-a/2=0$, with $a=4\mu\sin^2(\theta/2)$. For $a>0$ the roots have opposite signs, the positive root lies in $(0,1)$, and the negative root lies in $[-1,0)$ exactly when $P(-1)=2-2a\geq0$. At $a=0,1$ the unit-modulus roots are simple. Hence the [root condition for a multistep method](root-condition-for-a-multistep-method.md) holds for every Fourier frequency exactly when $\mu\leq1/4$. Under fixed $\mu$, the unscaled one-step defect is $-\Delta t^2u_{xxxx}/(12\mu)+O(\Delta t^3)$; dividing by the step changes its order to $O(\Delta t)$.

## ↑ Ancestors (7)

1. [Adams-Bashforth method](adams-bashforth-method.md)
2. [Linear multistep method](linear-multistep-method.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-4/39c/b/solution.md)
