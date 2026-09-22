<h1 id="s31/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For balanced global error $\varepsilon$, a method second order in both variables can take $h\sim\varepsilon^{1/2}$ and $k\sim\varepsilon^{1/2}$. With $O(1/h)$ work per time step in one spatial dimension, its cost scales as $\varepsilon^{-1}$. A method second order in space but first order in time instead needs $k\sim\varepsilon$, so its cost is $\boxed{O(\varepsilon^{-3/2})}$ under the same per-step cost assumption. Equivalently at fixed $h$, using $k\sim h^2$ rather than $k\sim h$ needs about $1/h$ more steps. A restrictive stability condition or different linear-solver cost can dominate these accuracy-based estimates.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [S31](../../../s31.md)
4. [2019](../../../../2019-split.md)
5. [Past exam of the short options paper shared by Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
