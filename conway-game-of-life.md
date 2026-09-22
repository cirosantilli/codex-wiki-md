# Conway Game of Life

↑ **Parent:** [Computer science](computer-science-split.md)

[Conway's Game of Life](conway-game-of-life.md) is a [cellular automaton](cellular-automaton.md) in which a simple local rule produces patterns that remain still, pulse, or travel across a square grid. Choose the starting pattern; after that there are no player decisions. The [Life blinker](life-blinker.md) and [Life glider](life-glider.md) below make the surprise concrete: the rule mentions only births and survival, yet repeated applications create a clock and a moving shape.

The standard board is infinite, with cells at [ordered pairs](ordered-pair.md) $(x,y)\in\mathbb Z^2$ of [integers](integer-split.md). At generation $t\in\{0,1,2,\ldots\}$ let $a_t(x,y)$ be $1$ for a live cell and $0$ for a dead cell. Count all eight cells sharing an edge or a corner, excluding the center itself:

$$
n_t(x,y)=\sum_{\substack{i,j\in\{-1,0,1\}\\(i,j)\ne(0,0)}}a_t(x+i,y+j).
$$

The local [Boolean function](boolean-function.md) defining the next generation is

$$
a_{t+1}(x,y)=\begin{cases}1,&n_t(x,y)=3,\\1,&a_t(x,y)=1\text{ and }n_t(x,y)=2,\\0,&\text{otherwise}.\end{cases}
$$

This is the rule `B3/S23`: a dead cell is born with exactly three live neighbors; a live cell survives with exactly two or three. A live cell with zero or one, or with four through eight, dies. A dead cell with two stays dead. All counts and center states come from generation $t$: this is a synchronous update, even if an [algorithm](algorithm-split.md) computes its cells one at a time.[Johnston and Greene, Conway's Game of Life: Mathematics and Construction, chapter 1: simultaneous updates and B3/S23 notation](https://github.com/nathanieljohnston/game-of-life-book/blob/master/early_life.tex)

In particular, the two births in the [Life blinker](life-blinker.md) do not help any other cell survive until the following generation. Writing each answer over its old value and then reading that new value for another count changes the rule. The simplest correct [algorithm](algorithm-split.md) reads one [array](array-data-structure.md) and writes the next generation into a second [array](array-data-structure.md); swap their roles after the entire step. The [one-row in-place Life update](one-row-in-place-life-update.md) achieves the same rule with less auxiliary storage by preserving the old values that later counts still need.

A finite implementation must specify its boundary convention. Holding all cells outside the rectangle permanently dead can destroy a [Life glider](life-glider.md) when it reaches the edge. Wrapping neighbor coordinates from one edge to the opposite edge allows interaction with patterns on the other side. Neither convention is the infinite board. The figures display finite windows into an infinite board initially dead everywhere except the stated live cells; the windows do not impose walls.

[Conway's Game of Life](conway-game-of-life.md) illustrates [emergence](emergence.md) in a precise, modest sense: the [Life glider](life-glider.md)'s motion is a collective pattern derived from local birth and death, without a motion command. It has [deterministic evolution](deterministic-evolution.md); visually surprising behavior introduces no random choices. Nor do the words "alive" and "dead" make it an experimentally validated model of [biology](biology-split.md). The beauty is that the same rule yields a stable four-cell square, the [Life blinker](life-blinker.md), and the [Life glider](life-glider.md): three qualitatively different behaviors from a handful of cells.

For the stable square, take the live [set](set-split.md) $\{(0,0),(1,0),(0,1),(1,1)\}$. Each live cell has three live neighbors, and every dead cell has at most two. The next generation is identical: this configuration is a [fixed point](fixed-point.md) of the global update [function](function-split.md). In contrast, the [Life blinker](life-blinker.md) returns after two generations, and the [Life glider](life-glider.md) returns only after allowing a [translation](translation-geometry.md).

The patterns are useful as small, exact checks of an [algorithm](algorithm-split.md): the square checks survival without births, the [Life blinker](life-blinker.md) checks births and deaths in one simultaneous step, and the [Life glider](life-glider.md) checks several steps and diagonal neighbors. More elaborate constructions can encode data and assemble [Boolean circuits](boolean-circuit.md); Johnston and Greene develop constructions that simulate arbitrary computation in their chapter 9. This is a statement about suitably designed patterns with enough space and time, not a claim that every starting pattern computes something useful or that a fixed finite board has unlimited [computer memory](computer-memory.md).[Johnston and Greene, chapter 9: universal computation constructions](https://github.com/nathanieljohnston/game-of-life-book/blob/master/universal_computation.tex)

Martin Gardner introduced [Conway's Game of Life](conway-game-of-life.md) to his Scientific American readers in October 1970, reporting that Conway selected the rules after experimentation with patterns. The aim was sustained, varied behavior rather than immediate extinction or trivially demonstrable unlimited growth. These were mathematical explorations of chosen rules.[Gardner, The fantastic combinations of John Conway's new solitaire game life, Scientific American 223, October 1970, pp. 120–123](https://www.ibiblio.org/lifepatterns/october1970.html)

Gardner's hands-on procedure is still a useful experiment: place black counters for the current live cells; mark doomed counters by stacking another black counter; mark births with white counters; finish checking before removing the doomed stacks and turning white counters black. Count only the original black occupants. Repeat with three adjacent counters to obtain the [Life blinker](life-blinker.md), then with the five coordinates of the [Life glider](life-glider.md). Recording each generation tests whether the procedure implements the rule; it does not measure a natural population.[Gardner, October 1970: two-color procedure for simultaneous births and deaths](https://www.ibiblio.org/lifepatterns/october1970.html)

**Table of contents**

- [Life oscillator](life-oscillator.md)
  - [Life blinker](life-blinker.md)
- [Life glider](life-glider.md)
- [One-row in-place Life update](one-row-in-place-life-update.md)

## ↑ Ancestors (2)

1. [Computer science](computer-science-split.md)
2. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Bit mask](bit-mask.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/10/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/10/c/solution.md)
