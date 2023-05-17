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

### Direct Products and Groups of Order 4

#### Direct product

* Let $G$ and $H$ be two (multiplicative) groups. The ***direct product*** $G\times H$ of $G$ and $H$ ot be the set $\set{(g,h)\vert g\in G, h\in H}$ of ordered pairs of elements from $G$ and $H$, with the obvious component-wise multiplication of elements $(g_{1}, h_{1})(g_{2}, h_{2}) = (g_{1}g_{2}, h_{1}h_{2})$ for $g_{1},g_{2}\in G$ and $h_{1}, h_{2}\in H$.

#### Groups of order 4

* A group of order 4 is isomorphic either to a ***cyclic group*** $C_{4}$ or to a ***Klein Four Group*** $C_{2}\times C_{2}$.

#### Groups of order $p$

* Let $G$ be a group having ***prime order*** $p$. Then $G$ is ***cyclic***, that is, $G\cong C_{P}$.

#### Groups of order 6

* Let $G$ be a group of order 6. Then $G\cong C_{6}$ or $G\cong D_{3}$.

### Generators

* The elements $\set{g_{1},g_{2},...,g_{r}}$ of a group $G$ are said to ***generate*** $G$ if every element of $G$ can be obtained by repeated multiplication of $g_{i}$ and ***their inverses***.
* A group is ***cyclic*** if and only if it can be ***generated*** by a single element.
* Let $G$ be a group of order $2n$ generated by two elements $a$ and $b$ that satisfy the equations $a^{n} = 1, b^{2} = 1$ and $ba = a^{-1}b$. Then $G\cong D_{n}$.

### Defining relations

* The equations $\set{a^{n} = 1,b^{2} = 1, ba = a^{-1}b}$ are called ***defining relations*** for $D_{n}$, which means roughly that $D_{n}$ is the ***largest group generated*** by two elements $a$ and $b$ that satisfy these equations.

#### Groups of order $mn$

* Let $G$ be a group of order $mn$ generated by two elements $a$ and $b$ that satisfy the equations $a^{m} = 1, b^{n} = 1$ and $ba = ab$. Then $G\cong C_{m}\times C_{n}$.

#### Groups of order 8

* Let $G$ be a group of order 8 generated by two elements $a$ and $b$ that satisfy the equations $a^{4} = 1, b^{2} = a^{2}$ and $ba = a^{-1}b$. Then $G\cong Q_{8}$.
* Let $G$ be a group of order 8. Then $G$ is ***isomorphic*** to one of $C_{8}, C_{4}\times C_{2}, C_{2}\times C_{2}\times C_{2}, D_{4}$ and $Q_{8}$.
* $Q_{8}$ is known as the ***quaternion group***, where we can define as the subgroup of $GL(2,\mathbb{C})$$: 

```math
1 = \begin{pmatrix} 1 & 0 \\
 0 & 1\end{pmatrix}\quad a = \begin{pmatrix} 0 & 1\\ -1 & 0\end{pmatrix}\quad a^{2} = \begin{pmatrix} -1 & 0\\ 0 & -1\end{pmatrix}\quad a^{3} = \begin{pmatrix} 0 & -1\\ 1 & 0\end{pmatrix},
```

```math
b  = \begin{pmatrix} i & 0 \\ 0 & -i\end{pmatrix}\quad ab = \begin{pmatrix} 0 & -i\\ -i & 0\end{pmatrix}\quad a^{2}b = \begin{pmatrix} -i & 0\\ 0 & i\end{pmatrix}\quad a^{3}b = \begin{pmatrix} 0 & i\\ i & 0\end{pmatrix}.
```

### Homomorphisms and Quotient Groups

#### Quotient Groups

