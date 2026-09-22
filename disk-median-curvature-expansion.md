# Disk-median curvature expansion

↑ **Parent:** [Median filter](median-filter.md)

At a smooth point with nonzero [gradient](gradient.md), rotate coordinates so $\nabla u=G e_2$. Write $u=u_0+Gy+\tfrac12(Ax^2+2Bxy+Cy^2)+O(|(x,y)|^3)$. A candidate [median](median.md) $u_0+dh^2$ has level boundary $y=(dh^2-Ax^2/2)/G+O(h^3)$ in the disk. The area imbalance is $(2d-A/3)h^3/G+o(h^3)$; equal half-areas force $d=A/6$. Here $A=\Delta u-\nabla u^T(D^2u)\nabla u/|\nabla u|^2$ is the tangential second [derivative](derivative.md), giving the formula. The disk uses uniform area measure, not its boundary measure.

## ↑ Ancestors (6)

1. [Median filter](median-filter.md)
2. [Image smoothing](image-smoothing.md)
3. [Diffusion image processing](diffusion-image-processing.md)
4. [Image processing](image-processing.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-64/3/solution.md)
