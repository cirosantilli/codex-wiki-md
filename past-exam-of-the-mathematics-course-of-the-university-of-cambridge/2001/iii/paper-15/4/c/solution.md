<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use both [Kähler identities](../../../../../../kahler-identities.md) from the preceding parts, so that $\partial^*=i[\Lambda,\bar\partial]$ and $\bar\partial^*=-i[\Lambda,\partial]$. For odd operators $a,b$, write $\{a,b\}=ab+ba$. Direct expansion gives

$$
\{\partial,[\Lambda,\bar\partial]\}+\{\bar\partial,[\Lambda,\partial]\}
=[\Lambda,\{\partial,\bar\partial\}]=0.
$$

Since $\partial\bar\partial+\bar\partial\partial=0$, we obtain

$$
\Delta_\partial=i\{\partial,[\Lambda,\bar\partial]\}
=-i\{\bar\partial,[\Lambda,\partial]\}=\Delta_{\bar\partial}.
$$

Together with part (b), this proves the full [Kähler Laplacian identity](../../../../../../kahler-laplacian-identity.md)

$$
\boxed{\Delta_d=2\Delta_\partial=2\Delta_{\bar\partial}.}
$$

Now take the exact form $\eta$. Being $\bar\partial$-exact, it is orthogonal to the harmonic space, so $H\eta=0$, and it is also $\bar\partial$-closed. Choose $\alpha=G\eta$ for the [Dolbeault Green operator](../../../../../../dolbeault-green-operator.md) of the [Dolbeault Laplacian](../../../../../../dolbeault-laplacian.md). Commutation gives $\bar\partial\alpha=G\bar\partial\eta=0$. Therefore

$$
\boxed{\eta=\Delta_{\bar\partial}\alpha=\bar\partial\bar\partial^*\alpha.}
$$

Suppose also $\partial\eta=0$, and put $v=\bar\partial^*\alpha$, $u=\partial v$. The mixed identities and $(\bar\partial^*)^2=0$ give

$$
\bar\partial u=-\partial\bar\partial v=-\partial\eta=0,\qquad
\bar\partial^*u=-\partial\bar\partial^*v=0.
$$

Thus $u=\partial\bar\partial^*\alpha$ is harmonic for the [Dolbeault Laplacian](../../../../../../dolbeault-laplacian.md). By the [Kähler Laplacian identity](../../../../../../kahler-laplacian-identity.md) it is also $\partial$-harmonic and hence $\partial^*u=0$. But it is $\partial$-exact, so

$$
\|u\|^2=\langle\partial v,u\rangle=\langle v,\partial^*u\rangle=0.
$$

Consequently **$\boxed{\partial\bar\partial^*\alpha=0}$**: the form $v$ is $\partial$-closed.

For every harmonic form $h$ of the same bidegree as $v$, $\langle v,h\rangle=\langle\alpha,\bar\partial h\rangle=0$. Harmonic spaces for the two Dolbeault Laplacians coincide, so $v$ has no $\partial$-harmonic component. Apply the $\partial$ version of the [Dolbeault Hodge decomposition](../../../../../../dolbeault-hodge-decomposition-on-a-compact-hermitian-manifold.md). Since $v$ is $\partial$-closed, it has no $\partial^*$-coexact component either. Thus $v=\partial\phi$, with $\phi\in A^{p-1,q-1}$. We conclude the requested [ddbar lemma](../../../../../../ddbar-lemma.md):

$$
\boxed{\eta=\bar\partial\partial\phi.}
$$

For example $\phi=\partial^*Gv$ is a choice, since the same Green operator serves $\Delta_\partial=\Delta_{\bar\partial}$. If $p=0$ or $q=0$, the relevant negative-bidegree space is zero and the argument forces $\eta=0$. Compactness, the absence of boundary and the [Kähler](../../../../../../kahler-manifold.md) condition are essential to this global harmonic argument.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
