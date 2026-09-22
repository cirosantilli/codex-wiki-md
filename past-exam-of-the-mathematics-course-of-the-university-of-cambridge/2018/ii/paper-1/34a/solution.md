<h1 id="34a/solution">Solution</h1>

↑ **Parent:** [34A](../34a.md)

Choose any basis of two independent local solutions and collect their coefficients into a column $c_n$ immediately to the right of the $n$th cell boundary. The **[Floquet matrix](../../../../../floquet-matrix-for-a-one-dimensional-periodic-potential.md)** is the one-period matrix $F(E)$ defined by

$$
c_{n+1}=F(E)c_n.
$$

Equivalently, it advances the Cauchy data $(\psi,\psi')^T$ by one period. The [Wronskian](../../../../../wronskian.md) of two solutions of the stationary [Schrödinger equation](../../../../../schrodinger-equation.md) is constant between the delta functions, and the derivative jump at each delta function also has determinant one. Consequently

$$
\boxed{\det F=1.}
$$

For a real potential the Floquet matrix in the real Cauchy-data basis is real, so its trace is real in every basis. Its [Floquet multipliers](../../../../../floquet-multiplier.md) $\rho_\pm$ satisfy

$$
\rho_+\rho_-=1,
\qquad
\rho_++\rho_-=\operatorname{tr}F.
$$

By [Bloch theorem](../../../../../bloch-s-theorem.md), an energy is in the interior of an [allowed energy band](../../../../../allowed-energy-band.md) when $\rho_\pm=e^{\pm iqa}$ are distinct unit-modulus numbers. Since $\operatorname{tr}F$ is real, this is equivalent to

$$
\boxed{(\operatorname{tr}F)^2<4.}
$$

For the [attractive delta-comb Kronig-Penney model](../../../../../attractive-delta-comb-kronig-penney-model.md), integrating the [Schrödinger equation](../../../../../schrodinger-equation.md) across a lattice point gives

$$
\psi(na^+)=\psi(na^-),
\qquad
\psi'(na^+)-\psi'(na^-)=-2\lambda\psi(na).
$$

At negative energy write $E=-\hbar^2\mu^2/(2m)$ and use the local basis $e^{\pm\mu(x-na)}$. Free propagation through one cell followed by the derivative jump gives

$$
F_-(\mu)=
\begin{pmatrix}1-\lambda/\mu&-\lambda/\mu\\
\lambda/\mu&1+\lambda/\mu\end{pmatrix}
\begin{pmatrix}e^{\mu a}&0\\0&e^{-\mu a}\end{pmatrix}.
$$

Thus

$$
\det F_-=1,
\qquad
\frac12\operatorname{tr}F_-
=\cosh(\mu a)-\frac\lambda\mu\sinh(\mu a).
$$

The band condition is therefore

$$
-1<\cosh(\mu a)-\frac\lambda\mu\sinh(\mu a)<1.
$$

Using $(\cosh u-1)/\sinh u=\tanh(u/2)$ and $(\cosh u+1)/\sinh u=\coth(u/2)$ gives the requested inequality

$$
\boxed{\lambda\tanh\frac{\mu a}{2}<\mu<\lambda\coth\frac{\mu a}{2}.}
$$

At positive energy write $E=\hbar^2k^2/(2m)$ and use $e^{\pm ik(x-na)}$. The corresponding matrix is

$$
F_+(k)=
\begin{pmatrix}1+i\lambda/k&i\lambda/k\\
-i\lambda/k&1-i\lambda/k\end{pmatrix}
\begin{pmatrix}e^{ika}&0\\0&e^{-ika}\end{pmatrix},
$$

so

$$
\det F_+=1,
\qquad
\frac12\operatorname{tr}F_+
=\cos(ka)-\frac\lambda k\sin(ka).
$$

Hence the positive-energy bands are exactly the values of $k>0$ for which

$$
\boxed{\left|\cos(ka)-\frac\lambda k\sin(ka)\right|<1.}
$$

Finally, the zero-energy limit has $\tfrac12\operatorname{tr}F=1-\lambda a$. If $\lambda a>2$, then $|1-\lambda a|>1$, and therefore **zero energy lies in a forbidden gap**.

## ↑ Ancestors (10)

1. [34A](../34a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
