<h1 id="euler-s-formula">Euler's formula</h1>

↑ **Parent:** [Complex number](complex-number.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euler's_formula)

For a real [angle](angle.md) $\theta$ in [radians](radian.md), Euler's formula states

$$
e^{i\theta}=\cos\theta+i\sin\theta,
$$

where $i$ is the [imaginary unit](imaginary-unit.md). It connects the [complex exponential](complex-exponential-function.md) to the [sine](sine.md) and [cosine](cosine.md) coordinates of the [unit circle](complex-unit-circle.md). In particular, $|e^{i\theta}|=1$, and multiplying by $e^{i\theta}$ rotates a [complex number](complex-number.md) through angle $\theta$ without changing its [modulus](modulus.md). At $\theta=\pi/3$ it gives $e^{i\pi/3}=1/2+i\sqrt3/2$; at $\theta=\pi$, it gives $e^{i\pi}=-1$.

The identity makes [angle](angle.md) addition algebraic: $e^{i\alpha}e^{i\beta}=e^{i(\alpha+\beta)}$. Expanding the product and comparing [real parts](real-part.md) and [imaginary parts](imaginary-part.md) recovers the [sine addition formula](sine-addition-formula.md) and [cosine addition formula](cosine-addition-formula.md). Differentiating $e^{i\omega t}$ gives $i\omega e^{i\omega t}$, and differentiating again gives $-\omega^2e^{i\omega t}$. Its real and imaginary coordinates therefore solve the [harmonic oscillator equation](simple-harmonic-motion.md). This is why [complex exponentials](complex-exponential-function.md) are useful building blocks in [Fourier analysis](fourier-analysis-split.md): differentiation acts on each frequency by simple multiplication.

<a id="image-euler-s-formula-turns-circular-motion-into-sine-and-cosine-traces"></a>
![](circle-exponential-oscillator.png)

**[Figure 10](#image-euler-s-formula-turns-circular-motion-into-sine-and-cosine-traces). Euler's formula turns circular motion into sine and cosine traces**.

A short justification separates the even and odd powers in the absolutely convergent [power series](power-series.md) for $e^{i\theta}$. The even powers give $\sum_{n\geq0}(-1)^n\theta^{2n}/(2n)!=\cos\theta$, and the odd powers give $i\sum_{n\geq0}(-1)^n\theta^{2n+1}/(2n+1)!=i\sin\theta$. The [absolute convergence](absolute-convergence.md) permits this regrouping. The formula thus links an analytic definition of the [complex exponential](complex-exponential-function.md) to a geometric motion rather than merely introducing a convenient notation.

[Leonhard Euler](leonhard-euler.md) presents the relation between imaginary exponentials and [sines](sine.md) and [cosines](cosine.md) in his 1748 Introductio in analysin infinitorum, volume 1, chapter VIII, section 138. His derivation uses limiting powers after connecting trigonometric addition to algebra. The original Latin and Ian Bruce's English translation can be read together in [Euler, Introductio, chapter VIII, section 138](https://www.17centurymaths.com/contents/euler/introductiontoanalysisvolone/ch8vol1.pdf).

## ↑ Ancestors (6)

1. [Complex number](complex-number.md)
2. [Complex analysis](complex-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (27)

- [Characteristic function](characteristic-function-split.md)
- [Delay stability of proportional integrator control](delay-stability-of-proportional-integrator-control.md)
- [Entire function](entire-function.md)
- [Fourier analysis](fourier-analysis-split.md)
- [Laplace transform](laplace-transform.md)
- [Mathematics](mathematics-split.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-2/2b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-1/1a/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ia/paper-1/1c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ia/paper-3/7e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-1/17f/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-3/14a/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-2/41c/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2002/paper-1/11/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-1/9/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2004/paper-1/9/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2004/paper-1/9/a/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-1/section-b/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2008/paper-1/12/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-1/17/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-2/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2020/paper-1/11/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2020/paper-1/11/a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-1/20/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/11/e/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/section-b/8/a/solution.md)
- [Polar form of a complex number](polar-form-of-a-complex-number.md)
