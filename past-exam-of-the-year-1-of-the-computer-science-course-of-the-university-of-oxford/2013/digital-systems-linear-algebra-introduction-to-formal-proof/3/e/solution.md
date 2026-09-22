<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

A traditional UNIX-like [file system](../../../../../file-system-split.md) identifies a [computer file](../../../../../computer-file.md) by an [inode number](../../../../../inode-number.md). Its [inode](../../../../../inode.md) records [file metadata](../../../../../file-metadata.md), such as byte length, ownership and permissions, and contains direct [file data block](../../../../../file-data-block.md) addresses plus [indirect block pointers](../../../../../indirect-block-pointer.md). A [file-system directory](../../../../../file-system-directory.md) maps a name to the [inode number](../../../../../inode-number.md); the filename need not be stored inside the [inode](../../../../../inode.md).

In the familiar direct/single/double/triple scheme, a single [indirect block pointer](../../../../../indirect-block-pointer.md) reaches a block of data-block addresses, a double [indirect block pointer](../../../../../indirect-block-pointer.md) reaches blocks of those addresses, and a triple [indirect block pointer](../../../../../indirect-block-pointer.md) adds one more level. If there are $d$ direct pointers, one pointer of each indirect level, block size $B$ bytes and pointer width $h$ bytes, put $q=\lfloor B/h\rfloor$. The index structure can name

$$
K=d+q+q^2+q^3
$$

data blocks, giving

$$
\boxed{L_{\rm index}=B(d+q+q^2+q^3).}
$$

The actual maximum is the minimum of this structural bound, the representable [file offset](../../../../../file-offset.md)/length bound, the addressable data-block space, and the capacity left on the device after allocating metadata and index blocks. For an unsigned $\ell$-bit byte-length field, its bound is $2^\ell-1$ bytes. An empty [computer file](../../../../../computer-file.md) is permitted and needs no data blocks in this scheme. Exact numerical limits cannot be given without the [inode](../../../../../inode.md) layout and field widths; different UNIX-like implementations choose different layouts, and some use extent trees rather than this traditional scheme.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
