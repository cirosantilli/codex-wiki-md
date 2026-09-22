<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [computational problem in the SCI hierarchy](../../../../../../computational-problem-in-the-sci-hierarchy.md) is a quadruple

$$
(\Xi,\Omega,\mathcal M,\Lambda).
$$

Here $\Omega$ is the primary set of inputs, $\Lambda$ is the set of permitted evaluation functions, $(\mathcal M,d)$ is the output [metric space](../../../../../../metric-space.md), and $\Xi:\Omega\to\mathcal M$ is the problem function. The [Solvability complexity index](../../../../../../solvability-complexity-index.md) is defined from the minimum height of a [tower of algorithms](../../../../../../tower-of-algorithms.md) that computes $\Xi$ from finite subsets of $\Lambda$.

For the [classical computational spectral problem](../../../../../../classical-computational-spectral-problem.md), take

$$
\Omega=\mathcal B(\ell^2(\mathbb N)),\qquad
\lambda_{ij}(A)=\langle Ae_j,e_i\rangle,\qquad
\Lambda=\{\lambda_{ij}:i,j\in\mathbb N\},
$$

and

$$
\Xi(A)=\operatorname{Sp}(A).
$$

Since the [spectrum of a bounded operator](../../../../../../spectrum-of-a-bounded-operator.md) is a nonempty [compact subset](../../../../../../compact-space.md) of the [complex numbers](../../../../../../complex-number.md), one may take $\mathcal M$ to be the nonempty compact subsets of $\mathbb C$ with the [Hausdorff distance](../../../../../../hausdorff-distance.md). The [Attouch--Wets topology](../../../../../../attouch-wets-topology.md) gives an equivalent convenient formulation on bounded spectral sets and also extends naturally to unbounded closed sets. This choice of $\mathcal M$ makes convergence mean convergence of the whole spectrum as a set, including both the absence of persistent [spectral pollution](../../../../../../spectral-pollution.md) and the approximation of every genuine spectral point.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 358](../../../paper-358-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