* Let $N$ be a ***normal subgroup*** of a group $G$, and let $g,h\in G$. Then the product of any element in the coset $gN$ with any element in the coset $hN$ is equal to an element in the coset $ghN$.
* If $N$ is a ***normal subgroup*** of $G$ and $gN,hN$ are cosets of $N$ in $G$, then $(gN)(hN) = ghN$.
* Let $N$ be a ***normal subgroup*** of a group $G$. Then the set $G/N$ of left cosets $gN$ of $N$ in $G$ forms a group under multiplication of sets.
* The group $G/N$ is called the ***quotient group*** of $G$ by $N$.
* If $G$ is finite, then $$|G/N| = |G:N| = |G|/|N|.$$

#### Homomorphisms

* Let $G$ and $H$ be groups. A ***homomorphism*** $\phi$ from $G$ to $H$ is a map $\phi:G\to H$ such that $\phi(g_{1}g_{2}) = \phi(g_{1})\phi(g_{2})$ for all $g_{1},g_{2}\in G$.
* An ***injective homomorphism*** is called a ***monomorphism***, i.e. if $\phi(g_{1}) = \phi(g_{2})\implies g_{1} = g_{2}.$
* A ***surjective homomorphism*** is called an ***epimorphism***, i.e.  $\text{im}(\phi)\in H$.
* An ***isomorphism*** is a homomorphism $\phi$ which is a ***bijection***.

### Kernels and Images

* Let $\phi:G\to H$ be a ***homomorphism***. Then the ***kernel*** $\ker(\phi)$ of $\phi$ is defined to be the set of elements of $G$ that map onto $1_{H}$, i.e. $$\ker(\phi) = \set{g\in G:\phi(g) = 1_{H}}.$$ Note that $\ker(\phi)$ always contains $1_{G}$.

#### Homomorphisms lemma

* Let $\phi:G\to H$ be a ***homomorphism***. Then $\phi(1_{G}) = 1_{H}$ amd $\phi(g^{-1}) = \phi(g)^{-1}$ for all $g\in G$.
* Let $\phi:G\to H$ be a ***homomorphism***. Then $\phi$ is ***injective*** if and only if $\ker(\phi) = \set{1_{G}}.$
* Let $\phi:G\to H$ be a ***homomorphism***. Then $\ker(\phi)$ is a ***normal subgroup*** of $G$.
* Let $N$ be a ***normal subgroup*** of a group $G$. Then the map $\pi:G\to G/N$ defined by $\pi(g) = gN$ is a ***homomorphism*** with kernel $N$.
* Let $\phi:G\to H$ be a ***homomorphism***. Then $\text{im}(\phi)$ is a ***subgroup*** of $H$.

### The Isomorphism Theorems

#### First Isomorphism Theorem

* Let $\phi:G\to H$ be a ***homomorphism*** with ***kernel*** $K$. Then $G/K\cong\text{im}(\phi)$. More precisely, there is an ***isomorphism*** $\overline{\phi}: G/K\to\text{im}(\phi)$ defined by $\overline{\phi}(gK) = \phi(g)$ for all $g\in G$.

#### Second Isomorphism Theorem

Let $G$ be a group. Let $H$ be any subgroup and let $K$ be a normal subgroup of a group $G$. Then the following conditions hold:

* $HK = KH$ is a ***subgroup*** of $G$,
* $H\cap K$ is a ***normal subgroup*** of $H$, and 
* $H/(H\cap K)\cong HK/K$.

#### Third Isomorphism Theorem

Let $K\subseteq H\subseteq G$, where $K$ and $H$ are both ***normal subgroups*** of $G$. Then:

* $K$ is a ***normal subgroup*** of $H$.
* $H/K$ is a ***normal subgroup*** of $G/K$.
* $(G/K)/(H/K)\cong G/H$.

### Group Actions

Let $G$ be a group and $X$ a set. An ***action*** of $G$ on $X$ is a map $\cdot$: $G\times X\to X$, which satisfies the properties:

* $1_{G}\cdot x = x$ for all $x\in X$.
* $(gh)\cdot x = g\cdot(h\cdot x)$ for all $g,h\in G, x\in X$.

