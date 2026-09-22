<h1 id="29d/solution">Solution</h1>

↑ **Parent:** [29D](../29d.md)

Solve $\dot Q=-AQ$, $Q(0)=I$. Since $A^T=-A$, differentiation gives $Q^TQ=I$. To see why the [Lax equation preserves the spectrum](../../../../../lax-equation-preserves-the-spectrum.md), direct differentiation gives

$$
\frac d{dt}(Q^TLQ)=Q^T(AL+\dot L-LA)Q=0.
$$

Thus $L(t)=Q(t)L(0)Q(t)^T$ is an [orthogonal similarity](../../../../../orthogonal-similarity.md), so **all eigenvalues and all coefficients of its characteristic polynomial are first integrals**.

A $2n$-dimensional [Hamiltonian system](../../../../../hamiltonian-system.md) is [Liouville integrable](../../../../../integrable-hamiltonian-system.md) when it has $n$ functionally independent first integrals, including the Hamiltonian, whose pairwise [Poisson brackets](../../../../../poisson-bracket.md) vanish, on an open dense regular region.

For the three-particle periodic [Toda lattice](../../../../../periodic-toda-lattice.md), take $p_i=\dot q_i$. The proposed Hamiltonian has

$$
\dot q_i=\partial_{p_i}H=p_i,\qquad \dot p_i=-\partial_{q_i}H=e^{q_{i-1}-q_i}-e^{q_i-q_{i+1}},
$$

which are exactly the equations of motion. Differentiating the new variables gives

$$
\dot a_i=\tfrac12a_i(p_i-p_{i+1})=(b_{i+1}-b_i)a_i,\qquad\dot b_i=2(a_i^2-a_{i-1}^2).
$$

The transformation is **not canonical**. For example

$$
\{a_i,b_j\}=-\frac{a_i}{4}(\delta_{ij}-\delta_{i+1,j}),
$$

rather than canonical coordinate brackets. Moreover $a_1a_2a_3=1/8$, so the map forgets the common translation of all the $q_i$ and is not an invertible coordinate change on the six-dimensional phase space.

Multiplication of the displayed matrices gives diagonal entries $2(a_i^2-a_{i-1}^2)$ and off-diagonal entries $(b_{i+1}-b_i)a_i$ in $LA-AL$. Therefore they form the required [Lax pair](../../../../../lax-pair.md). The three characteristic coefficients are

$$
\begin{aligned}
C_1&=b_1+b_2+b_3,\\
C_2&=b_1b_2+b_2b_3+b_3b_1-a_1^2-a_2^2-a_3^2,\\
C_3&=b_1b_2b_3-b_1a_2^2-b_2a_3^2-b_3a_1^2+2a_1a_2a_3.
\end{aligned}
$$

They are independent first integrals, as permitted without proof. Equivalently **one may take**

$$
\boxed{\begin{aligned}
P&=p_1+p_2+p_3,\\
H&=\tfrac12\sum p_i^2+\sum e^{q_i-q_{i+1}},\\
J&=p_1p_2p_3-p_1e^{q_2-q_3}-p_2e^{q_3-q_1}-p_3e^{q_1-q_2}.
\end{aligned}}
$$

Indeed $C_1=-P/2$, $C_2=P^2/8-H/4$ and $C_3=1/4-J/8$. Their mutual Poisson commutation also follows directly: $P$ generates the common translation, and $\{H,J\}=0$ because $J$ is conserved.

## ↑ Ancestors (10)

1. [29D](../29d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
