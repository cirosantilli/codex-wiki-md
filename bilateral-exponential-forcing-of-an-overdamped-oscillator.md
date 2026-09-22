# Bilateral exponential forcing of an overdamped oscillator

↑ **Parent:** [Causal Green function of an overdamped oscillator](causal-green-function-of-an-overdamped-oscillator.md)

For $a>b>0$ with $a,b\ne1$, the solution of $(D_t+a)(D_t+b)y=e^{-|t|}$ that decays at both infinities is

$$
y(t)=\begin{cases}
\dfrac{e^t}{(a+1)(b+1)},&t\leq0,\\
\dfrac{e^{-t}}{(a-1)(b-1)}+\dfrac2{a-b}\left(\dfrac{e^{-at}}{a^2-1}-\dfrac{e^{-bt}}{b^2-1}\right),&t\geq0.
\end{cases}
$$

Its [Fourier transform](fourier-transform-split.md) is $2/[(1+k^2)(a+ik)(b+ik)]$. The lower half-plane contains only the [pole](pole.md) $-i$, while the upper half-plane contains $i,ia,ib$. Inverting by the [residue theorem](residue-theorem.md) gives the two expressions. Direct substitution verifies the equation separately on each side, and $y,y'$ match at zero, so there is no spurious impulsive source. The negative-time response is nonzero because the forcing already acts before zero, even though the [Green function](green-s-function-split.md) is causal. Coinciding rates $a=1$ or $b=1$ require limits with polynomial times exponential terms.

## ↑ Ancestors (6)

1. [Causal Green function of an overdamped oscillator](causal-green-function-of-an-overdamped-oscillator.md)
2. [Damped harmonic oscillator](damped-harmonic-oscillator.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-2/5/solution.md)