This is also defined as a ***left action***, while a ***right action*** can be defined as a map $X\times G\to X$ satisfying analogous properties.

#### Kernel of an action

* The ***kernel*** of an action $\cdot$ of $G$ on $X$ is defined to be the kernel $K = \ker(\phi)$ of the ***homomorphism*** $\phi:G\to\text{Sym}(X)$. So $$K = \set{g\in G\vert g\cdot x = x,\forall x\in X}.$$
* The action is said to be ***faithful*** if $K = \set{1}.$

#### Cayley's Theorem

* Every group $G$ is ***isomorphic*** to a ***permutation group***. 

### Orbits and Stabilisers

#### Orbits

* Let $\cdot$ be an action of $G$ act on $X$. We define a relation $\sim$ on $X$ by $x\sim y$ if and only if there exists a $g\in G$ with $y = g\cdot x$. The equivalence classes of $\sim$ are called the ***orbits*** of $G$ on $X$. In particular, the orbit of a specific element $x\in X$, which is denoted by $G\cdot x$ or by $\text{Orb}_ {G}(x)$ is $$G\cdot x = \text{Orb}_ {G}(x) = \set{y\in X:\text{there exists} g\in G\text{with}g\cdot x = y} = \set{g\cdot x:g\in G}.$$
* An action of $G$ on $X$ is ***transitive*** if it has only a single orbit. Equivalently, an action is ***transitive*** if for every $x,y\in X$, there is some $g\in G$ such that $g\cdot x = y$.

#### Stabiliser

* Let $G$ act on $X$ and let $x\in X$. Then the ***stabiliser*** of $x$ in $G$, denoted by $G_{x}$ or $\text{Stab}_ {G}(x)$, is $$\set{g\in G:g\cdot x = x}.$$ That is, the subset of $G$ comprising all elements that leave $x$ fixed.
* The stabiliser is not just a subset of $G$, but actually a ***subgroup***.
* Let $G$ act on $X$ and $x\in X$. Then $\text{Stab}_ {G}(x)$ is a subgroup of $G$ and $\cap_{x\in X}\text{Stab}_ {G}(x)$ is the ***kernel*** of the action of $G$ on $X$.

#### The Orbit-Stabiliser Theorem

* Let a finite group $G$ act on $X$, and let $x\in X$. Then $|G| = |\text{Orb}_ {G}(x)|\times |\text{Stab}_ {G}(x)|.$

### Conjugation Action and Conjugacy Classes

* Another important action of $G$ on $X = G$, which is defined by $$g\cdot x = gxg^{-1}$$for $g,x\in G$. This action is called ***conjugation***.
* The orbits of the action are called the ***conjugacy classes*** of $G$, and elements in the same conjugacy class are said to be ***conjugate*** in $G$.
* So $g,h\in G$ are conjugate if and only if there exists $f\in G$ with $h = fgf^{-1}$. We will write $\text{Cl}_ {G}(g)$ for the orbit of $g$, that is the conjugacy class containing $g$. Thus, $$\text{Cl}_ {G}(g) = \set{xgx^{-1}\vert x\in G}.$$

#### Centraliser

* The ***centraliser*** of $g$ in $G$ is written as $C_{G}(g)$, that is, $$C_{G}(g) = \set{x\in G\vert gx = xg}.$$
* Let $G$ be a finite group and let $g\in G$. Then $|\text{Cl}_ {G}(g)| = |G|/|C_{G}(g)|.$

#### Centre
* The kernel $K$ of the action consists of those $f\in G$ that fix and hence commute with all $g\in G$. This is called the ***centre*** of $G$ and is denoted by $Z(G)$. So we have $$Z(G) = \set{f\in G:fg = gf\quad\forall g\in G}.$$
* Note that $g\in Z(G)$ if and only if $\text{Cl}_ {G}(g) = \set{g}.$

