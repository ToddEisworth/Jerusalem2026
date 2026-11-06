## From almost disjoint families to coverings

Let $\lambda>\omega_2$ be singular of countable cofinality, and set

$$
R=\operatorname{Reg}\cap(\omega_2,\lambda),
\qquad
D=\operatorname{cf}_{\aleph_0}
\left(\prod R,<_{J_\lambda^{\mathrm{bd}}}\right).
$$

Here $D$ is the least cardinality of a family that bounds every countable subproduct modulo bounded subsets of $\lambda$.

Write $\mathrm{Fin}(\omega_1)=[\omega_1]^{<\omega}$, and define

$$
T_{\mathrm{Fin}(\omega_1)}(D)
=
\sup\left\{
|\mathcal G|:
\mathcal G\subseteq{}^{\omega_1}D
\text{ and }
g\neq h\in\mathcal G
\Longrightarrow
|\{\xi<\omega_1:g(\xi)=h(\xi)\}|<\aleph_0
\right\}.
$$

**Proposition.** If $\mathcal G\subseteq{}^{\omega_1}D$ is maximal subject to distinct members agreeing at only finitely many coordinates, then

$$
\operatorname{cov}(\lambda,\lambda,\omega_1,2)
\leq|\mathcal G|.
$$

Consequently,

$$
\operatorname{cov}(\lambda,\lambda,\omega_1,2)
\leq T_{\mathrm{Fin}(\omega_1)}(D).
$$

### A model-comparison lemma

Work in a sufficiently large structure

$$
\mathfrak H=(H(\chi),\in,\triangleleft),
$$

where $\triangleleft$ is a well-order, so that we have definable Skolem functions and canonical choices of witnesses.

**Lemma.** Suppose $N,M\prec\mathfrak H$, $\lambda\in N\cap M$, and $\mu<\lambda$ is an infinite cardinal with $\mu\subseteq M$. Assume that whenever

$$
\rho\in N\cap M\cap\operatorname{Reg},
\qquad
\mu<\rho<\lambda,
$$

the set $N\cap M\cap\rho$ is cofinal in $N\cap\rho$. Then

$$
N\cap\lambda\subseteq M.
$$

**Proof.** Suppose otherwise, and fix $\gamma\in N\cap\lambda\setminus M$. Choose

$$
A\in N\cap M,
\qquad
\gamma\in A\subseteq\lambda,
$$

with $\kappa=|A|$ as small as possible. Such an $A$ exists because $\lambda$ itself qualifies. By elementarity, $\kappa\in N\cap M$.

If $\kappa\leq\mu$, a canonical bijection $e:\kappa\to A$ belongs to $M$. Since $\kappa\subseteq M$, it follows that $A\subseteq M$, contradicting $\gamma\notin M$.

Suppose $\kappa>\mu$ is regular. Since $\lambda$ is singular, $\kappa<\lambda$. The canonical bijection $e:\kappa\to A$ belongs to both models, and

$$
\alpha=e^{-1}(\gamma)\in N\cap\kappa.
$$

Choose $\beta\in N\cap M\cap\kappa$ above $\alpha$. Then $e``\beta$ belongs to both models, contains $\gamma$, and has cardinality less than $\kappa$, contradicting minimality.

Finally, suppose $\kappa>\mu$ is singular. Choose canonically, in both models, an increasing decomposition

$$
A=\bigcup_{\eta<\tau}A_\eta,
\qquad
\tau=\operatorname{cf}(\kappa),
\qquad
|A_\eta|<\kappa.
$$

The least $\eta<\tau$ with $\gamma\in A_\eta$ belongs to $N$.

If $\tau\leq\mu$, then $\eta\in M$, so $A_\eta\in N\cap M$, contradicting minimality. If $\tau>\mu$, apply the common-trace hypothesis at the regular cardinal $\tau$ to choose $\zeta\in N\cap M\cap\tau$ above $\eta$. Then $A_\zeta\in N\cap M$ contains $\gamma$ and has cardinality less than $\kappa$, again a contradiction. $\square$

### The covering family

**Proof of the proposition.** Fix a witnessing family

$$
\bar f=\langle f_\alpha:\alpha<D\rangle\subseteq\prod R.
$$

Thus, for every countable $a\subseteq R$ and every $q\in\prod a$, there are $\alpha<D$ and $\mu<\lambda$ such that

$$
\rho\in a,\ \rho>\mu
\quad\Longrightarrow\quad
q(\rho)<f_\alpha(\rho).
\tag{1}
$$

Fix increasing cardinals

$$
\bar\mu=\langle\mu_n:n<\omega\rangle
$$

cofinal in $\lambda$, with $\omega_2<\mu_0$. Choose $\chi$ sufficiently large for all these parameters.

For $g\in\mathcal G$ and $n<\omega$, let

$$
M_{g,n}
=
\operatorname{Sk}_{\mathfrak H}
\left(
(\mu_n+1)
\cup\operatorname{ran}(g)
\cup\{\lambda,\bar f,\bar\mu\}
\right).
$$

