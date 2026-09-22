# Negative-energy direction gives exponential growth in a self-adjoint wave equation

↑ **Parent:** [Self-adjoint operator](self-adjoint-operator.md)

Let $\ddot q=Fq$ on a [Hilbert space](hilbert-space-split.md), with time-independent [self-adjoint operator](self-adjoint-operator.md) $F$, and conserved quadratic energy $E=\|\dot q\|^2/2-\langle q,Fq\rangle/2$. If $\langle q_0,Fq_0\rangle>0$, set $\dot q(0)=\alpha q_0$ with $\alpha^2=\langle q_0,Fq_0\rangle/\|q_0\|^2$ and $\alpha>0$. This gives $E=0$. For $N=\|q\|^2$, $N'=2\operatorname{Re}\langle q,\dot q\rangle$ and $N''=4\|\dot q\|^2$, so

$$
(\ln N)''=\frac{4[N\|\dot q\|^2-(\operatorname{Re}\langle q,\dot q\rangle)^2]}{N^2}\geq0
$$

by the [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md). Since $(\ln N)'(0)=2\alpha$, $N(t)\geq N(0)e^{2\alpha t}$. Positivity of $N$ follows from $N'(0)>0$ and $N''\geq0$. Thus a negative direction of the restoring energy $W=-\langle q,Fq\rangle/2$ yields an exponentially growing solution without a normal-mode expansion or a variational spectral theorem. If $W$ is positive definite, conserved $E$ instead controls the energy norm; a bound in the original [Hilbert space](hilbert-space-split.md) norm additionally follows from a coercive lower bound on $W$.

## ↑ Ancestors (7)

1. [Self-adjoint operator](self-adjoint-operator.md)
2. [Operator theory](linear-operator-theory-split.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-64/4/c/solution.md)
