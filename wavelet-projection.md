# Wavelet projection

↑ **Parent:** [Multiresolution analysis](multiresolution-analysis.md)

The wavelet projection is the [orthogonal projection](orthogonal-projection.md) onto the approximation space $V_J$. Iterating $V_{j+1}=V_j\oplus W_j$ expresses it as the coarse part of the [wavelet series](wavelet-series.md) plus details at levels below $J$. [Orthogonality](orthogonal-vectors.md) gives $\|m-P_Jm\|_2^2=\sum_{j\geq J,k}|b_{j,k}|^2$, which tends to zero by the [Parseval identity for a Hilbertian basis](parseval-identity-for-a-hilbertian-basis.md). The projection can also be represented by $A_J(x,y)=\sum_k\phi_{J,k}(x)\phi_{J,k}(y)$ as an [integral kernel](integral-kernel.md) in the Hilbert-space sense.

## ↑ Ancestors (7)

1. [Multiresolution analysis](multiresolution-analysis.md)
2. [Wavelet](wavelet.md)
3. [Fourier analysis](fourier-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-45/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-31/3/solution.md)