### Conjugacy Classes in Alternating Groups

* Let $G = S_{n}$ and $H = A_{n}$. Let $h\in H$, then $\text{Cl}_ {H}(h) = \text{Cl}_ {G}(h)$ or $|\text{Cl}_ {H}(h)| = \frac{1}{2}|\text{Cl}_ {G}(h)|.$

### Simple Groups

* A group $G$ with $|G| > 1$ is called ***simple*** if its only normal subgroups are $G$ and $\set{1}$.
* A ***simple abelian group*** is ***cyclic*** of ***prime order***.
* A subgroup $H$ of a group $G$ is ***normal*** in $G$ if and only if $H$ consists of a union of ***conjugacy classes*** of $G$.
* The group $A_{5}$ is ***simple***.

### Sylow's subgroup

* Let $G$ be a finite group of order $p^{n}\cdot m$, where $n$ is the largest power of the prime $p$ that divides $|G|$, so $m$ is not divisible by $p$. A subgroup of $G$ of order $p^{n}$ is called a ***Sylow p-subgroup*** of $G$.

#### Sylow's Theorem

Let $G$ be a finite group, $p$ is prime, and $|G| = p^{n}m$, where $p \not\vert m$. Then 

* $G$ has a Sylow p-subgroup, and any subgroup of $G$ of order $p^{a}$ for $1\leq a\leq n$ is ***contained*** in a Sylow p-subgroup of $G$.
* Any ***two*** Sylow p-subgroups of $G$ are ***conjugate*** in $G$.
* The number $r$ of Sylow p-subgroups of $G$ satisfies $r\equiv 1(\mod p)$ and $r\vert m$.

#### Sylow's Theorem 2

* Sylow's second theorem says any two Sylow p-subgroups of $G$ are ***conjugate*** in $G$, and here conjugate means there is a homomorphism $\phi:G\to\text{Sym}(X)$ and $\text{Sym}(X)\cong S_{|X|}$.

#### Applications of Sylow's Theorem

* Let $G$ be a group of order $p^{n}m$ with $n\geq 1$ and $p \not\vert m$. Let $$\text{Syl}_ {p}(G) = \set{H\leq G\vert|H| = p^{n}}$$ be the set of Sylow p-subgroups of $G$.
* If $P\in\text{Syl}_ {p}(G)$ and $g\in G$, then $gPg^{-1}\in\text{Syl}_ {p}(G)$.
* $|\text{Syl}_ {p}(G)|$ divides $m = |G|/|P|$.
* If there is only one Sylow p-subgroup of $G$, then it is ***a normal subgroup*** of $G$.
* There are ***no simple groups*** of order 24.

### Rings and Subrings

#### Definition of a ring

A ***ring*** is a set $R$ together with two binary operations $+,\cdot:R\times R\to R$ that satisfy the following properties:

* $(R,+)$ is an ***abelian group***.
* $(ab)c = a(bc)$ for all $a,b,c\in R$.
* $(a+b)c = ac+bc$ and $a(b+c) = ab+ac$ for all $a,b,c\in R$.
* There exists an element $1 = 1_{R}\in R$ such that $1a = a1 = a$ for all $a\in R$.

#### Commutative ring

* A ring $R$ is ***commutative*** if it satisfies $$ab = ba$$for all $a,b\in R$.
* $\mathbb{Z},\mathbb{Q},\mathbb{R} and \mathbb{C}$ are all ***commutative rings*** with their usual addition and multiplication.
* $\mathbb{Z}_ {n}$ is a ***commutative ring*** under addition and multiplication modulo $n$, for every positive integer $n$.

#### Definition of subrings

* A subset $S$ of a ring $R$ is called a ***subring*** of $R$ if it forms a ring under the same operations as $R$ with the same ***identity element***.

#### Subring proposition

