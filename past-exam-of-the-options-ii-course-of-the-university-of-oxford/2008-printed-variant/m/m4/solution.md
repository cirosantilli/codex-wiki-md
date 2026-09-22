<h1 id="m/m4/solution">Solution</h1>

↑ **Parent:** [M4](../m4.md)

The moment generating [function](../../../../function-split.md) is $M_X(\theta)=\mathbb E(e^{\theta X})$ where finite. The [continuity](../../../../continuous-function.md) theorem states that, if moment generating functions are finite on a common open interval containing zero and converge there to the moment generating [function](../../../../function-split.md) of a probability law, the corresponding distributions converge weakly to that law.

Integrating the gamma density and using the gamma integral gives

$$
M_X(\theta)=\frac{\lambda^\alpha}{\Gamma(\alpha)}\int_0^\infty x^{\alpha-1}e^{-(\lambda-\theta)x}\,dx
=\left(\frac{\lambda}{\lambda-\theta}\right)^\alpha,\qquad\theta<\lambda.
$$

For a geometric waiting time, on $1,2,\ldots$, summing the geometric series gives

$$
M_Y(\theta)=\sum_{j\ge1}p(1-p)^{j-1}e^{j\theta}=
\frac{pe^\theta}{1-(1-p)e^\theta},\qquad \theta<-\log(1-p)
$$

when $0<p<1$. For $p=1$, $Y=1$ deterministically. The waiting times between successive heads are independent and identically distributed, so $N=Y_1+\cdots+Y_k$ and $M_N=M_Y^k$. Therefore

$$
M_{2pN}(\theta)=\left\{\frac{pe^{2p\theta}}{1-(1-p)e^{2p\theta}}\right\}^k
\longrightarrow (1-2\theta)^{-k}.
$$

Indeed the denominator is $p(1-2\theta)+O(p^2)$ and the numerator is $p+O(p^2)$. On any sufficiently small fixed neighbourhood of zero these moment generating functions exist for all sufficiently small $p$. The limit is the moment generating [function](../../../../function-split.md) of a gamma law with **shape $k$ and rate $1/2$**, so

$$
\boxed{2pN\ \xrightarrow{d}\ \operatorname{Gamma}(k,1/2)}.
$$

## ↑ Ancestors (12)

1. [M4](../m4.md)
2. [M](../../m.md)
3. [2008 printed variant](../../../2008-printed-variant-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
