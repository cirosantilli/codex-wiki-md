<h1 id="22h/solution">Solution</h1>

↑ **Parent:** [22H](../22h.md)

The directed positive-transition graph gives the [communicating classes](../../../../../communicating-class.md) $\{1,3,6\}$, $\{2,4\}$ and $\{5\}$. **The first and last classes are closed; $\{2,4\}$ is open.** In particular the PDF's fourth row has all six entries equal to $1/6$. The converted TeX incorrectly drops the last entry; that incomplete row is not a transition distribution.

The finite irreducible closed class $C=\{1,3,6\}$ reaches state six almost surely. For example, from every state in $C$ there is a uniformly positive [probability](../../../../../probability.md) of hitting six within a bounded number of steps, so the [probability](../../../../../probability.md) of avoiding it for successive blocks tends to zero. Put $h_i=\Pr_i(T_6<\infty)$, with $h_1=h_3=h_6=1$ and $h_5=0$. First-step conditioning at states two and four gives

$$
h_2=\frac{2+h_2+h_4}{5},\qquad h_4=\frac{3+h_2+h_4}{6}.
$$

Solving $4h_2-h_4=2$ and $5h_4-h_2=3$ yields **$\boxed{h_2=13/19}$**, with $h_4=14/19$.

Starting in state three, the chain remains in $C$. In the order $(1,3,6)$ its [transition matrix](../../../../../stochastic-matrix.md) is

$$
M=\begin{pmatrix}0&1/2&1/2\\1/3&1/3&1/3\\1/4&1/2&1/4\end{pmatrix}.
$$

Its characteristic polynomial is $(\lambda-1)(\lambda+1/4)(\lambda+1/6)$. Thus, by the [Cayley-Hamilton theorem](../../../../../cayley-hamilton-theorem.md), $q_n=(M^n)_{2,3}$ is a [linear combination](../../../../../linear-combination.md) of $1,(-1/4)^n,(-1/6)^n$. The initial values are $q_0=0$, $q_1=1/3$, and $q_2=(1/3)(1/2+1/3+1/4)=13/36$. Solving for the three coefficients gives

$$
\boxed{\Pr_3(X_n=6)=\frac{12}{35}+\frac45\left(-\frac14\right)^n-\frac87\left(-\frac16\right)^n,\qquad n\geq1.}
$$

The limiting value $12/35$ agrees with the state-six [probability](../../../../../probability.md) of the [stationary distribution](../../../../../stationary-distribution.md) $(8/35,3/7,12/35)$ of this closed class.

## ↑ Ancestors (10)

1. [22H](../22h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
