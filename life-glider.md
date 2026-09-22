# Life glider

↑ **Parent:** [Conway Game of Life](conway-game-of-life.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Glider_(Conway's_Game_of_Life))

The [Life glider](life-glider.md) is a five-cell pattern that recreates its shape after four generations, shifted one cell along each coordinate. Use $x$ increasing rightward and $y$ increasing downward, as in the figure, and start from the live [set](set-split.md)

$$
G_0=\{(1,0),(2,1),(0,2),(1,2),(2,2)\}.
$$

Every cell outside $G_0$ starts dead. Applying the [Conway's Game of Life](conway-game-of-life.md) rule, rather than moving the drawing by hand, gives:

<a id="image-four-synchronous-conway-s-game-of-life-steps-translate-the-life-glider-by-1-1"></a>
![](conway-life-glider-frames.png)

**[Figure 16](#image-four-synchronous-conway-s-game-of-life-steps-translate-the-life-glider-by-1-1). Four synchronous Conway's Game of Life steps translate the Life glider by (1,1)** Original computed toy configuration, not measured data. All five panels use fixed coordinates. Orange dashed outlines in the last panel mark the original live cells; blue cells show the computed fourth generation. The displayed window is part of an infinite board, not a finite boundary.

For an exact check of every frame, the intermediate live [sets](set-split.md) are

$$
\begin{aligned}
G_1&=\{(0,1),(2,1),(1,2),(2,2),(1,3)\},\\
G_2&=\{(2,1),(0,2),(2,2),(1,3),(2,3)\},\\
G_3&=\{(1,1),(2,2),(3,2),(1,3),(2,3)\},\\
G_4&=\{(2,1),(3,2),(1,3),(2,3),(3,3)\}=G_0+(1,1).
\end{aligned}
$$

Here $G_0+(1,1)$ means add $(1,1)$ to each [ordered pair](ordered-pair.md) in $G_0$. In the first step, the live cells $(1,0)$ and $(0,2)$ have respectively one and one live neighbors, so die; the other three have respectively three, three and two and survive. Exactly $(0,1)$ and $(1,3)$ are born, with three live neighbors each. This derives $G_1$ and explains how motion can occur while individual cells merely switch states.

Because the rule uses the same relative neighbors at every position, applying the global update [function](function-split.md) and applying a [translation](translation-geometry.md) commute. Thus $G_{t+4}=G_t+(1,1)$ for every generation $t$; the four-step calculation establishes continued motion on the infinite board. The average displacement is $(1/4,1/4)$ cells per generation, or [Euclidean distance](euclidean-distance.md) $\sqrt{2}/4$ per generation. The live-cell count happens to stay five in these frames, but the rule does not conserve live-cell count in general: a single isolated live cell dies immediately. The [Life glider](life-glider.md) persists indefinitely in an otherwise empty infinite board; encounters with other patterns or a finite implementation's edge can change that conclusion.

// Destination: computer-science.bigb

## ↑ Ancestors (3)

1. [Conway Game of Life](conway-game-of-life.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Conway Game of Life](conway-game-of-life.md)
- [Life glider](life-glider.md)
- [Life oscillator](life-oscillator.md)
- [One-row in-place Life update](one-row-in-place-life-update.md)
