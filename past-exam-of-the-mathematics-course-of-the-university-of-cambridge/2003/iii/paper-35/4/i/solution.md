<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**The concavity inequality is true, but its printed equality condition is false.** At $b=1$ equality always holds, even for distinct states; for example take $\rho_1=|0\rangle\langle0|$ and $\rho_2=|1\rangle\langle1|$. The correct statement on $0\le b\le1$ is

$$
\boxed{\text{Equality holds iff }b\in\{0,1\}\text{ or }\rho_1=\rho_2.}
$$

For $0<b<1$, entropy is therefore strictly concave.

We give the [matrix](../../../../../../matrix.md) inequality needed for the proof. Define the [quantum relative entropy](../../../../../../quantum-relative-entropy.md) $D(\tau\|\sigma)=\operatorname{tr}\tau(\log_2\tau-\log_2\sigma)$ if the support of $\tau$ is contained in that of $\sigma$, and $+\infty$ otherwise. Diagonalize the two states with [eigenvalues](../../../../../../eigenvalue.md) $r_i,s_j$, and put $q_{ij}=|\langle i|j\rangle|^2$. Each row and column of $q$ sums to one. The elementary scalar inequality

$$
u\ln(u/v)\ge u-v
$$

follows from $x\ln x-x+1\ge0$, with equality exactly at $x=1$; use limits at zero. Consequently

$$
D(\tau\|\sigma)=\frac1{\ln2}\sum_{ij}q_{ij}r_i\ln(r_i/s_j)
\ge\frac1{\ln2}\sum_{ij}q_{ij}(r_i-s_j)=0.
$$

Equality forces $r_i=s_j$ whenever $q_{ij}>0$. Hence every [eigenvector](../../../../../../eigenvector.md) $|i\rangle$ of $\tau$ is also a $\sigma$-[eigenvector](../../../../../../eigenvector.md) with [eigenvalue](../../../../../../eigenvalue.md) $r_i$, so $\tau=\sigma$. Conversely identical states give zero relative entropy. This proves [nonnegativity of quantum relative entropy](../../../../../../nonnegativity-of-quantum-relative-entropy.md) and its equality condition, including states with zero [eigenvalues](../../../../../../eigenvalue.md) under the support convention.

Now set $\rho=b\rho_1+(1-b)\rho_2$. For $0<b<1$ its support contains both component supports. Direct expansion gives

$$
S(\rho)-bS(\rho_1)-(1-b)S(\rho_2)
=bD(\rho_1\|\rho)+(1-b)D(\rho_2\|\rho)\ge0.
$$

Since both coefficients are positive, equality holds exactly when both component states equal $\rho$, equivalently $\rho_1=\rho_2$. At either endpoint the mixture has only one component and equality is automatic. This proves the corrected [strict concavity of Von Neumann entropy](../../../../../../strict-concavity-of-von-neumann-entropy.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
