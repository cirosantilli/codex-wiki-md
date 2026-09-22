# Reciprocal-root three-step multistep family

↑ **Parent:** [Linear multistep method](linear-multistep-method.md)

Take $\sigma(\zeta)=\zeta[(5+\alpha)\zeta^2-(4+8\alpha)\zeta+11-5\alpha]/6$. The [root condition for a multistep method](root-condition-for-a-multistep-method.md) holds exactly for $-1<\alpha<1$. Since $\rho'(1)=\sigma(1)=2(1-\alpha)$, these and only these parameters give a convergent method. Its [exponential-symbol order criterion for a multistep method](exponential-symbol-order-criterion-for-a-multistep-method.md) has defect $-(\alpha+5)z^4/12+O(z^5)$, giving formal order three except at $\alpha=-5$, where the first defect is $z^5/10$. None of the convergent family is [A-stable](a-stability.md): for a parasitic root $r=\alpha+i\sqrt{1-\alpha^2}$, perturbation of $\rho(r(z))-z\sigma(r(z))=0$ gives $\operatorname{Re}[r'(0)/r]=(\alpha-1)/12<0$. A small negative real $z$ therefore moves it outside the unit disk. At $\alpha=1$, cancellation would remove a double unit root, but the original recurrence retains that unstable parasitic behavior; it is not legitimately replaced by the reduced Backward Euler recurrence for arbitrary starting values.

## ↑ Ancestors (6)

1. [Linear multistep method](linear-multistep-method.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-57/6/solution.md)
