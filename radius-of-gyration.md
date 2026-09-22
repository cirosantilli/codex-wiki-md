# Radius of gyration

↑ **Parent:** [Polymer](polymer.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Radius_of_gyration)

For $N$ equally weighted positions, the squared [radius of gyration](radius-of-gyration.md) is the average squared distance from the [center of mass](center-of-mass.md): $R_g^2=N^{-1}\sum_n\langle|\mathbf R_n-\mathbf R_{\rm cm}|^2\rangle$, where $\mathbf R_{\rm cm}=N^{-1}\sum_n\mathbf R_n$. Expanding pair differences gives $\sum_{m,n}|\mathbf R_m-\mathbf R_n|^2=2N\sum_n|\mathbf R_n-\mathbf R_{\rm cm}|^2$, and therefore

$$
R_g^2=\frac1{2N^2}\sum_{m,n}\langle|\mathbf R_m-\mathbf R_n|^2\rangle.
$$

For a [Gaussian chain](gaussian-chain.md) or [freely jointed chain](ideal-chain.md) with these $N$ positions and mean squared link length $b^2$, each pair [variance](variance-split.md) is $b^2|m-n|$. Summing separations yields $R_g^2=b^2(N^2-1)/(6N)\sim Nb^2/6$. Counting all endpoints of $N$ links instead gives $N+1$ positions and the corresponding finite-size formula.

## ↑ Ancestors (3)

1. [Polymer](polymer.md)
2. [Chemistry](chemistry-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Guinier expansion of a polymer scattering function](guinier-expansion-of-a-polymer-scattering-function.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-71/5/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-75/3/solution.md)
- [Radius of gyration](radius-of-gyration.md)
