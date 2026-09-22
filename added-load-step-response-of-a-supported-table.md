# Added-load step response of a supported table

↑ **Parent:** [Step response of a damped oscillator](step-response-of-a-damped-oscillator.md)

Adding a load $M$ to a spring-supported table shifts its static downward position by $\Delta=Mg/k$. If the load is deposited with negligible impulse and moves with the table, the moving [mass](mass.md) is $m+M$. Starting at the former equilibrium with zero [velocity](velocity.md), an [underdamped](underdamping.md) response is

$$
x(t)=\Delta\left[1-e^{-\beta t}\left(\cos\omega_dt+\frac\beta{\omega_d}\sin\omega_dt\right)\right],\qquad
\beta=\frac{b}{2(m+M)},\quad \omega_d^2=\frac{k}{m+M}-\beta^2.
$$

Its transient envelope decays over $1/\beta$. [Critical damping](critical-damping.md) $b=2\sqrt{k(m+M)}$ gives $x=\Delta[1-(1+\omega_0t)e^{-\omega_0t}]$. A nonzero impact impulse changes the initial [velocity](velocity.md) and therefore the transient.

## ↑ Ancestors (7)

1. [Step response of a damped oscillator](step-response-of-a-damped-oscillator.md)
2. [Causal Green function of a damped oscillator](causal-green-function-of-a-damped-oscillator.md)
3. [Damped harmonic oscillator](damped-harmonic-oscillator.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Response to the added load](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-2/section-b/b6/response-to-the-added-load.md)
