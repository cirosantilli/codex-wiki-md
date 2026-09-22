<h1 id="18c/solution">Solution</h1>

↑ **Parent:** [18C](../18c.md)

For a nonzero real vector $v$, the [Householder transformation](../../../../../householder-transformation.md) is

$$
H=I-2\frac{vv^T}{v^Tv}.
$$

Writing $P=vv^T/(v^Tv)$ gives $P^T=P$, $P^2=P$, so $H^T=H$ and $H^TH=(I-2P)^2=I$. Thus **$H$ is orthogonal**. It reverses the component along $v$ and fixes its orthogonal complement.

For [Householder QR decomposition](../../../../../householder-qr-decomposition.md), successively choose a reflector on each trailing row block to send its current column to a multiple of the first coordinate vector. Each step annihilates the subdiagonal entries without disturbing earlier columns. The reflector product gives an upper-trapezoidal $R$ and its transpose gives an orthogonal $Q$ with $A=QR$.

Here the first column has norm four. Taking $v=(-1,1,-1,1)^T$ gives $H_1=I-vv^T/2$ and

$$
H_1A=\begin{pmatrix}4&4&8\\0&6&-3\\0&0&9\\0&0&12\end{pmatrix}.
$$

The second column already has no unwanted entries. On the last two rows, reflect using $(-1,2)^T$:

$$
B=I_2-\frac25\begin{pmatrix}1&-2\\-2&4\end{pmatrix}=\begin{pmatrix}3/5&4/5\\4/5&-3/5\end{pmatrix},\qquad H_3=\operatorname{diag}(I_2,B).
$$

This maps $(9,12)^T$ to $(15,0)^T$. Therefore a full [QR factorization](../../../../../qr-decomposition.md) is

$$
\boxed{R=\begin{pmatrix}4&4&8\\0&6&-3\\0&0&15\\0&0&0\end{pmatrix},\qquad Q=H_1H_3=\frac1{10}\begin{pmatrix}5&5&1&-7\\5&5&-1&7\\-5&5&7&1\\5&-5&7&1\end{pmatrix}.}
$$

Both displayed factors arise from the explicit reflectors; in particular $Q^TQ=I_4$ and $QR=A$.

The first three diagonal entries of $R$ are nonzero, so the column rank is three and a consistent system has a unique solution. Consistency requires the last component of $Q^Tb$ to vanish. For the given right side this component is

$$
\frac1{10}[-7(1+\lambda)+7\cdot2+3+4]=\frac7{10}(2-\lambda).
$$

Hence

$$
\boxed{\lambda=2.}
$$

For this value the transformed right side is $(3,2,5,0)^T$. [Back substitution](../../../../../back-substitution.md) also gives $x=(-5/12,1/2,1/3)^T$. This illustrates the [Householder reduction of an overdetermined consistent system](../../../../../householder-reduction-of-an-overdetermined-consistent-system.md).

## ↑ Ancestors (10)

1. [18C](../18c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
