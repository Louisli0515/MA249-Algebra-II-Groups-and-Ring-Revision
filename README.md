# MA249-Algebra-II-Groups-and-Ring-Revision
My own notes about the MA249 Algebra II: Groups and Rings revision, mainly from the notes and example sheets

## Lecture notes

[ma249-notes.pdf](https://github.com/Louisli0515/MA249-Algebra-II-Groups-and-Ring-Revision/files/11467501/ma249-notes.pdf)

First thing first, feel free to download the 2022-2023 lecture notes for MA249 Algebra II Groups and Rings.

## Example sheets

### Order of Groups, Orders of Elements

* Let $G$ be a group. The number of elements in $G$ is called the ***order*** of $G$ and is denoted by $|G|$. This may be finite or infinite.
* Let $g\in G$, then the ***order*** of $g$, denoted by $|g|$ is the least integer $n > 0$ such that $g^{n} = 1$, if such an $n$ exists. If there is no such $n$, then $g$ has infinite order and we write $|g| = \infty$.

#### Lemma about order of elements

* $|g| = 1$ if and only if $g = 1$.
* If $|g| = n$, then for $k\in\mathbb{Z}$, $g^{k} = 1$ if and only if $n\vert k$.

### Cyclic Groups

* A group $G$ is called ***cyclic*** if it consists of the integral powers of a single element. i.e. for every $h\in G$, there exists $k\in\mathbb{Z}$ with $g^{k} = h$. The element $g$ is called a ***generator*** of $G$.
* In an infinite cyclic group, every generator $g$ has infinite order. In a finite cyclic group of order $n$, every generator $g$ has order $n$.

### $\mathbb{Z}_ {n}$ group

* $\mathbb{Z}_ {n} = \set{0,1,2,...,n-1}$, forming a group under the operation of ***addition*** modulo $n$.
