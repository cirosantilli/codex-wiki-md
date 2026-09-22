<h1 id="5/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [Fourier sine series](../../../../../../fourier-sine-series.md) automatically meets the zero-temperature [boundary conditions](../../../../../../boundary-condition.md) because $\sin0=\sin(n\pi)=0$. Equivalently, extend $\Theta_0$ oddly from $(0,L)$ to $(-L,L)$ and then periodically with period $2L$. Its [Fourier series](../../../../../../fourier-series-split.md) has only sine terms, with

$$
\boxed{k_n=\frac{n\pi}{L},\qquad b_n=\frac2L\int_0^L\Theta_0(x)\sin\!\left(\frac{n\pi x}{L}\right)dx\quad(n\geq1)}.
$$

The coefficient formula follows from the [orthogonality](../../../../../../orthogonal-vectors.md) identity

$$
\int_0^L\sin(k_nx)\sin(k_mx)\,dx=\frac L2\delta_{nm}.
$$

For piecewise smooth initial data the series equals $\Theta_0$ at interior continuity points and the average of its one-sided values at interior jumps. More general square-integrable data have convergence in [L2 norm convergence](../../../../../../l2-norm-convergence.md). A classical solution continuous at the initial corners additionally requires $\Theta_0(0)=\Theta_0(L)=0$, in agreement with the prescribed [boundary conditions](../../../../../../boundary-condition.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [5](../../../5.md)
4. [Discrete mathematics, continuous mathematics and probability (resit)](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
