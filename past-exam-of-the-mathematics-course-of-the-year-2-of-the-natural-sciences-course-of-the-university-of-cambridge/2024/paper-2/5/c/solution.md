<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [convolution theorem](../../../../../convolution-theorem.md) gives the causal response

$$
\phi(t)=\frac{I_0}q\int_0^{\min(t,1)}e^{-p(t-\tau)}\sin\bigl(q(t-\tau)\bigr)\,d\tau\quad(t>0).
$$

Define the integrated [impulse response](../../../../../impulse-response.md), for $s\geq0$, by

$$
F(s)=\frac{1-e^{-ps}\cos(qs)-(p/q)e^{-ps}\sin(qs)}{p^2+q^2}.
$$

Direct differentiation gives $F'(s)=e^{-ps}\sin(qs)/q$ and $F(0)=F'(0)=0$. Thus

$$
\boxed{\phi(t)=\begin{cases}
0,&t\leq0,\\
I_0F(t),&0<t\leq1,\\
I_0\bigl[F(t)-F(t-1)\bigr],&t>1.
\end{cases}}
$$

In particular, after switch-off the answer is

$$
\boxed{\phi(t)=\frac{I_0}{p^2+q^2}\left\{
e^{-p(t-1)}\left[\cos q(t-1)+\frac pq\sin q(t-1)\right]
-e^{-pt}\left[\cos qt+\frac pq\sin qt\right]\right\},\quad t>1.}
$$

The response and its first [derivative](../../../../../derivative.md) are continuous at both switching times, and the post-pulse motion is a freely decaying [damped harmonic oscillator](../../../../../damped-harmonic-oscillator.md). The expression described as valid for $t<1$ in the paper is understood for $0<t<1$; before the pulse the causal output is zero.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
