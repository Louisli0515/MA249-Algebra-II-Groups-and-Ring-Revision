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
* All cyclic groups are ***abelian***.

### $\mathbb{Z}_ {n}$ group

* $\mathbb{Z}_ {n} = \set{0,1,2,...,n-1}$, forming a group under the operation of ***addition*** modulo $n$.

### Isomorphisms and Isomorphic groups

* An ***isomorphism*** $\phi:G\to H$ between two groups $G$ and $H$ is a bijection from $G$ to $H$ such that $\phi(g_{1}g_{2}) = \phi(g_{1})\phi(g_{2})$ for all $g_{1},g_{2}\in G$. 
* Two groups $G$ and $H$ are called ***isomorphic*** if there is an isomorphism between them. In this case we write $G\cong H$.

#### Isomorphism lemmas

* If $\phi:G\to H$ is an ***isomorphism***, then $\phi(1_{G}) = 1_{H}$ and $\phi(g^{-1}) = \phi(g)^{-1}$ for all $g\in G$.
* If $\phi:G\to H$ is an ***isomorphism***, then $|g| = |\phi(g)|$ for all $g\in G$.

### Permutation Groups

If $a_{1},...,a_{r}$ are distinct elements of $X$, then the ***cycle*** $(a_{1},a_{2},...,a_{r})$ denotes the permutation $\phi\in\text{Sym}(X)$ with 

* $\phi(a_{i}) = a_{i+1}$ for $1\leq i< r$.
* $\phi(a_{r}) = a_{1}$ and
* $\phi(b) = b$ for $b\in X\setminus\set{a_{1},a_{2},...,a_{r}}$.

#### Permutation lemmas

* A permutation is called ***even*** if it is a product of an even number of transpositions, and ***odd*** if it is a product of an odd number of transpositions.
* A cycle of ***even length*** is ***odd*** and a cycle of ***odd length*** is ***even***. The product is seen as ***additivity*** when determining even or odd, e.g. when there are three 3-cycle with ***odd length***, then each cycle is ***even*** and the product of it is ***even***.

### Dihedral Groups

* The ***dihedral group*** of order $2n$ consists of the isometries of $P$, where $P$ is a regular $n$-sided polygon in the plane.
* $n$ reflections of $P$ are the elements $a^{k}b$ for $0\leq k < n$. Thus we have $$G = \set{a^{k}|0\leq k < n}\cup\set{a^{k}b|0\leq k < n}.$$

### Subgroups

* A subset $H$ of a group $G$ is called a ***subgroup*** of $G$ if it forms a group under the same operation as that of $G$.
* If $H$ is a subgroup of $G$, we write $H\leq G$.

#### Subgroup lemmas

* If $H$ is a subgroup of $G$, then the identity element $1_{H}$ of $H$ is equal to the identity element $1_{G}$ of $G$.
* Let $G$ be a group, $H\leq G$ and $K\leq G$, then $H\cap K$ is itself a ***subgroup*** of $G$.

Let $H$ be a non-empty subset of a group $G$. Then $H$ is a subgroup of $G$, if and only if 

* $h_{1},h_{2}\in H\implies h_{1}h_{2}\in H$ and 
* $h\in H\implies h^{-1}\in H$.

### Cosets and Lagrange's Theorem

* Let $g\in G$, then the ***left coset*** $gH$ is the subset $\set{gh|h\in H}$ of $G$. Similarly, the ***right coset*** $Hg$ is the subset $\set{hg|h\in H}$ of $G$.

#### Cosets lemma

The following are equivalent for $g,k\in G$:

* $k\in gH$;
* $gH = kH$;
* $g^{-1}k\in H$.

#### Lagrange's Theorem

* Let $G$ be a finite group and $H$ a ***subgroup*** of  $G$. Then the ***order*** of $H$ ***divides*** the ***order*** of $G$.
* Let $G$ be a finite group. Then for any $g\in G$, the order $|g|$ of $g$ divides the order $|G|$ of $G$.

#### Index

* The number of ***distinct left cosets*** of $H$ in $G$ is called the ***index*** of $H$ in $G$ and it's written as $|G:H|$.
* Let $G$ be a finite group and $H$ a subgroup of $G$. Then $$|G| = |H|\cdot|G:H|.$$

### Normal Subgroups

* A subgroup $H$ of a group $G$ is called ***normal*** in $G$ if $gH = Hg$ for all $g\in G$.

#### Normal subgroups lemma

* If $G$ is any group and $H$ is a subgroup with $|G:H| = 2$, then $H$ is a ***normal subgroup*** of $G$.
* Let $H$ be a ***subgroup*** of the group $G$. Then $H$ is ***normal*** in $G$ if and only if $ghg^{-1}\in H$ for all $g\in G$ and $h\in H$.
