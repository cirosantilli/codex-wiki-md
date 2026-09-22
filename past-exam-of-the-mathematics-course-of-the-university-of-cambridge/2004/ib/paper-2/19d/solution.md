<h1 id="19d/solution">Solution</h1>

↑ **Parent:** [19D](../19d.md)

Take the [momentum operator](../../../../../momentum-operator.md) $p=-i\hbar\,d/dx$ and sufficiently regular real $f$. Acting on a test [wave function](../../../../../wave-function.md), the [commutator](../../../../../commutator.md) is $[p,f]=-i\hbar f'$. Expanding the [factorized quantum Hamiltonian](../../../../../factorized-quantum-hamiltonian.md) gives

$$
(p+if)(p-if)=p^2+f^2+i(fp-pf)=p^2+f^2-\hbar f',
$$

so **$V(x)=(f(x)^2-\hbar f'(x))/(2m)$**, which is real.

Set $Q=p-if$. Its zero-mode equation is

$$
Q\psi_0=0\quad\Longleftrightarrow\quad\hbar\psi_0'+f\psi_0=0,
$$

with solution

$$
\boxed{\psi_0(x)=C\exp\!\left[-\frac1\hbar\int_0^x f(t)\,dt\right].}
$$

It satisfies $H\psi_0=Q^\dagger Q\psi_0/(2m)=0$ as a differential equation. It is an actual quantum state only when it is square-integrable. If $f(x)=cx^n+\cdots$, $c\ne0$, its antiderivative has leading term $cx^{n+1}/(n+1)$. For even $n$, this leading term has opposite signs at the two ends of the line, so the [wave function](../../../../../wave-function.md) grows at one end and cannot be normalized. For odd $n$, it has the same sign at both ends. Hence **normalizability requires odd $n$, and in fact holds exactly when $n$ is odd and $c>0$**. A negative leading coefficient makes it grow at both ends; $f=0$ gives a nonnormalizable constant. These are the [normalizable zero mode of a polynomial factorized Hamiltonian](../../../../../normalizable-zero-mode-of-a-polynomial-factorized-hamiltonian.md) conditions.

For a normalized state in the [operator domain](../../../../../operator-domain.md), integration by parts, with the appropriate vanishing boundary term, gives

$$
\langle\psi,H\psi\rangle=\frac1{2m}\int_{\mathbb R}|Q\psi|^2\,dx\geq0.
$$

Thus every [energy eigenvalue](../../../../../energy-eigenvalue.md) is nonnegative. Equality forces $Q\psi=0$ almost everywhere, whose first-order equation has the one-dimensional solution space above. Whenever its zero mode is normalizable, **every [energy eigenstate](../../../../../energy-eigenstate.md) not proportional to $\psi_0$ has strictly positive energy**. If the formal zero mode is not normalizable, there is no zero-energy eigenstate; the positivity statement still applies to every normalizable eigenstate. This argument concerns eigenvalues and does not assert a strictly positive bound on an arbitrary continuous spectrum.

For the [quantum harmonic oscillator](../../../../../quantum-harmonic-oscillator.md), take $f(x)=m\omega x$ with $m,\omega>0$. Then

$$
H=\frac{p^2}{2m}+\frac12m\omega^2x^2-\frac12\hbar\omega
=H_{\mathrm{osc}}-\frac12\hbar\omega.
$$

Its zero mode is normalizable and has no competitor of lower energy. Using the [Gaussian integral](../../../../../gaussian-integral.md) for its normalization gives the concise answer

$$
\boxed{E_{\min}=\frac12\hbar\omega,\qquad
\psi_{\min}(x)=\left(\frac{m\omega}{\pi\hbar}\right)^{1/4}e^{-m\omega x^2/(2\hbar)},}
$$

up to an arbitrary constant phase.

## ↑ Ancestors (10)

1. [19D](../19d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
