---
title: A market for consumer information
---

In this post I will make the case that giving consumers, so-called property
rights over their personal data is not in their best interest.  That is,
consumers will be worse off in the presence of some kind of technology that
allows them to sell or seek compensation for their personal information in a
market. The argument will make use of the notion of “equilibrium” which is a
term economists use to address the situation where a lot of people are making a
decision at the same time.  So while the individual consumer might benefit from
having rights to their own data, when *all* consumers are given this right,
*all* consumers will be worse off, or at least that will be the argument.

### The game

Consider a market for a good and, to simulate a large number of people, let each
consumers's personal valuation for the good be distributed on the continuum
$[0,1]$ such that the total number of people have a *mass* of $1$. To be more
precise, the valuation, $v$, of every consumer is distributed according to the
CDF $F$. The market is served by monopolist who aims to maximize it's profit in
the market. In the standard case the monopolist knows $F$ and thus sets the
price, $p$, that solves

$$ p^M = \frac{f(p)}{1-F(p)} $$.

Suppose instead that, before trade, every consumer has the option to sell its
personal valuation to the monopolist. That is, the consumer either sells
information or does not. The information is verifiable, meaning the consumer
has no option to lie or to only partially reveal their information. The
monopolist can then use the information during trade to offer personalized
prices to consumers. The timing is as follows

1. The monopolist offers a uniform (across consumers) price, $r \geq 0$, for
consumer information 
2. Every consumer decides whether or not to sell 
3. The monopolist uses the information to offer personalized prices $p(v)$ to
consumers who sell information and offers a uniform price $p$ to all consumers
who choose not to sell.

The equilibrium concept used in this kind of game is *Perfect Bayesian
Equilibrium* (PBE). Since the decision of each consumer to sell or not may be
informative about their valuation, in equilibrium, the monopolist has to form a
belief about what kind of consumer is choosing not to sell information. In turn,
the belief has to match the actual distribution of consumers, which shows the
nature of an equilibrium as a kind of stability condition.

### The solution

The unique solution to the game, that is, the unique PBE, is for the monopolist
to offer $r=0$ and for *all* consumers to sell their information. The monopolist
sets $p(v)=v$ and $p=1$. Clearly the equilibrium is very bad for consumers, as
they are both (a) perfectly price discriminated against and (b) not
compensated for the data they sell. So how can this be?

First notice that the *marginal consumer*, with valuation $\hat{v}$, who is
indifferent between selling and not selling, satisfies

$$ r = \hat{v} - p $$.

Here the LHS is the surplus from selling and the RHS is the surplus from not
selling and facing $p$ in the product market (remaining anonymous). Clearly,
given $r$ and $p$, for any consumer with $v \leq \hat{v}$ it is optimal to sell.
The valuation of the marginal consumer, $\hat{v}$, then acts as a cut-off where
all consumers with a higher valuation do not sell and remain anonymous. Thus,
given a cut-off, $\hat{v}$, the monopolist sets an optimal price, $p \geq
\hat{v}$. So, suppose that the monopolist sets $r > 0$ in the first stage. Then
the marginal consumer gets no payoff from not selling but a strictly positive
payoff from selling.  This precludes the existence of a marginal consumer.

On the other hand, it is clear that the above proposed equilibrium is in fact an
equilibrium where no one has an incentive to deviate. If every consumer sells
data, the monopolist can form any belief it wants about a consumer who does not
sell data, since on the equilibrium path, this is a probability zero event. Thus
choosing the belief $v=1$ with probability $1$ for a non-selling consumer, the
optimal price is $p=1$. In this case, any consumer who deviates to not selling
gets a payoff of zero, which makes the deviation non-profitable.

Finally, one might wonder if there is an equilibrium where no consumer sells
data and the monopolist sets the monopolist price $p^M$ and
$r=0$. But this is not an equilibrium since it is not stable. The monopolist can
profitably deviate to raising the price, $r$, and having the lower segment, who
do not trade at price $p^M$, sell their data. The proposed
equilibrium is thus unique.