Let $R$ be a ring and let $S$ be a subset of $R$. Then $S$ is a ***subring*** of $R$ if and only if 

* $S$ is a subgroup of $(R,+)$.
* $a_{1},a_{2}\in S\implies a_{1}a_{2}\in S$ and 
* $1_{R}\in S$.

#### Intersection

* The intersection of any set of subrings of $R$ is itself a subring.

### Isomorphisms and direct products

#### Isomorphism definition

A map $\phi:R\to S$ between two rings $R$ and $S$ is an ***isomorphism*** if 

* $\phi$ is a ***bijection***.
* $\phi(r_{1} + r_{2}) = \phi(r_{1})+\phi(r_{2})$ for all $r_{1},r_{2}\in R$ and 
* $\phi(r_{1}r_{2}) = \phi(r_{1})\phi(r_{2})$ for all $r_{1},r_{2}\in R$.

Two rings $R$ and $S$ are called ***isomorphic*** if there is an isomorphism between them.

#### Isomorphism Lemmas

Let $R$ and $S$ be rings, and $\phi:R\to S$ an ***isomorphism***. Then the following conditions hold:

* $\phi(0_{R}) = 0_{S}$.
* $\phi(1_{R}) = 1_{S}$.

#### Direct product definition

Let $R$ and $S$ be two rings. We define the ***direct product*** $R\times S$ of $R$ and $S$ to be the set $$\set{(r,s)\vert r\in R, s\in S}$$ of ordered pairs of elements from $R$ and $S$, with the obvious component-wise addition and multiplication $$(r_{1},s_{1}) + (r_{2},s_{2}) = (r_{1} + r_{2}, s_{1}+s_{2}),$$ and $$(r_{1},s_{1})(r_{2},s_{2}) = (r_{1}r_{2},s_{1}s_{2})$$ for $r_{1},r_{2}\in R$ and $s_{1},s_{2}\in S$.

#### Sun Tzu's Theorem

* The rings $\mathbb{Z}_ {m}\times\mathbb{Z}_ {n}$ and $\mathbb{Z}_ {mn}$ are ***isomorphic*** if and only if $m$ and $n$ are ***coprime***.

#### Direct product lemmas

* If $n = p_{1}^{a_{1}}...p_{k}^{a_{k}}$ is a ***decomposition*** of $n$ into a product of distinct primes then $$\mathbb{Z}_ {n}\cong \mathbb{Z}_ {p_{1}^{a_{1}}}\times...\times\mathbb{Z}_ {p_{k}^{a_{k}}}$$ as rings.

### Integral domains and fields

#### Definition of zero divisors and integral domain

* If $a$ and $b$ are non-zero elements of a ring $R$ with $ab = 0$, then $a$ and $b$ are called ***zero divisors***.
* A ring $R$ is called an ***integral domain*** (or just domain) if $R$ is ***commutative, nonzero*** and ***has no zero divisors***, that is if $a,b\in R, ab = 0$ implies $a = 0$ or $b = 0$.
* The rings $\mathbb{Z},\mathbb{Q},\mathbb{R}$ and $\mathbb{C}$ are all ***integral domains***.
* $\mathbb{Z}_ {n}$ is a ***domain*** if and only if $n$ is ***prime***.

#### Definition of unit

* An element $a$ of a ring $R$ is called a ***unit*** if it has a ***two-sided inverse*** under multiplication; that is, if there exists $b\in R$ with $ab = ba = 1$.

#### Definition of division ring and field

* A non-zero ring $R$ is called a ***division ring*** if $R\setminus\set{0}$ is a group under multiplication; that is, if all of its non-zero elements are units.
* A ***field*** is a ***commutative division ring***.
* Every ***field*** is an ***integral domain***.
* A ***finite integral domain*** is a ***field***.

#### Definition of characteristic 

