---
layout: post
title: Law of Total Expectation
#date: 2022-01-01 00:00:00-0000
#description: Expectations from your expectations.
---
---
#### Statement

Consider a random variable $$ X $$ with expectation denoted as $$ \mathbb{E}[X]$$ and let $$ Y $$ be another random variable in the same probability space. Then, the law of total expectation states that
\begin{equation} \nonumber
\mathbb{E}[X] = \mathbb{E}[\mathbb{E}[X|Y]]
\end{equation}

##### Proof: Continuous case
Consider the expectation in the left hand side of the above equation
\begin{equation} \nonumber
\mathbb{E}[X] = \int x p(x)dx
\end{equation}
where $$p(x)$$ is the probability density function (pdf) of random variable $$X$$. The pdf $$p(x)$$ satisfies
\begin{equation} \nonumber
p(x) = \int p(x,y)dy
\end{equation}
Therefore,

$$
\begin{align}
\mathbb{E}[X] &= \int x p(x)dx \nonumber \\
&= \int x \left[\int p(x, y) dy\right]dx \nonumber \\
&= \int x \left[\int p(x|y)p(y)dy\right]dx \nonumber\\
&= \int \left[\int x p(x|y)dx\right]p(y)dy \nonumber \quad (*) \\
&= \int \mathbb{E}[X|Y]dy \nonumber \\
&= \mathbb{E}[\mathbb{E}[X|Y]] \nonumber
\end{align}
$$

(*) The exchange of integrals is a consequence of [Fubini's theorem](https://web.ma.utexas.edu/users/m408m/Display15-2-3.shtml). Hence the law of total expectations cannot be applied in cases that do not satisfy the conditions of the Fubini's theorem.
