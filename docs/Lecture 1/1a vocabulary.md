# Reduced Product Vocabulary

Throughout, $I$ is a proper ideal on a cardinal $\kappa$, and
$\langle \lambda_i : i<\kappa\rangle$ is a sequence of cardinals.

## Order Modulo an Ideal

For functions $f,g$ with domain $\kappa$, write

$$
f<_I g
$$

if

$$
\{i<\kappa:g(i)\leq f(i)\}\in I.
$$

Thus $f<_I g$ means that $f(i)<g(i)$ for all $i<\kappa$ outside an $I$-small set.

Similarly,

$$
f\leq_I g
$$

means

$$
\{i<\kappa:f(i)>g(i)\}\in I.
$$

## Positive Sets

The collection of $I$-positive sets is

$$
I^+=\mathcal P(\kappa)\setminus I.
$$

Thus $B\in I^+$ means that $B$ is not $I$-small.

## Restriction of an Ideal

If $B\in I^+$, we regard $I\upharpoonright B$ as an ideal on $\kappa$, defined by

$$
I\upharpoonright B
=
\{A\subseteq\kappa:A\cap B\in I\}.
$$

Thus comparison modulo $I\upharpoonright B$ depends only on the coordinates in $B$.

## True Cofinality

Let

$$
P=\left(\prod_{i<\kappa}\lambda_i,<_I\right).
$$

We say that

$$
\operatorname{tcf}(P)=\theta
$$

if $\theta$ is regular and there is a sequence

$$
\langle f_\alpha:\alpha<\theta\rangle
$$

which is $<_I$-increasing and cofinal in $P$.

Equivalently,

$$
\alpha<\beta<\theta
\quad\Longrightarrow\quad
f_\alpha<_I f_\beta,
$$

and for every $g\in\prod_{i<\kappa}\lambda_i$, there is some $\alpha<\theta$ such that

$$
g<_I f_\alpha.
$$

## Limit Modulo an Ideal

We write

$$
\operatorname{tlim}_I\lambda_i=\lambda
$$

if, for every $\mu<\lambda$,

$$
\{i<\kappa:\lambda_i<\mu\}\in I.
$$

Thus the sequence $\langle\lambda_i:i<\kappa\rangle$ converges to $\lambda$ modulo $I$.

## Directedness

A partial order $P$ is **$\theta$-directed** if every subset of $P$ of cardinality less than $\theta$ has an upper bound.

Thus

$$
\left(\prod_{i<\kappa}\lambda_i,<_I\right)
$$

is $\theta$-directed if every family

$$
\{f_\alpha:\alpha<\delta\}
\subseteq
\prod_{i<\kappa}\lambda_i,
\qquad
\delta<\theta,
$$

has an upper bound modulo $I$.

## The Bounded Ideal

For an infinite cardinal $\kappa$, the bounded ideal on $\kappa$ is

$$
J_\kappa^{\mathrm{bd}}
=
\{A\subseteq\kappa:\sup A<\kappa\}.
$$

Thus

$$
f<_{J_\kappa^{\mathrm{bd}}}g
$$

means that

$$
f(i)<g(i)
$$

for all sufficiently large $i<\kappa$.

## Scales

Suppose

$$
\operatorname{tcf}\left(
\prod_{i<\kappa}\lambda_i,
<_{J_\kappa^{\mathrm{bd}}}
\right)=\theta.
$$

A sequence

$$
\langle f_\alpha:\alpha<\theta\rangle
$$

witnessing this true cofinality is called a **scale of length $\theta$** in the product
$\prod_{i<\kappa}\lambda_i$ modulo the bounded ideal.