---
title: Chapter 3 - Population
banner: ../figures/Ch03_Population/_page_49_Picture_0.jpeg
numbering:
  headings:
  heading_1:
    start: 4
kernelspec:
  name: python3
  display_name: 'Python 3'
---

(chap:population)=
# Population

Underlying virtually every concern relating to our experience on this planet is the story of human population. The discussion of continued energy growth in [Chapter 1](chap:expgrowth) was based on the historical growth rate of energy, which is partly due to growing population and partly due to increased use per capita. But the notion that population will continue an exponential climb, as is implicit in the [Chapter 1](chap:expgrowth) scenario, is impractical one of many factors that will render the "predictions" of [Chapter 1](#chap:expgrowth) invalid and prohibit "growth forever."

So let's add a dose of reality and examine a more practical scenario. Americans' per-capita use of energy is roughly *five times* the global average rate. If global population eventually doubles, and the average global citizen advances to use energy at the rate Americans currently do,[^1] then the total scale of energy use would go up by a factor of 10, which would take 100 years at our mathematically convenient 2.3% annual rate (see Eq. {eq}`eq:expgrowth:logM`. This puts a more realistic—and proximate-timescale on the end of energy growth than the fantastical extrapolations of [Chapter 1](chap:expgrowth). Although the focus of this chapter will be on the alarming rate of population growth, we should keep the energy and resource context in mind in light of the overall theme of this book. To this end, [](fig:population:popenergy) shows the degree to which energy demand has outpaced population growth, when scaled vertically to overlap in the nineteenth century. From 1900 to 1950, per-capita energy consumption increased modestly, but then ballooned dramatically after 1950, so that today we have the equivalent of 25 billion people on the planet operating at nineteenth century energy levels.

Since population plays a giant role in our future trajectory, we need to better understand its past. We can also gain some sense for theoretical expectations, then discuss the heralded "demographic transition" and its implications.

[^1]: ... so that global average energy use per capita increases by a factor of five from where it is today.
```{figure} ../figures/Ch03_Population/powerpop.svg
:label: fig:population:popenergy
:width: 95%
:align: center
:alt: Population (red) and energy demand (blue) on the same plot, showing how much faster energy demand (power) has risen compared to population, which translates to increasing per-capita usage. The vertical axes are scaled so that the curves overlap in the nineteenth century. ([](doi:10.1111/j.1466-8238.2010.00587.x); @wiki_worldpop; @ourworldindata)
Population (red) and energy demand (blue) on the same plot, showing how much faster energy demand (power) has risen compared to population, which translates to increasing per-capita usage. The vertical axes are scaled so that the curves overlap in the nineteenth century. ([](doi:10.1111/j.1466-8238.2010.00587.x); @wiki_worldpop; @ourworldindata)
```

# Population History

[](fig:population:popestimatelin) shows a history of global population for the last 12,000 years. Notice that for most of this time, the level is so far down as to be essentially invisible. It is natural to be alarmed by the sharp rise in recent times, which makes the current era seem wholly unusual: an aberration. But wait—maybe it's just a plain exponential function. All exponential functions—ruthless as they are—would show this alarming rise at some point, sometimes called a {term}`hockey stick` plot. In order to peer deeper, we plot population on a logarithmic vertical axis in [](#fig:population:popestimatelog). Now we bring the past into view, and can see whether a single exponential function (which would have a constant slope in a logarithmic plot) captures the story. Notice an exponential function when plotted logarithmically on the vertical axis looks like
$$\ln(y) &= \ln\left(Ae^{mx}\right)\\
\\
\ln(y) &= \ln(A) + \ln\left(e^{mx}\right)\\
\\
\ln(y) &= b + mx\\
$$
where in the second step, we used the rule that $\ln(a\cdot b)=\ln(a) +\ln(b)$, and in the third line we used the idea that the natural log "undoes" the exponential function. The last line also rewrites $\ln(A) = b$ since the natural log of the number $A$ is just some other number $b$. The last line looks like the equation of a line on the right hand side.

Wait, what? [](#fig:population:popestimatelog) still looks somewhat like a hockey stick (even more literally so)! How can that be?! This can't be good news. Peering more closely, we can crudely break the history into three eras, each following {term}`exponential growth` (straight lines on the plot), but at different rates. The early phase had a modest 0.004% growth rate. By the rule of 70, the corresponding doubling time is about 17000 years. From about -4000 years ago to 1700, the rate is about 0.075%, corresponding to a doubling time of approximately 1000 years. In more recent times, a 0.8% rate is more characteristic (90 year doubling). Indeed, we would be justified in saying that recent centuries are anomalous compared to the first 10,000 years of the plot. If we extend the the 0.075% line and the 0.8% line, we find that they intersect around the year 1700, which helps identify the era of marked transition.

The recent rapid rise is a fascinating development, and begs for a closer look. [](fig:population:popestimatefourera) shows the last ~1,000 years, for which we see several exponential-looking segments at ever-increasing rates. The doubling times associated with the four rates shown on the plot are presented in [](#table:population:popestimatefourera)

An interpretation of the population history might go as follows. Early humans did not proliferate quickly. Around 6000 years ago was the an increase in agriculture and a move away from hunter-gatherer societies. Not much changed during the period following the Dark Ages.[^2] The Renaissance (~1700) introduced scientific thinking so that we began to conquer diseases, allowing an uptick in population growth. In the mid-19th century (~1870), the explosive expansion of [fossil fuel](#chap:fossilfuels) usage permitted industrialization at a large scale, and mechanized farming practices. More people could be fed and supported, while our mastery over human health continued to improve. In the mid-20th century (~1950), the {term}`Green Revolution` [@greenrevolution] introduced a fossil-fuel-heavy diet of fertilizer and largescale mechanization of agriculture, turning food production into an industry. The combination of a qualitative change in the availability of cheap nutrition and the march of progress on disease control cranked the population rate even higher.

```{figure} ../figures/Ch03_Population/poplinear.svg
:label: fig:population:popestimatelin
:width: 100%
:align: center
:alt: Global population estimate, over the modern human era, on a linear scale. [](#fig:population:popenergy) offers a recent close-up. [[](doi:10.1111/j.1466-8238.2010.00587.x); @wiki_worldpop].
Global population estimate, over the modern human era, on a linear scale. [](#fig:population:popenergy) offers a recent close-up. [[](doi:10.1111/j.1466-8238.2010.00587.x); @wiki_worldpop].
```
```{figure} ../figures/Ch03_Population/poplog3era.svg
:label: fig:population:popestimatelog
:width: 100%
:align: center
:alt: Global population estimate, over the modern human era, on a logarithmic scale. [[](doi:10.1111/j.1466-8238.2010.00587.x); @wiki_worldpop]
Global population estimate, over the modern human era, on a logarithmic scale. [[](doi:10.1111/j.1466-8238.2010.00587.x); @wiki_worldpop]
```
```{figure} ../figures/Ch03_Population/poplog4era.svg
:label: fig:population:popestimatefourera
:width: 100%
:align: center
:alt: Global population estimate, over recent centuries. On the logarithmic plot, lines of constant slope are exponential in behavior. Four such exponential segments can be broken out in the plot, having increasing growth rates. [[](doi:10.1111/j.1466-8238.2010.00587.x); @wiki_worldpop]
Global population estimate, over recent centuries. On the logarithmic plot, lines of constant slope are exponential in behavior. Four such exponential segments can be broken out in the plot, having increasing growth rates. [[](doi:10.1111/j.1466-8238.2010.00587.x); @wiki_worldpop]
```

[^2]: ... except that famine and plague took a toll in the 14th century.

```{table} Doubling times for [](#fig:population:popestimatefourera)
:label: table:population:popestimatefourera
:align: center
| Years      | % growth | t<sub>2</sub> (yr)|
|:----------:|----------:|---:|
| 1000–1700  | 0.08%    | 875 |
| 1700–1870  | 0.48%    | 145 |
| 1870–1950  | 0.80%    | 87.5|
| 1950–2020  | 1.70%    | 40  |
```

In more recent years, the rate has fallen somewhat from the 1.7% fit of the last segment in [](#fig:population:popestimatefourera), to around 1.1%. Rounding down for convenience, continuation at a 1% rate would increase population from 7 billion to 8 billion people in less than 14 years. The math is the same as in [Chapter 1](#chap:expgrowth), re-expressed here as
$$
\label{eq:population:popvst}
P = P_{0}e^{\ln(1+p)(t-t_{0})},
$$


where $P_0$ is the population at time $t_0$, and $P$ is the population at time $t$ if the growth rate is steady at $p$. Inverting this equation,[^3] we have
[^3]: ... recalling that that the natural log and exponential functions "undo" each other as inverse functions.

$$
\label{eq:population:inverted_t}
t - t_{0} = \frac{\ln\left(\frac{p}{p_{0}}\right)}{\ln(1+p)}.
$$


```{tip} Example 
We can use Eq. {eq}`eq:population:popvst` to determine how many people we will have in the year 2100 if we continue growing at a 1% rate, starting from 7 billion in the year 2010. We set  $P_0 = 7$  Gppl[^4], $t_0 = 2010, p = 0.01$, then compute the population in 2100 to be  $P = 7e^{\ln 1.01 \cdot 90} = 17$  Gppl.
Eq. {eq}`eq:population:inverted_t` is the form that was used to conclude that increasing from 7 to 8 Gppl takes less than 14 years at a 1% rate. The computation looks like:  $\ln(8/7)/\ln(1.01) = 13.4$ . Note that we need not include the factors of a billion in the numerator and denominator, since they cancel in the ratio. The actual time for adding one billion people has lately been 12 years, as we have been growing at a rate slightly higher than 1%.
```
```{table} Population milestones: dates at which we added another one billion living people to the planet. The Time and Doubling columns are expressed in years. Around 1965, the growth rate got up to 2%, for a 35 year doubling time.
:label: table:population:popmilestones
:align: center
| Year | Population (Gppl) | Time | Rate | Doubling |
|:------:|:---------------:|-----:|:----:|----------:|
| 1804 | 1                 | —    | 0.4% | 170      |
| 1927 | 2                 | 123  | 0.8% | 85       |
| 1960 | 3                 | 33   | 1.9% | 37       |
| 1974 | 4                 | 14   | 1.9% | 37       |
| 1987 | 5                 | 13   | 1.8% | 39       |
| 1999 | 6                 | 12   | 1.3% | 54       |
| 2011 | 7                 | 12   | 1.2% | 59       |
| 2023 | 8                 | 12   | 1.1% | 66       |
```
[^4]: Gppl is giga-people, or billion people

[](#table:population:popmilestones) and [](fig:population:popestimatefourera) illustrate how long it has taken to add each billion people, extrapolating to the 8 billion mark (as of writing in 2020). The first billion people obviously took tens of thousands of years, each new billion people taking less time ever since. Growth rate peaked in the 1960s at 2% and a doubling time of 35 years. The exponential rate is moderating now, but even 1% growth continues to add a billion people every 13 years, at this stage. A famous book by Paul Ehrlich called The Population Bomb [@populationbomb], first published in 1968, expressed understandable alarm at the 2% rate that had only *increased* to that point. The moderation to 1% since that period is reassuring, but we are not at all out of the woods yet. The next section addresses natural mechanisms for curbing growth. 
```{figure} ../figures/Ch03_Population/popbillionincrease.svg
:label: fig:population:doublings
:width: 100%
:align: center
:alt: Graphical representation of [](#tabel:population:popmilestones) showing the time between each billion people added.
Graphical representation of [](#tabel:population:popmilestones) showing the time between each billion people added.
```

# Logistic Model

Absent human influence, the population of a particular animal species on the planet might fluctuate on short timescales (year by year) and experience large changes on very long timescales (centuries or longer). But by-and-large nature finds a rough equilibrium. Overpopulation proves to be temporary, as exhaustion of food resources, increased predation, and in some cases disease (another form of predation, really) knock back the population.[^5] On the other hand, a small population finds it easy to expand into abundant food opportunities, and predators reliant on the species have also scaled back due to lack of prey. We have just described a form of *negative feedback*, corrective action to remedy a maladjusted system back toward equilibrium.
[^5]: For reference, the SARS-CoV2 pandemic of 2020 barely impacted global population growth rates. When population grows by more than 80 million each year, a disease killing even a few million people barely registers as a hit to the broader trend.

```{note} Definition: Negative feedback
Means that a correction is applied in a direction opposite the recent motion. If a pendulum moves to the right, a restoring force pushes it back to the left, while moving too far to the left results in a rightward push. A mass oscillating on a spring demonstrates similar characteristics, as must all equilibrium phenomena. 

The word *negative* may sound like something thing we would not want, but its cousin {term}`positive feedback` leads to disastrous runaway conditions. An example of positive feedback is the bacteria example from [Chapter 1](#chap:expgrowth) having more bacteria only increases the rate of growth. Exponentials are the hallmark of positive feedback, while equilibrium signals negative feedback.
```
 We can make a simple model for how a population might evolve in an environment hosting negative feedback. When a population is small and resources are abundant, the birth rate is proportional to the population.
```{tip} Example
:label: ex:population:fawns
If a forest has 100 breeding-aged deer, or 50 couples, we can expect 50 fawns in a year (under the simplifying and unimportant assumption of one fawn per female per year). If the forest has 200 deer, we can expect 100 fawns. The birth rate is simply *proportional* to the population capable of giving birth.[^6] 
```
[^6]: 6: ... no negative feedback yet

If the setup in the [Example](#ex:population:fawns) were the only element to the story, we would find exponential growth: more offspring means a larger population, which ultimately reaches breeding age to produce an even larger population.[^7] But as the population grows, negative feedback will begin to play a role. We will denote the population as  $P$ , and its rate of change as  $\dot{P}$.[^8]  We might say that the growth rate, or  $\dot{P}$, is

[^7]: We have just described a state of {term}`positive feedback`: more begets more.
[^8]:  $\dot{P}$  is a time derivative, i.e., the change in population over time (indicated by the dot on top), defined as  $\dot{P} = \Delta P/\Delta t$ . But don't panic if calculus is not your thing: what we describe here is still totally understandable.

$$
\label{eq:population:dotP}
\dot{P} = rP,
$$

where $r$ represents the birth rate in proportion to the population (e.g., 0.04 if 4% of the population will give birth in a year).[^9] This equation just re-iterates the simple idea that the rate of population growth is dependent on (proportional to) the *present* population. The solution to this {term}`differential equation` is an exponential:

$$
\label{eq:population:expP}
P = P_{0}e^{r(t - t_{0})},
$$
which is really just a repeat of Eq. {eq}`eq:population:popvst` where  $r$  takes the place of  $\ln(1 + p)$.

[^9]: In terms of the growth rate we used before,  $p$ , as in Eq. {eq}`eq:population:popvst`  $r = \ln(1 + p)$ . So for instance, if growing at 2%,  $p = 0.02$  and  $r$  also is 0.02 ( $r \approx p$  for small values of  $p$ ).

```{tip} Example
:label: ex:population:fawns2
Paralleling the deer population scenario from the [Example](#ex:population:fawns), if we set  $r = 0.5$ , and have a population of  $P = 100$  adult deer (half female), Eq. {eq}`eq:population:dotP` says that  $\dot{P} = 50$ , meaning the population will change by 50 units.[^10] We could then use Eq. {eq}`eq:population:expP` to determine the population after 4 years:  $P = 100e^{0.5 \cdot 4} \approx 739$.
```
[^10]: A more adorable term for "units" is fawns, in this case. We ignore death rate here, but it effectively reduces  $r$  in ways that we will encounter later.
Let's say that a given forest can support an ultimate number of deer, labeled  $Q$ , in steady state, while the current population is labeled  $P$ . The difference,  $Q - P$  is the "room" available for growth, which we might think of as being tied to available resources. Once  $P = Q$ , no more resources are available to support growth.

```{note} Definition: Carrying Capacity
Often used to describe $Q$: the population supportable by the environment. The carrying capacity ($Q$) for human population on Earth is not an agreed-upon number, and in any case it is a strong function of lifestyle choices and resource dependence.
```
$Q-P$  quantifies a growth-limiting mechanism by representing available room. One way to incorporate this feature into our growth rate equation is to make the rate of growth look like
$$
\label{eq:population:Pdot2}
\dot{P} = \frac{Q - P}{Q} rP.
$$

We have multiplied the original rate of  $rP$  by a term that changes the effective growth rate  $r \rightarrow r(Q - P)/Q$ . When  $P$  is small relative to  $Q$ , the effective rate is essentially the original  $r$ . But the effective growth rate approaches zero as  $P$  approaches  $Q$ . In other words, growth slows down and hits zero when the population reaches its final saturation point, as  $P \rightarrow Q$  (see [](#fig:population:growthrate)).
```{figure} ../figures/Ch03_Population/growthvsPt.svg
:label: fig:population:growthrate
:width: 100%
:align: center
:alt: The rate of growth in the logistic model decreases as population increases, starting out at *r* when  $P = 0$  and reaching zero as  $P \rightarrow Q$  (see Eq.{eq}`eq:population:Pdot2`
The rate of growth in the logistic model decreases as population increases, starting out at *r* when  $P = 0$  and reaching zero as  $P \rightarrow Q$  (see Eq.{eq}`eq:population:Pdot2`
``` 

The mathematical solution to this modified differential equation (whose solution technique is beyond the scope of this course) is called a {term}`logistic curve`, plotted in [](#fig:population:logistic) and having the form
$$
\label{eq:population:logistic}
P(t) = \frac{Q}{1 + e^{-r(t - t_0)}}.
$$

```{exercise} Growth Rate vs. Population
:label: ex:population:growthrate
Pick a value for  $Q$  (10 billion, maybe) and then various values of $P$ that are less than or equal to $Q$ to see how the effective growth rate will be modified. Make a graph like [](#fig:population:growthrate).
```
```{solution} ex:population:growthrate
:label: ex:population:growthratesoln
:class: dropdown
I'm going to set the carrying capacity to $Q=10$ (billion people) and the initial population to $P=2.5$ (billion people), corresponding to 1950. One can set $r$, but it is not necessary because we are interested in how $r$ changes. Since $r\rightarrow r(Q-P)/Q$, $r$ will change according to $(Q-P)/Q$. At any particular point in time, $P$ is a constant value, but the x-axis of [](#fig:population:growthrate) shows changing population values. Therefore, we first need to know how $P$ changes in time for a constant growth rate. To determine this, we must solve Eq. {eq}`eq:population:logistic`. I used Microsoft Excel to do calculations and make a graph. Here are the steps I used.
1. Enter years beginning at $t_0=1950$ and increment by 1 year up to the year $t=2000$.
2. Notice in [](#fig:population:doublings) that the population in 1950 is approximately 2.5 billion.
3. From [](#table:population:popestimatefourera), the rate from 1950 to 2000 is on average about $r=1.7\%=0.017$.
4. Calculate the logistic equation {eq}`eq:population:logistic`. In cell B2, I enter `=2.5*exp(0.017*(A2-1950))'.
5. Highlight the cells B2 to B52. Type `fill down` in the search bar, and Excel will copy the forumula for the rest of the cells.
6. For fun, I made a graph of population over time.
![Excel spreadsheet for population vs. time calculations and graph.](../figures/Ch03_Population/PvtExcel.png)
7. The population values are now going to be the x-axis for the rate, $r$.
8. In cell C2, I calculate $r(Q - P)/Q$ by entering `=0.017*(10-B2)/10`.
9. Use the fill down trick from step 5.
10. Make a graph and label it.
![Excel spreadsheet for growth rate vs. population calculations and graph.](../figures/Ch03_Population/rvtExcel.png)
```

The first part of the curve in [](#fig:population:logistic) for very negative values[^11] of  $t - t_0$ , is exponential but still small. At  $t = t_0$  (time of inflection), the population is  $Q/2$ . As time marches forward into positive territory,  $P$  approaches  $Q$ . As it does so, negative feedback mechanisms (limits to resource/food availability, predation, disease) become more assertive and suppress the rate of growth until it stops growing altogether when $P$ reaches $Q$.

[^11]: The parameter  $t_0$  is the time when the logistic curve hits its halfway point. Times before this have negative values of  $t - t_0$ .

```{figure} ../figures/Ch03_Population/_page_54_Figure_1.jpeg
:label: fig:population:logistic
:width: 100%
:align: center
:alt: Logistic population curve (blue), sometimes called an S-curve, as given in Eq. {eq}`eq:population:logistic`, in this case plotting for  $r = 0.5$  to match examples in the text. The red curve is the exponential that would result without any negative feedback.
Logistic population curve (blue), sometimes called an S-curve, as given in Eq. {eq}`eq:population:logistic`, in this case plotting for  $r = 0.5$  to match examples in the text. The red curve is the exponential that would result without any negative feedback.
```
```{note} Example
:label: ex:population:fawns3
Continuing the deer scenario, let's say the forest can ultimately support 840 adults,[^12] and keep  $r = 0.5$  as the uninhibited growth rate. Using these numbers, Eq. {eq}`eq:population:logistic` yields 100 adults at  $t = t_0-4$  years (effectively the initial state in [](#:label: ex:population:fawns). One year later, at  $t = t_0 - 3$ , Eq. {eq}`eq:population:logistic` yields 153—very close to the nominal addition of 50 members. But now four years in ($t = t_0$), we have 420 instead of the 739 we got under unrestricted exponential growth in [Example](#:label: ex:population:fawns2).[^13]
```

The logistic curve is the *dream scenario*: no drama. The population simply approaches its ultimate value smoothly, in a tidy manner. We might imagine or hope that human population follows a similar path. Maybe the fact that we've hit a linear phase—consistently adding one billion people every 12 years, lately—is a sign that we are at the inflection, and will start rolling over toward a stable endpoint. If so, we know from the logistic curve that the linear part is halfway to the final population.

Three consecutive 12-year intervals appear in [](#table:population:popmilestones). If the middle one is the midpoint of a logistic linear phase — in 2011 at 7 billion people — it would suggest an ultimate population of 14 billion.

## Overshoot

But not so fast. We left out a crucial piece: feedback delay. The math that leads to the logistic curve assumes that the negative feedback[^14]  acts instantaneously in determining population rates.

Consider that human decisions to procreate are based on present conditions: food, opportunities, stability, etc. But humans live for many decades, and do not impose their full toll on the system until many years after birth, effectively delaying the negative feedback. The logistic curve and equation that guided it had no delay built in.

[^12]: tuned for a convenient match to the numbers we have used in the foregoing examples.
[^13]: Not coincidentally,  $P = Q/2$  at the halfway point, $t = t_0$.
[^14]: ... based on remaining resources, $Q-P$, at the moment in Eq. {eq}`eq:population:dotP`.

```{note} Definition: Overshoot 
A generic consequence of delaying negative feedback. Since negative feedback is a “corrective,” stabilizing influence, delaying its application allows the system to “get away” from the control, thereby exceeding the target equilibrium state.

By "generic consequence," we just mean an outcome that is characteristic of the situation, independent of details.
```

This is a pretty easy concept to understand. The logistic curve of [](#fig:population:logistic) first accelerates, then briefly coasts before decelerating to arrive smoothly at a target. Following an example from [@meadows2004limits], *The Limits to* , it is much like a car starting from rest by accelerating before applying the brakes to gently come to a stop when the bumper barely kisses a brick wall. The driver is operating a negative feedback loop: seeing/sensing the proximity to the wall and slowing down accordingly. The closer to the wall, the slower the driver goes until lightly touching the wall. Now imagine delaying the feedback to the driver by applying a blindfold and giving voice descriptions of the proximity to the wall, so that decisions about how much to brake are based on conditions from a delayed communication process. Obviously, the driver will crash into the wall if the feedback is delayed, unless slowing down the whole process dramatically. Likewise, if the negative consequences—signals that we need to slow down population growth—arrive decades after the act of producing more humans, we can expect to exceed the "natural" limit,  $Q$ — a condition called *overshoot*.

Another example of feedback delay leading to overshoot: let's say you are holding down the space bar and trying to position the cursor in the middle of the screen. But your connection is lagging and even though you release the space bar when you *see*the cursor reach the middle, it keeps sailing past due to the delay: overshooting.

```{tip} Example
We did not detail the mechanisms of negative feedback operating on the deer population in [Example](#ex:population:fawns3) that act to stabilize the population at 푄, but to illustrate how delayed negative feedback produces overshoot, consider predation as one of the operating forces. To put some simple numbers on it, let's say that steady state can support one adult (hunting) mountain lion for every 50 deer. Initially, when the population was 100 deer, this means two predators. When the deer population reaches $Q= 840$, we might have $\sim 17$ predators. But it takes time for the predators to react to the growing number of prey, perhaps taking a few years to produce the requisite number of hunting adults. Lacking the full complement of predators, the deer population will sail past the 840 mark until the predator population rises to establish the ultimate balance. In fact, the predators will likely also exceed their steady population in a game of catch-up that leads to oscillations like those seen in [](#fig:population:feedback)
```

We can explore what happens to our logistic curve if the negative feedback is delayed by various amounts. [](#fig:population:feedback) gives a few examples of overshoot as the delay increases. To avoid significant overshoot, the delay ($\tau$) needs to be smaller than the natural timescale governing the problem: $1/r$, where $r$ is the rate in Eqs. {eq}`eq:population:dotP` and {eq}`eq:population:logistic` In our deer example using $r=0.5$, any delay longer than about 2 years causes overshoot. For more modest growth rates (human populations), relevant delays are in decades (see [Box](#box:population:overshoot).

```{figure} ../figures/Ch03_Population/_page_56_Figure_1.jpeg
:label: fig:population:feedback
:width: 100%
:align: center
:alt: Feedback delay generally results in overshoot and oscillation, shown for various delay values, $\tau$. The black curve ($\tau = 0$) is the nominal no-delay logistic curve. As the delay increases, the severity of overshoot increases. Delays are explored in increments of 0.5 times the characteristic timescale of $1/r$ (using $r=0.5$ here to match previous examples, so that a delay of $\tau = 1.5/r$ equates to 3 time units on the graph, for instance). The delay durations are also indicated by bar lengths in the legend.
Feedback delay generally results in overshoot and oscillation, shown for various delay values, $\tau$. The black curve ($\tau = 0$) is the nominal no-delay logistic curve. As the delay increases, the severity of overshoot increases. Delays are explored in increments of 0.5 times the characteristic timescale of $1/r$ (using $r=0.5$ here to match previous examples, so that a delay of $\tau = 1.5/r$ equates to 3 time units on the graph, for instance). The delay durations are also indicated by bar lengths in the legend.
```

Eventually all the curves in [](#fig:population:feedback) converge to the steady state value of 1.0,[^15] but human population involves complexities not captured in this bare-bones mathematical model.[^16] All the same, the generic phenomenon of overshooting when negative feedback is delayed is a robust attribute, even if the oscillation and eventual settling does not capture the future of human population well.

```{figure} ../figures/Ch03_Population/_page_56_Figure_3.jpeg
:label: fig:population:popalonglogistic
:width: 100%
:align: center
:alt: Human population data points (blue) and a logistic curve (red) that represents the best fit to data points from 1950 onward. The resulting logistic function has  $Q \approx 12$  Gppl,  $r = 0.028$ , and a midpoint at the year 1997. The actual data sequence has a sudden bend at 1950 (could this be the Green Revolution?) that prevents a suitable fit to a larger span of data. In other words, the actual data do not follow a single logistic function very well, which is to be expected when conditions change suddenly (energy and technology, in this case) [[](doi:10.1111/j.1466-8238.2010.00587.x); @wiki_worldpop].
Human population data points (blue) and a logistic curve (red) that represents the best fit to data points from 1950 onward. The resulting logistic function has  $Q \approx 12$  Gppl,  $r = 0.028$ , and a midpoint at the year 1997. The actual data sequence has a sudden bend at 1950 (could this be the Green Revolution?) that prevents a suitable fit to a larger span of data. In other words, the actual data do not follow a single logistic function very well, which is to be expected when conditions change suddenly (energy and technology, in this case) [[](doi:10.1111/j.1466-8238.2010.00587.x); @wiki_worldpop].
```

```{hint} Will Human Population Overshoot?
:label: box:population:overshoot
Are humans in danger of population overshoot? What is our $r$ value? It is tempting to take $r=0.01$ corresponding to the present 1% growth rate. This would imply that any delay shorter than 100 years will not produce significant overshoot, which seems reassuring. But if human population is following a logistic curve rather than an exponential, resource availability is already exerting a moderating influence, now appearing to be in the linear "cruise" phase roughly halfway to the limiting value. A fit to the data [](#fig:population:popalonglogistic) suggests that  $r \approx 0.028$ , corresponding to a timescale of 36 years  $(1/r)$ . This puts the overshoot-prone delay squarely into relevant timescales for human lifetimes, generations, and societal change—thus leaving the door open for an overshoot scenario.
```

[^15]: ... meaning that population $P$ arrives at $Q$.
[^16]: For instance, a dramatic overshoot and collapse could be disruptive enough to take out our current infrastructure for fossil-fuelaided agriculture so that the $Q$ value essentially resets to some lower value.

## Logistic Projection

As suggested by [](#fig:population:popalonglogistic) Human population is *not* following a strict logistic curve. If it were, the early period would look exponential at the ~2.8% rate corresponding to the best-fit logistic matching our recent trajectory, but growth was substantially slower than 2.8% in the past. Technology and fossil fuels have boosted our recent growth well beyond the sub-percent rates typical before ∼1950. The point is that while reference to mathematical models can be extremely helpful in framing our thinking and exposing *robust, generic modes* of interest, *we should seldom take any mathematical model literally*, as it likely does not capture the full complexity of the system it is trying to model. In the present case, it is enough to note that:
1. exponentials relentlessly drive toward infinity (ultimately unrealistic);
2. logistic curves add a sensible layer of reality, capping growth in some steady-state outcome;
3. other dynamical factors such as delays can prevent a smooth logistic function, possibly leading to overshoot; and
4. many other factors (medical and technological breakthroughs, war, famine, climate change) can muddy the waters in ways that could make the situation better or worse than simple projections.

# Demographic Transition

Perhaps not surprisingly, the rate of a country's population growth is correlated to its wealth, as seen in [](#fig:population:popgrowthvGDP) An attractive path to reducing population growth would be to have poor countries slide down this curve to the right: becoming more affluent and transforming societal values and pressures accordingly to produce a lower net population growth rate.

Population growth happens when the birth rate exceeds the death rate.

```{note} Definition: Birth rate
Typically expressed in births per 1000 people per year, minus {term}`death rate` (also in deaths per 1000 people per year) is the net population rate[^17]. If the difference is positive, the population grows, and it shrinks if the difference is negative.
``` 
[^17]: This ignores immigration, which just shifts living persons around.shifts living persons around.

```{figure} ../figures/Ch03_Population/_page_58_Figure_1.jpeg
:label: fig:population:popgrowthvGDP
:width: 100%
:align: center
:alt: Net population rate, in percent, as a function of per-capita GDP. A clear trend shows wealthier countries having lower growth rates. A win–win solution would seem to present itself, in which everyone arrives at the lower right-hand side of this graph: more money for all and a stable population! Dot size (area) is proportional to population [@wikiGDP; @wikipopulation; @wikibirthrate; @wikideathrate].
Net population rate, in percent, as a function of per-capita [GDP.](#page-448-2) A clear trend shows wealthier countries having lower growth rates. A win–win solution would seem to present itself, in which everyone arrives at the lower right-hand side of this graph: more money for all and a stable population! Dot size (area) is proportional to population [@wikiGDP; @wikipopulation; @wikibirthrate; @wikideathrate].
```

```{tip} Example
:label: ex:population:USbirthrate
The U.S. has a birth rate of about 12 people per 1000 per year, and a death rate of 8.1 people per 1000 per year. The net rate is then roughly +4 per 1000 per year, translating to 0.4% net growth.[^18] 

Niger has a birth rate of 46 per 1000 per year and a death rate of 11, resulting in a net of positive 35, or 3.5%.
```

As conditions change, birth and death rates need not change in lock-step. Developed countries tend to have low birth rates *and* low death rates, balancing to a relatively low net population growth rate. Developing countries tend to have high death rates and even higher birth rates, leading to large net growth rates. [](#fig:population:birthtodeathrates) depicts both birth rates and death rates for the countries of the world. A few countries (mostly in Europe) have slipped below the replacement line, indicating declining population.[^19] 

The general sense is that developed countries have "made it" to a responsible low-growth condition, and that population growth is driven by poorer countries. An attractive solution to many[^20] is to bring developing countries up to developed-country standards so that they, too, can settle into a low growth rate. This evolution from a fast-growing poor country to a slow (or zero) growth well-off country is called the {term}`demographic transition`.

```{note} Definition: The demographic transition
Refers to the process by which developing countries having high death rates and high birth rates adopt technologies, education, and higher standards of living that result in low death rates and low birth rates, more like advanced countries.
```

[^18]: 4 per 1000 is 0.4 per 100, which is another way to say 0.4 percent.
[^19]: Note that immigration is not considered here: just birth rate and death rate within the country.
[^20]: . . . but unsolicited "preaching" to others.

In order to accomplish this goal, reduced death rates are facilitated by introducing modern medicine and health services to the population. Reduced birth rates are partly in response to reduced infant mortality eventually leading to fewer children as survival is more guaranteed. But also important is better education—especially among women in the society who are more likely to have jobs and be empowered to exercise control of their reproduction (e.g., more say in relationships and/or use of contraception). All of these developments take time and substantial financial investment.[^21] Also, the economy in general  must be able to support a larger and better-educated workforce. The demographic transition is envisioned as a transformation or complete overhaul, resulting in a country more in the mold of a "first-world" country.[^22]

[^21]: Better hospitals and schools are not free.
[^22]: One may justifiably question whether this is the "correct" goal.

```{figure} ../figures/Ch03_Population/_page_59_Figure_1.jpeg
:label: fig:population:birthtodeathrates
:width: 100%
:align: center
:alt: Birth rates and death rates for countries, where dot size is proportional to population. The diagonal line indicates parity between birth and death rates, resulting in no population growth. Countries above the line are growing population, while countries below are shrinking. A few countries fall a bit below this line [@wikipopulation; @wikibirthrate; @wikideathrate].
Birth rates and death rates for countries, where dot size is proportional to population. The diagonal line indicates parity between birth and death rates, resulting in no population growth. Countries above the line are growing population, while countries below are shrinking. A few countries fall a bit below this line [@wikipopulation; @wikibirthrate; @wikideathrate].
```

[](#fig:population:birthtodeathrates) hints at the narrative. Countries are spread into an arc, one segment occupying a band between 5–10 deaths per 1000 people per year and birth rates lower than 20 per 1000 people per year. Another set of countries (many of which are in Africa) have birth rates above 20 per 1000 per year, but also show higher death rates. The narrative arc is that a country may start near Lesotho, at high death and birth rates, then migrate over toward Nigeria as death rates fall (and birth rates experience a temporary surge). Next both death and birth rates fall and run through a progression toward Pakistan, India, the U.S., and finally the European steady state. [](#fig:population:demogtransition) schematically illustrates the typical journey.

The demographic transition receives widespread advocacy among Western intellectuals for its adoption, often coupled with the sentiment that it can't come soon enough. Indeed, the humanitarian consequences appear to be positive and substantial: fewer people living in poverty and hunger; empowered women; better education; more advanced jobs; and greater tolerance in the society. It might even seem condemnable *not* to wish for these things for all people on Earth.

```{figure} ../figures/Ch03_Population/_page_59_Figure_8.jpeg
:label: fig:population:demogtransition
:width: 100%
:align: center
:alt: Schematic of how the demographic transition may play out in the space plotted in [](#fig:population:birthtodeathrates) At points A and D, birth rates and death rates are equal, resulting in no population growth. Typically, death rates decline while birth rates increase (point B), and eventually death rates reach a floor while birth rates begin to fall (at C).
Schematic of how the demographic transition may play out in the space plotted in [](#fig:population:birthtodeathrates) At points A and D, birth rates and death rates are equal, resulting in no population growth. Typically, death rates decline while birth rates increase (point B), and eventually death rates reach a floor while birth rates begin to fall (at C).
```

However, we need to understand the consequences. Just because we *want* something does not mean nature will comply. Do we have the resources to accomplish this goal? If we fail in pursuit of a global demographic transition, have we unwittingly unleashed even *greater* suffering on humanity by increasing the total number of people who can no longer be supported? It is possible that well-intentioned actions produce catastrophic results, so let us at least understand what is at stake. It may be condemnable *not to wish* for a global demographic transition, but failing to explore potential downsides may be equally ignoble.

## Geographic Considerations

[](#fig:population:popgrowbycountry) shows the net population rate (birth minus death rate) on a world map. Africa stands out as the continent having the largest net population growth rate, and has been the focus of much attention when discussing population dynamics.

% ../figures/Ch03_Population/_page_60_Figure_4.jpeg was the original image
```{figure} https://upload.wikimedia.org/wikipedia/commons/thumb/2/2d/Population-growth-rate-2023-OWID.png/1280px-Population-growth-rate-2023-OWID.png
:label: fig:population:popgrowbycountry
:width: 100%
:align: center
:alt: Net population growth rate by country: birth rate minus death rate per 1000 people per year. The highest net growth (darkest shading) is Niger, in Saharan Africa [@wikibirthrate; @wikideathrate].
Net population growth rate by country: birth rate minus death rate per 1000 people per year. The highest net growth (darkest shading) is Niger, in Saharan Africa [@wikibirthrate; @wikideathrate].
```

But let us cast population rates in different countries in a new light. Referring to [](#fig:population:popgrowbycountry) it is too easy to look at Niger's net population rate—which is about ten times higher than that of the U.S. (see [](#ex:population:USbirthrate)—and conclude that countries similar to Niger present a greater risk to the planet in terms of population growth. However, our perspective changes when we consider absolute population levels. Who cares if a country's growth rate is an explosive 10% if the population is only 73 people?[^23] 

[](#fig:population:absgrowthcountry) multiplies the net rate by population to see which countries contribute the most *net new people* to the planet each year, and [](#table:population:toptenpop) lists the top ten. Africa no longer appears to be the most worrisome region in this light.[^24] India is the largest people-producing country at present, adding almost 18 million per year. Far behind is China, in second place. The U.S. adds about 1.6 million per year, a little beyond the top ten. This exercise goes to show that context is important in evaluating data.

[^23]: But check back in 100 years!
[^24]: Although, the continent as a whole accounts for 35% of the total added population each year.

```{figure} ../figures/Ch03_Population/_page_61_Figure_1.jpeg
:label: fig:population:absgrowthcountry
:width: 100%
:align: center
:alt: Absolute population growth rate by country: how many millions of people are added per year (birth rate minus death rate times population) [@wikipopulation; @wikibirthrate; @wikideathrate].
Absolute population growth rate by country: how many millions of people are added per year (birth rate minus death rate times population) [@wikipopulation; @wikibirthrate; @wikideathrate].

```

```{table} Top ten populators [@wikipopulation; @wikibirthrate; @wikideathrate], in terms of absolute number of people added to each country. Birth rates and death rates are presented as number per 1,000 people per year. These ten countries account for 55% of population growth worldwide.
:label: table:population:toptenpop

| Country     | Population (millions) | Birth Rate | Death Rate | Annual Millions Added |
|------------:|----------------------:|-----------:|-----------:|--------------------:|
| India       | 1366                  | 20.0       | 7.1        | 17.7                |
| China       | 1434                  | 12.1       | 7.1        | 7.2                 |
| Nigeria     | 201                   | 38.0       | 15.3       | 4.6                 |
| Pakistan    | 216                   | 24.9       | 7.3        | 3.8                 |
| Indonesia   | 271                   | 17.6       | 6.3        | 3.1                 |
| Ethiopia    | 112                   | 36.1       | 10.7       | 2.8                 |
| Bangladesh  | 163                   | 20.2       | 5.6        | 2.3                 |
| Philippines | 108                   | 24.2       | 5.0        | 2.1                 |
| Egypt       | 100                   | 26.8       | 6.1        | 2.1                 |
| DR Congo    | 87                    | 36.9       | 15.8       | 1.8                 |
| Whole World | 7711                  | 19.1       | 8.1        | 86                  |
```

Adding another relevant perspective, when one considers that the percapita energy consumption in the United States is more than 200 times that of Niger,[^25]  together with the larger U.S. population, we find that the *resource impact* from births is almost 400 times higher for the U.S. than for Niger.[^26] On a per capita basis, a citizen of the U.S. places claims on future resources at a rate 28 times higher than a citizen of Niger via population growth.[^27] On a finite planet, the main reason we *care* about population growth is in relation to limited resources. Thus from the resource point of view, the problem is not at all confined to the developing world. [](#table:population:toptenenergy) indicates how rapidly the top ten countries are creating energy demand (as a proxy to resource demands in general) based on population growth alone. [](#fig:population:toptenenergy) provides a graphical perspective of the same (for all countries). For reference, one gigawatt (GW) is the equivalent of a large-scale nuclear or coal-fired power plant. So China, the U.S., and India each add the equivalent of 10–20 such plants per year just to satisfy the demand created by population growth.[^28]

[^25]: The average American rate of energy use is 10,000 W vs. 50 W for Niger.
[^26]: In other words, for every additional kilogram of coal, steel, or whatever required by Niger's added population, the U.S. will require 400 kg of the same to satisfy its population growth.
[^27]: 28 is smaller than 400 by the ratio of populations in the two countries.
[^28]: This does not even consider rising standards placing additional burdens.

```{table} Top ten countries for growth in energy demand. Populations are in millions. Poweris in Watts or 10<sup>9</sup> W (= GW). The power added annually is the absolute increase in demand *due to population growth*, and is a proxy for resource demands in general. The last column provides some measure of an individual citizen's share of the responsibility in terms of increasing pressure on resources. The top three contributors to new power demand via population growth alone (China, the U.S., and India) account for about a third of the global total. [wikienergyconsumption; @wikipopulation; @wikibirthrate; @wikideathrate]
:label: table:population:toptenenergy
| Country       | Population(×10<sup>6</sup>) | Annual<br>Growth (×10<sup>6</sup>) | Per Capita Power (W) | Power Added Annually (GW) | Power Added Per Citizen (W) |
|--------------:|---------------------:|---------------------------:|------------------------:|--------------------------------:|----------------------------------:|
| China         | 1434                 | 7.2                        | 2800                    | 20.2                            | 14                                |
| United States | 329                  | 1.6                        | 10,000                  | 15.6                            | 48                                |
| India         | 1366                 | 17.7                       | 600                     | 10.5                            | 8                                 |
| Saudi Arabia  | 34                   | 0.54                       | 10,100                  | 5.5                             | 160                               |
| Iran          | 83                   | 1.0                        | 4300                    | 4.3                             | 52                                |
| Mexico        | 128                  | 1.7                        | 2000                    | 3.3                             | 26                                |
| Indonesia     | 271                  | 3.1                        | 900                     | 2.8                             | 10                                |
| Brazil        | 211                  | 1.3                        | 2000                    | 2.7                             | 13                                |
| Egypt         | 100                  | 2.1                        | 1200                    | 2.5                             | 25                                |
| Turkey        | 83                   | 0.85                       | 2100                    | 1.8                             | 21                                |
| Whole World   | 7711                 | 86                         | 2300                    | 143                             | 18.4                              |
```

```{figure} ../figures/Ch03_Population/_page_62_Figure_3.jpeg
:label: fig:population:toptenenergy
:width: 100%
:align: center
:alt: Graphical representation of [](#table:population:toptenenergy) for all countries. Dots, whose size is proportional to population, indicate how many people are added per year, and how much additional energy demand is created as a consequence. Color indicates the added population-growth-driven power demand an individual citizen is responsible for generating each year as a member of the society. Negative cases (contracting) include Russia, Japan, Germany, and Ukraine [wikienergyconsumption; @wikipopulation; @wikibirthrate; @wikideathrate].
Graphical representation of [](#table:population:toptenenergy) for all countries. Dots, whose size is proportional to population, indicate how many people are added per year, and how much additional energy demand is created as a consequence. Color indicates the added population-growth-driven power demand an individual citizen is responsible for generating each year as a member of the society. Negative cases (contracting) include Russia, Japan, Germany, and Ukraine [wikienergyconsumption; @wikipopulation; @wikibirthrate; @wikideathrate].
```

The last column in [](#table:population:toptenenergy) is the per-citizen cost, meaning, for instance that each person in the U.S. adds about 50 Watts per year of energy demand via the country's net population growth rate.[^29] In this sense, the last column is a sort of "personal contribution" an individual makes to the world's resource demands via net population rates and consumption rates in their society. Those having high scores should think twice about assigning blame externally, and should perhaps tend to their own house, as the saying goes. 

Before departing this section, let us look at continent-scale regions rather than individual countries in terms of adding people and resource demands. [](#table:population:poppressures) echoes similar information to that in [](#table:population:toptenenergy) in modified form. What we learn from this table is that Asia's demands are commensurate with their already-dominant population; North America creates the next largest pressure despite a much smaller population; Africa is significant in terms of population growth, but constitutes only 10% of resource pressure at present. Finally, Europe holds 10% of the globe's people but lays no claim on added resources via population growth, resembling the target end-state of the demographic transition.[^30]

```{table} Population pressures from regions of the world, ranked by added power demand. Some of the columns are expressed as percentages of the total. The bottom row has totals in millions of people or total GW in place of percentages. [wikienergyconsumption; @wikipopulation; @wikibirthrate; @wikideathrate]
:label: table:population:poppressures

| Country     | Population (%) | Annual Growth (%) | Per Capita<br>Power (W) | Power Added Annually (%) | Power Added Per Citizen (W) |
|------------:|---------------:|------------------:|------------------------:|-------------------------:|----------------------------:|
| Asia        | 59.7           | 55.1              | 1800                    | 60.5                     | 18.9                        |
| N. America  | 7.6            | 5.5               | 7100                    | 23.0                     | 56.1                        |
| Africa      | 16.9           | 34.7              | 500                     | 9.9                      | 10.8                        |
| S. America  | 5.5            | 4.4               | 2000                    | 5.4                      | 18.1                        |
| Oceania     | 0.5            | 0.5               | 5400                    | 1.5                      | 49.5                        |
| Europe      | 9.7            | −0.1              | 4900                    | −0.3                     | −0.6                        |
| Whole World | 7,711 M        | 86 M              | 2300                    | 143 GW                   | 18.4                        |
```
[^29]: citizen of Niger, by comparison, only adds 1.7 W of demand per year on energy resources via population growth.
[^30]: Note that European countries are nervous about their decline in a growing, competitive world.

## Cost of the Demographic Transition

A final point relates to the trajectory depicted in [Figure](#page-59-1) [3.12](#page-59-1) for [demo](#page-445-2)[graphic transitions:](#page-445-2) death rate decreases first while birth rates remain high—or rise even higher—before starting to come down. An example sequence is illustrated in [Figure](#page-63-2) [3.16:](#page-63-2) initially the rates are high (at 푟1), and the same (resulting in steady population); then the death rate transitions to a new low rate (푟2) over a time 푇; and the birth rate begins to fall some time 휏 later before matching the death rate and stabilizing population again. The yellow-shaded area between the curves indicates the region where birth rate exceeds death rate, leading to a net population growth (a surge in population).

The amount of growth in the surge turns out to be proportional to the exponential of the area between the curves. For this trapezoid cartoon, the area is just the base ( $\tau$ ) times the height (rate difference), so that the population increase looks like  $e^{(r_1-r_2)\tau}$ , where  $r_1$  is the initial rate per year and  $r_2$  is the final rate. Note in the cartoon example of [Figure 3.16,](#page-63-2) The actual curves may take any number of forms, but the key point is that delayed onset of birth rate decrease introduces a population surge, and that magnitude of the surge grows as the area between the curves increases.**Example 3.3.2** If we start at a birth/death rate of 25 per 1,000 per year ( $r_1 = 0.025$ ), end up at 8 ( $r_2 = 0.008$ ; verify that these numbers are reasonable according to [Figure](#page-59-0) [3.11\)](#page-59-0), and have a delay of  $\tau = 50$  years for the birth rate to start decreasing, we see the population increasing by a factor of
$$
e^{(r_1 - r_2)\tau} = e^{(0.025 - 0.008) \cdot 50} = e^{0.85} = 2.34.
$$

**Table 3.5:** 

30: Note that European countries are nervous about their decline in a growing, competitive world.

<span id="page-63-2"></span>![](../figures/Ch03_Population/_page_63_Figure_10.jpeg)

**Figure 3.16:** Schematic demographic transition time sequence.

the area between the curves is only dependent on the rate difference (height) and the delay, 휏. The time it takes to complete the transition, 푇, is irrelevant, as the area of the parallelogram is just the base times the height. Thus the population surge associated with a demographic transition is primarily sensitive to the rate difference and the delay until birth rate begins to decline.

#### This means that the population more than doubles, or increases by 134%.

So to effect a demographic transition means to increase the population burden substantially. Meanwhile, the transitioned population consumes resources at a greater rate—a natural byproduct of running a more advanced society having better medical care, education, and employment opportunities. Transportation, manufacturing, and consumer activity all increase. The net effect is a double-whammy: the combined impact of a *greater* population using *more* resources per capita. The resource impact on the planet soars.

The pertinent question is whether the Earth is prepared to host a dramatic increase in resource usage. Just because we might find appealing the idea that all countries on Earth could make it through the demographic transition and live at a first-world standard *does not mean nature has the capacity to comply*. The U.S. per-capita energy usage is roughly five times the current global average. To bring 7 billion people to the same standard would require five times the current scale. Completion of a global demographic transition would roughly double the current world population so that the total increase in energy would be a factor of ten. The blue-dashed projection in [Figure](#page-64-0) [3.17](#page-64-0) looks rather absurd as an extension of the more modest—but still rather remarkable—energy climb to date. As we are straining to satisfy current energy demand, the "amazing dream" scenario seems unlikely to materialize.

Energy in this context is a proxy for other material resources. Consider the global-scale challenges we have introduced today: deforestation, fisheries collapse, water pressures, soil degradation, pollution, climate change, and species loss, for instance. What makes us think we can survive a global demographic transition leading to a consumption rate many times higher than that of today? Does it not seem that we are already approaching a breaking point?

If nature won't let us realize a particular dream, then is it morally responsible to pursue it? This question becomes particularly acute if the very act of *pursuing* the dream increases the pressure on the system and *makes failure even more likely*. Total suffering might be maximized if the population builds to a point of collapse. In this sense, we cleverly stack the most possible people into the stadium to witness a most spectacular event: the stadium's collapse—which only happened because we packed the stadium. You see the irony, right?

The drive to realize a global demographic transition is strong, for the obvious set of reasons discussed above (improved quality of life, educational opportunity, greater tolerance, dignity, and fulfillment). Challenging the vision may be an uphill battle, since awareness about resource limits is not prevalent. This may be an example of the natural human tendency to extrapolate: we have seen the benefits of the demographic transition in many countries over the last century, and may expect this trend to

<span id="page-64-0"></span>![](../figures/Ch03_Population/_page_64_Figure_7.jpeg)

**Figure 3.17:** What our energy demand would have to do (blue-dashed line) if the growing global population (here projected as a red-dashed logistic curve) grew its percapita energy consumption to current U.S. standards by the year 2100 (a factor-of-five increase). Historical energy and population are represented as solid curves. The departure from past reality would have to be staggering [\[15,](#page-432-2) [16\]](#page-432-1).

continue until all countries have completed the journey. But bear in mind that earlier successes transpired during times in which global resource availability was not a major limitation. If conditions change, and we reach a "full" earth, past examples may offer little relevant guidance.

## <span id="page-65-0"></span>**3.4 Touchy Aspects**

#### <span id="page-65-1"></span>**3.4.1 Population Discussions Quickly Get Personal**

Some of the decisions we make that translate into impact on our physical world are deeply personal and very difficult to address. No one wants to be told what they should eat, how often they should shower, or what temperature they should keep their dwelling. But the touchiest of all can be reproduction. It can be tricky to discuss population concerns with someone who has kids. Even if not intentional, it is too easy for the topic to be perceived as a personal attack on their own choices. And we're not talking about choices like what color socks to wear. Children are beloved by (most) parents, so the insinuation that having children is bad or damaging quickly gets tangled into a sense that their "angel" is being attacked—as is their "selfish" decision to have kids (see [Box](#page-65-2) [3.2\)](#page-65-2). The disconnect can be worse the larger the number of kids someone has. Couples having two kids take some solace in that they are exercising net-zero "replacement." Having two kids is not a *strict* replacement,One common side-step is to focus attention on the high birthrates in other countries, so that the perceived fault lies elsewhere. As pointed out above, if stress on the planet—and living within our means—is what concerns us, undeveloped countries are not putting as much pressure on global resources as many of the more affluent countries are. So while pointing elsewhere offers a bit of a relief, and is a very natural tendency, it does not get the whole picture.

The overall point is to be aware of the sensitive nature of this topic when discussing with others. Making someone feel bad about their choices even if unintentionally—might *in rare cases* result in an appreciation and greater awareness. But it is *more likely* to alienate a person from an otherwise valuable perspective on the challenges we face.

#### <span id="page-65-2"></span>**Box 3.2: Which is More Selfish?**

Parents, many of whom sacrifice dearly in raising kids—financially, emotionally, and in terms of time investment—understandably view their tireless commitment as being selfless: they often give up their own time, comfort, and freedom in the process. It is understandable, then, that they may view those not having kids as being selfish: the opposite of selfless. But this can be turned on its head. Why, in that parents and children overlap (doubleoccupancy) on Earth. But the practice is at least consistent with a steady state.

exactly, did they decide to have kids and contribute to the toll on our planet? It was their choice (or inattention) that placed them in parental roles, and the entire planet—not just humans—pays a price for their decision, making it seem a bit selfish.<sup>31</sup> 31: Reasons for having children are numer-In the end, almost any decision we make can be called selfish, since we usually have our own interests at least partly in mind. So it is pointless to try assigning more or less selfishness to the decision to have kids or not to have them. But consider this: if the rest of the Earth—all its plants and creatures—had a say, do you think they would vote for adding another human to the planet? Humans have the *capacity*, at least, to consider a greater picture than their own self interest, and provide representation to those sectors that otherwise have no rights or voice in our highly human-centric system.

#### <span id="page-66-0"></span>**3.4.2 Population Policy**

What could governments and other organizations do to manage popula-
tion? Again, this is touchy territory, inviting collision between deeply
personal or religious views and the state. China initiated a one-child pol-
icy in 1979 that persisted until 2015 (exceptions were granted depending
on location and gender). The population in China never stopped climb-
ing during this period, as children born during prior periods of higher
birth rates matured and began having children of their own—even if
restricted in number. The population curve in China is not expected to
flatten out until sometime in the 2030–2040 period.<sup>32</sup> Such top-down
policies can only be enacted in strong authoritarian regimes, and would
be seen as a severe infringement on personal liberties in many countries.
Religious belief systems can also run counter to deliberate efforts to limit
population growth. In addition, shrinking countries are at a competitive
disadvantage in global markets, often leading to policies that incentivize
having children.

The net effect of the various exceptions
meant that for most of this period half of
Chinese parents could have a second child.

<sup>32</sup>: This is another case of delay in negative
feedback resulting in overshoot.

One striking example of rarely-achieved sustainable population control comes from the South Pacific island of Tikopia [\[21\]](#page-432-7). Maintaining a stable population for a few thousand years on this small island involved not only adopting food practices as close to the island's natural plants as possible, but also invoking strict population controls. The chiefs in this egalitarian society routinely preached zero population growth, and also prevented overfishing. Strict limits were placed on family size, and cultural taboos kept this small island at a population around 1,200.<sup>33</sup> Population control methods included circumventing insemination, abortion, infanticide, suicide, or "virtual suicide," via embarking on dangerous sea voyages unlikely to succeed. In this way, the harshness of nature was replaced by harsh societal norms that may seem egregious to us. When Christian missionaries converted inhabitants in the twentieth century, the practices of abortion, infanticide and suicide were quenched and the population
  

[21]: Diamond (2005), *Collapse: How Societies* Choose to Fail or Succeed
  

33: A group size of 1,200 is small enough to prevent hiding irresponsible actions behind anonymity.ous: genetic drive; family name/tradition; labor source; care in old age; companionship and love (projected onto not-yet-existing person). Note that adoption can also satisfy many of these aims without contributing additional population.

meant that for most of this period half of Chinese parents could have a second child.

feedback resulting in overshoot.

*Choose to Fail or Succeed*

prevent hiding irresponsible actions behind anonymity.

began to climb, leading to famine and driving the population excess off the island.  
Nature, it turns out, is indifferent to our belief systems.In the end, personal choice will be important, if we are to tame the population predicament. Either conditions will be too uncertain to justify raising children, or we adopt values that place short term personal and human needs into a larger context concerning ecosystems and long-term human happiness.

# <span id="page-67-0"></span>**3.5 Upshot: Everything Depends on Us**

We would likely not be discussing a finite planet or limits to growth or climate change if only one million humans inhabited the planet, even living at United States standards. We would perceive no meaningful limit to natural resources and ecosystem services. A common knee-jerk reaction to a statement Conversely, it is not difficult to imagine that 100 billion people on Earth would place a *severe* strain on the planet's ability to support us—especially if trying to live like Americans—to the point of likely being impossible. If we had to pick a single parameter to dial in order to ease our global challenges, it would be hard to find a more effective one than population.

Maybe we need not take any action. Negative feedback *will* assert itself strongly once we have gone too far—either leading to a steady approach to equilibrium or producing an overshoot/collapse outcome. Nature *will* regulate human population one way or another. It just may not be in a manner to our liking, and we have the opportunity to do better via awareness and choice.

Very few scholars are unconcerned about population pressure. Yet the issue is consistently thorny due to both its bearing on personal choice and a justified reluctance to "boss" developing nations to stop growing prior to having an opportunity to naturally undergo a demographic transition for themselves. Conventional thinking suggests that undergoing the demographic transition ultimately is the best solution to the population problem. The question too few ask is whether the planet can support this path for all, given the associated population surge and concomitant demand on resources. If not, pursuit of the transition for the world may end up causing more damage and suffering than would otherwise happen due to increased populations competing for dwindling resources.

# <span id="page-67-1"></span>**3.6 Problems**

1. The text accompanying [Figure](#page-49-0) [3.1](#page-49-0) says that Earth currently hosts the equivalent of 25 billion nineteenth-century-level energy consumers. If we had maintained our nineteenth-century energy appetite but

belief systems.

that we would be better off with a smaller population is to demand an answer to who, exactly, we propose eliminating. Ideally, we should be able to discuss an important topic like population without resorting to accusations of advocating genocide. Of course we need to take care of those already alive, and address the problem via future reproductive choices.

followed the same population curve, what would our global power demand be today, in TW? How does this compare to the actual 18 TW we use today?

<span id="page-68-0"></span>2. Notice that on logarithmic plots,<sup>34</sup> factors of ten on the logarithmic 34: See, for example, Figures [3.3](#page-50-3) and [3.4.](#page-50-1) axis span the *same distance*. This applies for *any* numerical factor—not just ten.<sup>35</sup> 35: This is due to the property of logarithms Shorter (minor) tick marks between labeled (major) ticks multiply the preceding tick label by 2, 3, 4, 5, 6, 7, 8, 9. The graphic below illustrates the constant distance property for a factor of two.<sup>36</sup> 36: The green bars indicate that the same Now try a different multiplier (not 2 or 10), measuring the distance between tick marks, and report/draw how you graphically verified that your numerical factor spans the same distance no matter where you "slide" it on the axis.
![](../figures/Ch03_Population/_page_68_Figure_3.jpeg)

- <span id="page-68-1"></span>3. Looking at [Figure](#page-50-3) [3.3,](#page-50-3) if humans had continued the slow growth phase characteristic of the period until about 1700, what does the *graph* suggest world population would be today, approximately, if the magenta line were extended to "now?"<sup>37</sup> marks work. Put the answer in familiar terms, measured in millions or billions, depending on what is most natural.<sup>38</sup>
- 4. Looking at [Figure](#page-50-1) [3.4,](#page-50-1) if humans had continued the moderate growth phase characteristic of the period from the year 1000 to 1700, what does the *graph* See margin notes for [Problem](#page-68-1) [3.](#page-68-1) suggest world population would be today, approximately, if the magenta line were extended to "now?"
- 5. If we were to continue a 1% population growth trajectory into the future, work out how many years it would take to go from 7 billion people to 8 billion, and then from 8 billion to 9 billion.
- <span id="page-68-3"></span>6. At present, a billion people are added to the planet every 12 years. If we maintain a 1% growth rate in population, what will global population be in 2100 (use numbers in [Table](#page-51-0) [3.2](#page-51-0) as a starting point), and how quickly will we add each new billion at that point?
- <span id="page-68-2"></span>7. A decent approximation to recent global population numbers using a logistic function is<sup>39</sup> 39: See [Eq.](#page-53-2) [3.6.](#page-53-2)

$$
P = \frac{14}{1 + \exp[-0.025 \times (year - 2011)]}
$$

in billions of people. First verify that inserting the year 2011 results in 7 (billion), and then add a column to [Table](#page-51-0) [3.2](#page-51-0) for the "prediction" resulting from this function. Working back into the past, when does it really start to deviate from the truth, and why do you

Hint: It is perfectly acceptable to hold a (preferably transparent) straight-edge up to a graph!

34: See, for example, Figures 3.3 and 3.4.

35: This is due to the property of logarithms

that  $\log \left(\frac{a}{b}\right) = \log a - \log b$ . The property applies for any base, so  $\log_{10}$  and ln behave the same way.distance from 1 to 2 applies to 3–6, 40–80, and 500–1,000.

37: Determine graphically (may need to zoom in). See [Problem](#page-68-0) [2](#page-68-0) and the associated graphic to better understand how the tick

38: I.e., don't say 0.01 billion if 10 million is more natural, or 8,000 million when 8 billion would do.

See margin notes for Problem 3.

39: See Eq. 3.6.

think that is (hint: what changed so that we invalidated a single, continuous mathematical function)?

- 8. Using the logistic model presented in [Problem](#page-68-2) [7,](#page-68-2) what would the population be in the year 2100? How does this compare to the exponential result at 1% growth as in [Problem](#page-68-3) [6?](#page-68-3)
- 9. Which of the following are examples of positive feedback, and which are examples of negative feedback?
	- a) a warming arctic melts ice, making it darker, absorbing more solar energy
	- b) if the earth's temperature rises, its infrared radiation to space increases, providing additional cooling
	- c) a car sits in a dip; pushing it forward results in a backward force, while pushing it backward results in a forward force
	- d) a car sits on a hill; pushing it either way results in an acceleration (more force, thanks to gravity) in that direction
	- e) a child wails loudly and throws a tantrum; to calm the child, parents give it some candy: will this encourage or discourage similar behaviors going forward?
- 10. Think up an example from daily life (different from examples in the text) for how a delay in negative feedback can produce overshoot, and describe the scenario.
- 11. Pick five countries of interest to you not represented in any of the tables in this chapter and look up their birth rate and death rate [\[19,](#page-432-5) [20\]](#page-432-6) , then find the corresponding dot on [Figure](#page-59-0) [3.11,](#page-59-0) if possible.<sup>40</sup> 40: Numbers may change from when the based on dot size. At the very least, identify the corresponding region on the plot.
- <span id="page-69-0"></span>12. A country in the early stages of a demographic transition may have trimmed its death rate to 15 per 1,000 people per year, but still have a birth rate of 35 per 1,000 per year. What does this amount do in terms of net people added to the population each year, per 1,000 people? What rate of growth is this, in percent?
- 13. If the population of the country in [Problem](#page-69-0) [12](#page-69-0) is 20 million this year, how many people would we expect it to have next year? How many were born, and how many died during the year?
- 14. [Figure](#page-59-0) [3.11](#page-59-0) shows Egypt standing well above China in terms of excess birth rate compared to death rate.<sup>41</sup> Yet [Table](#page-61-1) [3.3](#page-61-1) indicates 41: . . . much farther from dashed line that China contributes a much larger annual addition to global population than does Egypt. Explain why. Then, using the first four columns in [Table](#page-61-1) [3.3,](#page-61-1) replicate the math Show work and add one more decimal place that produced the final column's entries for these two countries to reinforce your understanding of the interaction between birth and death rates and population in terms of absolute effect.
- 15. In a few clear sentences, explain why the maps in [Figure](#page-60-1) [3.13](#page-60-1)

Comparison of this problem and [Problem](#page-68-3) [6](#page-68-3) highlights the difference the choice of mathematical model can make.

[\[19\]](#page-432-5): (2016), *List of Sovereign States and Dependent Territories by Birth Rate* [\[20\]](#page-432-6): (2011), *List of Sovereign States and Dependent Territories by Mortality Rate*

plot was made; population can help settle

41: ...much farther from dashed line

to the answer as a way to validate that you did more than copy the table result.

and [Figure](#page-61-0) [3.14](#page-61-0) look so different, in terms of which countries are shaded most darkly?

- 16. [Table](#page-62-0) [3.4](#page-62-0) indicates which countries place the highest populationdriven new demand on global resources using energy as a proxy. Which countries can American citizens regard as contributing more total resource demand? The point is that the U.S. is a major con-At the individual citizen-contribution level, what other citizens can Americans identify as being responsible for a greater demand on resources via population growth?
- 17. The last two columns in [Table](#page-62-0) [3.4](#page-62-0) were computed for this book from available information on population, birth and death rates, and annual energy usage for each country (as represented in the first four columns; references in the caption). Use logical reasoning to replicate Careful about <sup>10</sup><sup>6</sup> factors and GW = <sup>10</sup><sup>9</sup> W. the calculation that produces the last two columns from the others and report how the computation goes, using an example from the table.
- 18. The bottom row of [Table](#page-62-0) [3.4](#page-62-0) is important enough to warrant having students pull out and interpret its content. Some students may see this as free/easy What is world population, in billions? How many people are added to the world each year? What is the typical power demand for a global citizen (and how does it compare to the U.S.)? If a typical coal or nuclear plant puts out 1 GW of power, how many power-plant-equivalents must we add each year to keep up with population increase? And finally, how much power (in W) is added per global citizen each year due to population growth (and it is worth reflecting on which countries contribute more than this average)?
- 19. If you were part of a global task force given the authority to make binding recommendations to address pressures on resources due to population growth, which three countries stand out as having the largest impact at present? Would the recommendations be the same for all three? If not, how might they differ?
- 20. [Table](#page-63-1) [3.5](#page-63-1) helps differentiate concerns over which region contributes pressures in raw population versus population-driven resource demand. By taking the ratio of population growth (in %) to population (as % of world population), we get a measure of whether a region is "underperforming" or "overperforming" relative to its population. Likewise, by taking the ratio of the added power (in %) to population, we get a similar measure of performance in resource demand. In this context, which region has the highest ratio for population pressure, and which region has the highest ratio for population-induced pressure on energy resources?
- 21. If a country starting out at 30 million people undergoes the demographic transition, starting at birth/death rates of 35 per 1,000 per year and ending up at 10 per 1,000 per year, what will the final population be if the delay, 휏, is 40 years?

tributor to increased resource demand via population growth.

Careful about  $10^6$  factors and GW =  $10^9$  W.

points, but consider the value in internalizing the associated information.

For instance, Oceania has a ratio of 1.0 for population growth (0.5% of population growth and 0.5% of global population), meaning it is not over- or under-producing relative to global norms. But in terms of power, it is 3 times the global expectation (1.5 divided by 0.5).

<span id="page-71-0"></span>22. The set of diagrams below show five different time sequences on the left akin to [Figure](#page-63-2) [3.16,](#page-63-2) labeled 1–5. The first four on the left have increasing 휏 (delay until birth rate begins falling), and the last increases birth rate before falling again. On the right are five trajectories in the birth/death rate space (like [Figure](#page-59-1) [3.12\)](#page-59-1), scrambled into a different order and labeled A–E.<sup>42</sup> 42: Note that figures A. and E. differ only Deduce how the corresponding trajectory for each time sequence would appear in the birth/death rate plot on the right, matching letters to numbers for all five.

by whether the transition pauses (dwells) at the corner for some time.

![](../figures/Ch03_Population/_page_71_Figure_3.jpeg)

- <span id="page-71-1"></span>23. Referring to the figures for [Problem](#page-71-0) [22](#page-71-0) (and described within the same problem), which pair<sup>43</sup> 43: . . . number and associated letter; not corresponds to the largest population surge, and which pair produces the smallest? Explain your reasoning, consistent with the presentation in the text.
- 24. Referring to the figures for [Problem](#page-71-0) [22](#page-71-0) (and described within the same problem), which pair<sup>44</sup> 44: . . . number and associated letter; not is most similar to the actual trajectory we witness (i.e., [Figure](#page-59-0) [3.11\)](#page-59-0), and what does this say about the

necessarily arranged next to each other

necessarily arranged next to each other

population cost of the demographic transition in the context of [Problem](#page-71-1) [23?](#page-71-1)

- 25. Considering [Figure](#page-59-0) [3.11](#page-59-0) in the context of a trajectory (as in [Figure](#page-59-1) [3.12\)](#page-59-1), would it appear that most countries in the world have begun the demographic transition? Have very few of them started? Is it about half-and-half? Justify your answer.
- 26. Express your view about what you learn from [Figure](#page-64-0) [3.17.](#page-64-0) Do you sense that the prescribed trajectory is realistic? If so, justify. If not, what about it bothers you? What does this mean about the goal of bringing the (growing) world to "advanced" status by the end of this century? Are we likely to see this happen?
- 27. Make as compelling an argument as you can for why we should promote the demographic transition worldwide for those countries who have not yet "arrived" at the lower-right corner of [Figure](#page-58-0) [3.10.](#page-58-0) What are the positive rewards?
- 28. Make as compelling an argument as you can for why pursuit of the demographic transition may be ill-advised and potentially create rather than alleviate hardship. What are the downsides?
- 29. List the pros and cons a young person without children might face around the decision to have a biological child of their own<sup>45</sup> 45: Assume for the purpose of the question Consider not only personal contexts, but external, global ones as that it is biologically possible. well, and thoughts about the future as you perceive it. It does not matter which list is longer or more compelling, but it is an exercise many will go through at some point in life—although maybe not explicitly on paper.
- 30. Do you think governments and/or tribal laws have any business setting policy around child birth policies? If so, what would you consider to be an acceptable form of control? If not, what other mechanisms might you propose for limiting population growth (or do you even consider that to be a priority or at all appropriate)?

Hint: think about what the graph would look like in these scenarios.

45: Assume for the purpose of the question
that it is biologically possible.

:::{glossary}
exponential growth
: happens when the rate of growth — as a percentage or fraction — is constant.

hockey stick
: a term used to describe plots that suddenly shoot up after a very long time of relative inaction. Plots of human population, atmospheric CO<sub>2</sub>, energy use, all tend to show this characteristic—which resembles an exponential curve.

Green Revolution
: refers to the modernization of agricultural practices worldwide beginning around 1950, when fossil fuels transformed both fertilization and mechanization.

positive feedback
: involves a reaction to some stimulus in the same direction as the stimulus, thus amplifying the effect. Positive feedback leads to an unstable, runaway process—like exponential growth.

differential equation
: an equation that relates functions and their derivatives. The subject is often sequenced after calculus within a curriculum.

logistic curve
: describes a mathematical model in which rate of growth depends on how close the population is to the carrying capacity. The resulting population curve over time is called the logistic function, or more informally, an S-curve.

death rate
: quantifies the number of deaths per 1000 people per year, typically. Numbers tend to be in the 5–30 range.

demographic transition
: refers to the process in which an undeveloped country initially having high birth rate and high death rate transitions to low death rates followed by low birth rates as medical and resource conditions improve.
:::