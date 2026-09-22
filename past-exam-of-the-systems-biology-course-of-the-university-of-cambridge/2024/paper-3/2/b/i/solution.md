<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**TODO: Complete the data-specific numerical results and diagnostics when the original `Iris_data.csv` is available.**

The estimate requested is the [sample mean](../../../../../../sample-mean.md), **$\boxed{\bar x=n^{-1}\sum_i x_i}$**. The named electronic file `Iris_data.csv` is not present in the supplied source archive or this repository, and its measurements are not printed in the paper. Consequently its numerical [sample mean](../../../../../../sample-mean.md) cannot be recovered from the paper alone. The familiar built-in iris data must not be silently substituted: the question does not identify those observations as its sample.

The following R code reads the actual file and prints its [sample mean](../../../../../../sample-mean.md). The later code blocks in Question 2 continue this same script and use the resulting `x`, `n` and `xbar`.

```
dat <- read.csv("Iris_data.csv", check.names = FALSE)
# Recognize common labels, or a single measurement column.
keys <- tolower(gsub("[^[:alnum:]]", "", names(dat)))
j <- which(keys %in% c("sepallength", "sepallengthcm", "x"))
if (length(j) == 0L && ncol(dat) == 1L) j <- 1L
if (length(j) != 1L) {
  stop("Select the sepal-length column explicitly after inspecting names(dat).")
}
x <- dat[[j]]
stopifnot(is.numeric(x), length(x) > 0L, all(is.finite(x)))
n <- length(x)
xbar <- mean(x)
cat("n =", n, " sample mean =", format(xbar, digits = 12), "\n")
```

This reader assumes a header row and one observation per row. An alternative layout should be identified explicitly rather than dropping measurements or treating an identifier column as a length.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [2024](../../../../split.md)
6. [Past exam of the systems biology course of the University of Cambridge](../../../../../split.md)
7. [Systems Biology course of the University of Cambridge](../../../../../../systems-biology-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
