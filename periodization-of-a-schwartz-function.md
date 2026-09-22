# Periodization of a Schwartz function

↑ **Parent:** [Poisson summation formula](poisson-summation-formula.md)

For a [Schwartz function](schwartz-function.md) on the [real numbers](real-number.md), its periodization $P_f$ is a [smooth](smooth-function.md) [periodic function](periodic-function.md) of [period of a function](period-of-a-function.md) one. Rapid decay gives [uniform convergence](uniform-convergence.md) on $[0,1]$ of the defining [series](series-mathematics.md) and each differentiated [series](series-mathematics.md). Its $k$th [Fourier coefficient](fourier-coefficient.md) is

$$
c_k=\int_0^1P_f(x)e^{-2\pi ikx}\,dx
=\sum_{n\in\mathbb Z}\int_n^{n+1}f(u)e^{-2\pi iku}\,du
=\widehat f(k).
$$

The change of variable $u=x+n$ uses $e^{2\pi ikn}=1$. Rapidly decreasing [Fourier coefficients](fourier-coefficient.md) give the absolutely and uniformly convergent [Fourier series](fourier-series-split.md) $P_f(x)=\sum_k\widehat f(k)e^{2\pi ikx}$. Evaluation at $x=0$ proves the [Poisson summation formula](poisson-summation-formula.md).[Lecture 17, §17.1, Theorem 17.8 and proof, printed p. 3: periodization and Fourier coefficients](number-theory-i-mit-18-785-fall-2021/lecture-17-the-functional-equation.md)

The same identity explains [aliasing](aliasing.md) in the [Nyquist–Shannon sampling theorem](nyquist-shannon-sampling-theorem.md): applying the [Poisson summation formula](poisson-summation-formula.md) to the [Schwartz function](schwartz-function.md) $x\mapsto f(x)e^{-2\pi i\xi x}$ gives

$$
\sum_{n\in\mathbb Z}f(n)e^{-2\pi i\xi n}
=\sum_{k\in\mathbb Z}\widehat f(\xi+k).
$$

The sampled spectrum is periodic in [frequency](frequency.md), and shifted copies of the continuous [Fourier transform](fourier-transform-split.md) add together. When those copies overlap, the samples cannot separate their contributions. The [Nyquist–Shannon sampling theorem](nyquist-shannon-sampling-theorem.md) adds a [bandlimited function](bandlimited-function.md) hypothesis to make reconstruction possible.

## ↑ Ancestors (6)

1. [Poisson summation formula](poisson-summation-formula.md)
2. [Fourier analysis](fourier-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-28/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-30/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-126/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-137/1/solution.md)
