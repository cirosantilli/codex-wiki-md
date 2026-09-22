<h1 id="8b/solution">Solution</h1>

↑ **Parent:** [8B](../8b.md)

Write the [linear differential equation](../../../../../linear-differential-equation.md) as $\dot{\mathbf x}=M\mathbf x$, with

$$
M=\begin{pmatrix}-4&-3\\3&-4\end{pmatrix}.
$$

Its [characteristic polynomial](../../../../../characteristic-polynomial.md) is $(\lambda+4)^2+9$. Thus a choice of [eigenvalues](../../../../../eigenvalue.md) and [eigenvectors](../../../../../eigenvector.md) is

$$
\boxed{\lambda_1=-4+3i,\quad\mathbf x^{(1)}=\binom1{-i},
\qquad\lambda_2=-4-3i,\quad\mathbf x^{(2)}=\binom1i.}
$$

The distinct [eigenvalues](../../../../../eigenvalue.md) give two [linearly independent](../../../../../linear-independence.md) solutions, and the general complex solution is

$$
\mathbf x(t)=a_1\mathbf x^{(1)}e^{\lambda_1t}+a_2\mathbf x^{(2)}e^{\lambda_2t}.
$$

Real solutions have $a_2=\overline{a_1}$. Equivalently,

$$
\mathbf x(t)=e^{-4t}\binom{C\cos3t-D\sin3t}{C\sin3t+D\cos3t},\qquad C,D\in\mathbb R.
$$

They spiral counterclockwise towards the origin, which is a [stable spiral](../../../../../stable-spiral.md).

In a forced [linear differential equation](../../../../../linear-differential-equation.md), [resonance in a differential equation](../../../../../resonance-in-a-differential-equation.md) occurs when exponential forcing excites a mode with the same exponent as its [eigenvalue](../../../../../eigenvalue.md), producing a polynomial factor such as $t$ multiplying that exponential. Merely matching an exponent is not enough: its projection onto that mode must be nonzero. Here $te^{\lambda_jt}$ still decays in absolute magnitude because the real part of $\lambda_j$ is negative; resonance refers to this extra factor, not necessarily to unbounded growth.

For each forcing vector, resolve it in the [eigenvector](../../../../../eigenvector.md) basis:

$$
\binom{p_j}{q_j}=c_{1j}\binom1{-i}+c_{2j}\binom1i,
\qquad c_{1j}=\frac{p_j+iq_j}{2},\quad c_{2j}=\frac{p_j-iq_j}{2}.
$$

If $u_k$ is the coefficient of the $k$th [eigenvector](../../../../../eigenvector.md), its scalar equation is $\dot u_k=\lambda_k u_k+\sum_jc_{kj}e^{\lambda_jt}$. Multiplying by $e^{-\lambda_kt}$ and integrating shows that the $j=k$ contribution is $c_{kk}te^{\lambda_kt}$, whereas a $j\ne k$ contribution is $c_{kj}e^{\lambda_jt}/(\lambda_j-\lambda_k)$. Therefore the exact conditions for no resonant response are

$$
\boxed{p_1+iq_1=0,\qquad p_2-iq_2=0.}
$$

Under these conditions one [particular solution](../../../../../particular-solution.md) is

$$
\mathbf x_{\rm p}(t)=\frac{c_{21}}{6i}\mathbf x^{(2)}e^{\lambda_1t}
-\frac{c_{12}}{6i}\mathbf x^{(1)}e^{\lambda_2t},
$$

which contains no factor of $t$. For a real forcing, $p_2=\overline{p_1}$ and $q_2=\overline{q_1}$, and the two boxed conditions are conjugate to each other.

## ↑ Ancestors (11)

1. [8B](../8b.md)
2. [Section II](../section-ii.md)
3. [Paper 2](../../paper-2-split.md)
4. [Ia](../../split.md)
5. [2004](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
