<h1 id="23f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

We prove the estimate first for $u$ in the [Schwartz space](../../../../../../schwartz-space.md). By the [Fourier inversion theorem](../../../../../../fourier-inversion-theorem.md) and the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md),

$$
\begin{aligned}
|u(x)|
&\leq C\int_{\mathbb R^n}|\widehat u(\xi)|\,d\xi\\
&\leq C
\left(\int_{\mathbb R^n}(1+|\xi|^2)^{-n}\,d\xi\right)^{1/2}
\lVert u\rVert_{H^n}.
\end{aligned}
$$

The integral is finite because $n>n/2$.

For $0<\alpha\leq1$, the elementary bound

$$
|e^{it}-1|\leq C_\alpha|t|^\alpha
$$

gives

$$
\begin{aligned}
|u(x)-u(y)|
&\leq C|x-y|^\alpha
 \int_{\mathbb R^n}|\xi|^\alpha|\widehat u(\xi)|\,d\xi\\
&\leq C|x-y|^\alpha
\left(\int_{\mathbb R^n}
 |\xi|^{2\alpha}(1+|\xi|^2)^{-n}\,d\xi\right)^{1/2}
\lVert u\rVert_{H^n}.
\end{aligned}
$$

The last integral is finite near zero for every $\alpha>0$ and at infinity exactly when $2\alpha<n$. Choose, for example, $\alpha=1/4$, which works for every $n\geq1$. We obtain

$$
\lVert u\rVert_{C^{0,1/4}}
\leq C_n\lVert u\rVert_{H^n}.
$$

Density of the Schwartz space in $H^n$ extends the estimate and supplies a unique Hölder-continuous representative. Therefore

$$
H^n(\mathbb R^n)\hookrightarrow C^{0,1/4}(\mathbb R^n)
$$

continuously. This is the [Fourier proof of Hölder regularity from a Sobolev norm](../../../../../../fourier-proof-of-holder-regularity-from-a-sobolev-norm.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [23F](../../23f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
