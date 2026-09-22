<h1 id="2d/solution">Solution</h1>

↑ **Parent:** [2D](../2d.md)

The two diagonal $2\times2$ blocks allow the [characteristic polynomial](../../../../../characteristic-polynomial.md) to factor immediately:

$$
\det(\lambda I-A)=\bigl[(\lambda-i)^2-1\bigr]\bigl[(\lambda-i)^2+1\bigr].
$$

Thus the [characteristic equation](../../../../../characteristic-equation-of-a-constant-coefficient-differential-equation.md) is

$$
\boxed{(\lambda-i-1)(\lambda-i+1)\lambda(\lambda-2i)=0.}
$$

Solving the two block [eigenvalue](../../../../../eigenvalue.md) equations gives the following nonzero [eigenvectors](../../../../../eigenvector.md) and corresponding [eigenvalues](../../../../../eigenvalue.md):

$$
\begin{array}{c|c}
\text{eigenvector}&\text{eigenvalue}\\\hline
a=(1,1,0,0)^T&1+i\\
b=(1,-1,0,0)^T&-1+i\\
c=(0,0,1,i)^T&2i\\
d=(0,0,1,-i)^T&0
\end{array}
$$

For example, the lower block maps $(1,i)^T$ to $(2i,-2)^T=2i(1,i)^T$, and maps $(1,-i)^T$ to zero. The four [eigenvalues](../../../../../eigenvalue.md) are distinct. Alternatively, the [determinant](../../../../../determinant.md) of the matrix with columns $a,b,c,d$ is $(-2)(-2i)=4i\ne0$. Hence they form a [basis](../../../../../basis.md) and **span the complex vector space $\mathbb C^4$**. Their nonzero scalar multiples are all the corresponding eigenvectors.

For any [eigenvector](../../../../../eigenvector.md) $v$ with [eigenvalue](../../../../../eigenvalue.md) $\lambda_v$, its one-dimensional [vector subspace](../../../../../vector-subspace.md) satisfies $A(sv)=\lambda_vsv$. If $\lambda_v\ne0$, every $tv$ has preimage $(t/\lambda_v)v$, so the restricted [linear map](../../../../../linear-map.md) is onto that same subspace. Consequently

$$
\boxed{A(\mathbb Ca)=\mathbb Ca,\quad A(\mathbb Cb)=\mathbb Cb,\quad A(\mathbb Cc)=\mathbb Cc,\quad A(\mathbb Cd)=\{0\}.}
$$

The last line is the [kernel of a linear map](../../../../../kernel-of-a-linear-map.md) direction: multiplication by $A$ collapses that line to the zero-dimensional subspace.

## ↑ Ancestors (10)

1. [2D](../2d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