The elements of $\operatorname{ran}(g)$ are included individually among the generators. Since $|\operatorname{ran}(g)|\leq\aleph_1$, we have

$$
|M_{g,n}|\leq\mu_n<\lambda.
$$

We will show that

$$
\mathcal C
=
\{M_{g,n}\cap\lambda:g\in\mathcal G,\ n<\omega\}
\tag{2}
$$

covers every countable subset of $\lambda$.

### Building the chain

Fix a countable $Y\subseteq\lambda$. Construct a continuous increasing chain

$$
\langle N_i:i<\omega_1\rangle
$$

of countable elementary submodels of $\mathfrak H$, with $Y\subseteq N_0$ and $\lambda,\bar f,\bar\mu\in N_0$.

At stage $i$, the set

$$
a_i=N_i\cap R
$$

is countable, and regularity gives

$$
q_i(\rho)=\sup(N_i\cap\rho)<\rho
\qquad(\rho\in a_i).
$$

Apply (1) and choose $\alpha_i<D$ and $n_i<\omega$ such that

$$
\rho\in N_i\cap R,\ \rho>\mu_{n_i}
\quad\Longrightarrow\quad
\sup(N_i\cap\rho)<f_{\alpha_i}(\rho).
\tag{3}
$$

Arrange that $\alpha_i\in N_{i+1}$. Since $\bar f\in N_{i+1}$, this ensures that

$$
\rho\in N_i\cap R
\quad\Longrightarrow\quad
f_{\alpha_i}(\rho)\in N_{i+1}\cap\rho.
\tag{4}
$$

At limit stages, take unions.

### Fixing the cutoff and obtaining infinite agreement

Since $\omega_1$ is regular, some $n^*<\omega$ has

$$
W=\{i<\omega_1:n_i=n^*\}
$$

unbounded in $\omega_1$. Enumerate $W$ increasingly as

$$
\langle i_\xi:\xi<\omega_1\rangle,
$$

and define $h\in{}^{\omega_1}D$ by

$$
h(\xi)=\alpha_{i_\xi}.
$$

By maximality of $\mathcal G$, there is $g\in\mathcal G$ such that

$$
\{\xi<\omega_1:g(\xi)=h(\xi)\}
$$

is infinite: otherwise $h$ could be added to $\mathcal G$.

Choose increasing matching coordinates $\langle\xi_k:k<\omega\rangle$, and put

$$
j_k=i_{\xi_k},
\qquad
\delta=\sup_{k<\omega}(j_k+1).
$$

Then $\delta<\omega_1$ is a limit ordinal, the sequence $\langle j_k:k<\omega\rangle$ is cofinal in $\delta$, and

$$
n_{j_k}=n^*,
\qquad
\alpha_{j_k}=g(\xi_k).
\tag{5}
$$

### Comparing the models

Set

$$
N=N_\delta,
\qquad
M=M_{g,n^*}.
$$

We verify the hypotheses of the model-comparison lemma. Certainly $\lambda\in N\cap M$ and $\mu_{n^*}\subseteq M$.

Let

$$
\rho\in N\cap M\cap\operatorname{Reg},
\qquad
\mu_{n^*}<\rho<\lambda.
$$

For all sufficiently large $k$, we have $\rho\in N_{j_k}$. Equations (3)–(5) give

$$
\sup(N_{j_k}\cap\rho)
<
f_{\alpha_{j_k}}(\rho)
=
f_{g(\xi_k)}(\rho)
\in N_{j_k+1}\cap M\cap\rho.
\tag{6}
$$

The value belongs to $M$ because

$$
g(\xi_k)\in\operatorname{ran}(g)\subseteq M
$$

and $\bar f,\rho\in M$. It belongs to $N_{j_k+1}$ by (4).

Since the $j_k$'s are cofinal in $\delta$, equation (6) shows that $N_\delta\cap M\cap\rho$ is cofinal in $N_\delta\cap\rho$. The model-comparison lemma therefore gives

$$
Y\subseteq N_\delta\cap\lambda
\subseteq M_{g,n^*}\cap\lambda.
$$

Thus $\mathcal C$ covers every countable subset of $\lambda$.

A maximal family $\mathcal G$ is infinite, so

$$
|\mathcal C|
\leq|\mathcal G|\cdot\aleph_0
=|\mathcal G|.
$$

Every member of $\mathcal C$ has cardinality less than $\lambda$, and hence

$$
\operatorname{cov}(\lambda,\lambda,\omega_1,2)
\leq|\mathcal G|.
$$

This proves the proposition. $\square$

**Remark.** The order of the selections matters. We first find $\omega_1$ many stages with a common cutoff, and only then use maximality to obtain infinitely many matching stages. Those stages are cofinal in a countable limit $\delta$, and the model $N_\delta$ already contains $Y$. Thus finite intersections suffice for the almost disjointness argument.