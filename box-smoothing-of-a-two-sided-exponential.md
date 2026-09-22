# Box smoothing of a two-sided exponential

↑ **Parent:** [Convolution](convolution.md)

For $a,b>0$, the [convolution](convolution.md) of the normalized interval indicator $(2a)^{-1}\mathbf1_{[-a,a]}$ with the two-sided exponential $(2b)^{-1}e^{-|x|/b}$ is

$$
w(x)=\begin{cases}[1-e^{-a/b}\cosh(x/b)]/(2a),&|x|\leq a,\\\sinh(a/b)e^{-|x|/b}/(2a),&|x|\geq a.\end{cases}
$$

Split the defining integral at $t=x$ in the interior case; outside the interval the absolute value has a fixed sign. These elementary integrals prove the formula and its continuity at the joining points. With [Fourier transform](fourier-transform-split.md) convention $\widehat w(k)=\int w(x)e^{-ikx}dx$, the [convolution theorem](convolution-theorem.md) gives $\widehat w(k)=\sin(ak)/[ak(1+b^2k^2)]$, using its continuous value at $k=0$. [Parseval's identity](parseval-identity.md) can therefore turn the squared integral of this rational-trigonometric transform into a piecewise elementary real-space integral.

## ↑ Ancestors (6)

1. [Convolution](convolution.md)
2. [Fourier analysis](fourier-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2004/paper-1/3/c/solution.md)
