<h1 id="section-b/b4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

There are errors in the original PDF at this point, not merely in the TeX transcription. The second exponential must denote the [eigenvalue](../../../../../eigenvalue.md) $\lambda_-(z)=e^{-\gamma^-z}$, not the propagation coefficient itself. More substantially, the printed prefactor $\operatorname{sech}(\delta z)$ is inconsistent with the stated exponential [eigenvalues](../../../../../eigenvalue.md). It must be $\cosh(\delta z)$. The original's primed Jones-matrix label distinguishes the distributed component from the earlier static matrix; below write $\mathcal J(z)$ to avoid confusing that prime with a derivative.

Complex [eigenvalues](../../../../../eigenvalue.md) have no intrinsic largest/smallest ordering, so $+$ and $-$ are modal labels. Keep the circular [eigenvectors](../../../../../eigenvector.md) fixed, put $\gamma=(\gamma^++\gamma^-)/2$ and $\delta=(\gamma^+-\gamma^-)/2$, and use the [spectral decomposition](../../../../../spectral-decomposition.md) from part (c):

$$
\mathcal J(z)=e^{-\gamma^+z}P_++e^{-\gamma^-z}P_-.
$$

Its diagonal entries are $(e^{-\gamma^+z}+e^{-\gamma^-z})/2=e^{-\gamma z}\cosh(\delta z)$, and its upper off-diagonal entry is $i(e^{-\gamma^+z}-e^{-\gamma^-z})/2=-ie^{-\gamma z}\sinh(\delta z)$. Therefore

$$
\boxed{\mathcal J(z)=e^{-\gamma z}
\begin{pmatrix}\cosh(\delta z)&-i\sinh(\delta z)\\i\sinh(\delta z)&\cosh(\delta z)\end{pmatrix}.}
$$

Where $\cosh(\delta z)\neq0$, this can be factored as

$$
\mathcal J(z)=e^{-\gamma z}\cosh(\delta z)
\begin{pmatrix}1&-i\tanh(\delta z)\\i\tanh(\delta z)&1\end{pmatrix}.
$$

The unfactored expression is valid even at zeros of the cosine-like factor when $\delta$ is imaginary. The printed expression is $\operatorname{sech}^2(\delta z)$ times this correct matrix; its [eigenvalues](../../../../../eigenvalue.md) are consequently $e^{-\gamma^\pm z}\operatorname{sech}^2(\delta z)$ rather than those specified. A second check is $\det\mathcal J=e^{-2\gamma z}$, whereas the printed version has [determinant](../../../../../determinant.md) $e^{-2\gamma z}\operatorname{sech}^4(\delta z)$. Thus the requested printed identity cannot be proved except in the degenerate case $\delta=0$; the following parts use the consistent propagator.

## ↑ Ancestors (14)

1. [D](../d.md)
2. [B4](../../b4.md)
3. [Section B](../../../section-b.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the optics and electrodynamics course of the University of Cambridge](../../../../split.md)
6. [Optics and Electrodynamics course of the University of Cambridge](../../../../../optics-and-electrodynamics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