* Let $R$ be a ring. If there exists a positive integer $n$ such that $nx = 0$ for all $x\in R$, then we call the smallest such positive integer is the ***characteristic*** of $R$. If there is no such positive integer, then we say the charateristic of $R$ is 0.
* $\mathbb{Z}_ {n}$ has characteristic $n$.
* $\mathbb{Z}$ and $\mathbb{Q}$ have characteristic 0.
* The polynomial ring $R[x]$ has the ***same characteristic*** as $R$.

### Polynomials

#### Polynomials Lemma

* If $R$ is an integral domain, then so is $R[x]$.
* If $R$ is ***an integral domain***, then the units in $R$ and in $R[x]$ are the ***same***.

#### Polynomial division with remainder

* For any $f,g\in F[x]$ with $0\ne g$, there exists $q,r\in F[x]$ with $f = qg + r$, where either $r = 0$ or $\deg(r) < \deg(g).$

#### Remainder Theorem

* Let $f = f(x)\in F[x]$. Then for $a\in F$, $f(a) = 0$ if and only if $(x-a)$ divides $f$.

### Ideals and Quotient Rings

#### Homomorphisms

Let $R$ and $S$ be rings. A ***ring homomorphism*** $\phi$ from $R$ to $S$ is a function $\phi:R\to S$ that satisfies the following conditions:

* $\phi(r_{1}+r_{2}) = \phi(r_{1})+\phi(r_{2})$ for all $r_{1},r_{2}\in R$,
* $\phi(r_{1}r_{2}) = \phi(r_{1})\phi(r_{2})$ for all $r_{1},r_{2}\in R$ and 
* $\phi(1_{R}) = 1_{S}$.

#### Kernel and image

* The ***image*** $\text{im}(\phi)$ of a ring homomorphism is just its image as a function: $$\text{im}(\phi) = \set{\phi(r)| r\in R}.$$
* The ***kernel*** $\ker(\phi)$ of a ring homomorphism is defined to be its kernel as a homomorphism of additive groups. That is, $$\ker(\phi) = \set{r\in R|\phi(r) = 0_{S}}.$$
* $\phi$ is ***injective*** if and only if $\ker(\phi) = \set{0}.$

#### Ideals

A subset $I$ of a ring $R$ is called an ***ideal*** in $R$ if 

* $I$ is a ***subgroup*** of $(R,+)$;
* For all $x\in R$ and $y\in I$, we have $xy\in I$ and $yx\in I$.

#### Ideal lemmas

* An ideal $I$ of $R$ contains $1_{R}$ only when $I = R$.
* Let $\phi:R\to S$ be a ring homomorphism. Then $\ker(\phi)$ is an ***ideal*** in $R$.
* If $I$ and $J$ are ideals of $R$, then so is $I+J = \set{i+j|i\in I,j\in J}.$

#### Principal ideal

* When $R$ is a commutative ring, the subset $$(a) = \set{ra|r\in R}$$ consists of all multiples of $a$ in $R$, is an ideal of $R$. It is known as the ***principal ideal*** generated by $a$. 
* It is often written as $aR$ or $Ra$.


### Quotient Rings

* The ***cosets*** of an ideal form a ***ring*** under addition in the quotient group and the multiplication $(I+a)(I+b) = I+ab$.

#### First Isomorphism Theorem for Rings

* Let $\phi:R\to S$ be a ring homomorphism with kernel $I$. Then $R/I\cong\text{im}(\phi)$. More precisely, there is an ***isomorphism*** $\overline{\phi}: R/I\to\text{im}(\phi)$ defined by $\overline{\phi}(I+a) = \phi(a)$ for all $a\in R$.

### Domains

* A domain $R$ is called a ***principal ideal domain*** if every ideal of $R$ is principal.
* For every field $F$, the polynomial ring $F[x]$ is a ***principal ideal domain***.

#### Divisibility in integral domains

The following statements are equivalent for $x,y\in R$.

* $x\vert y$;
* $y\in (x)$;
* $(x)\supseteq (y)$.
