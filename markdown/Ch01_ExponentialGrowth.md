---
title: Chapter 1 - Exponential Growth
banner: ../figures/Ch01_ExponentialGrowth/banner.jpeg
numbering:
  headings:
  heading_1:
    start: 2
kernelspec:
  name: python3
  display_name: 'Python 3'
---

(chap:expgrowth)=
# Exponential Growth

Humans have amazing strengths, but also significant weaknesses. Chief among them, perhaps, is our collective difficulty in grasping the mathematical consequences of exponential growth.[^1] This is an ironic state, given that our economic and political goals are often geared explicitly to support continued growth. The degree to which an expectation and desire for continued growth is woven into our society makes it important to examine the phenomenon carefully, so that we might avoid building upon a shaky foundation. In this chapter, we explore the general nature of exponential growth, in order to understand the impossibility of its long-term continuance by way of exposing various absurd consequences that uninterrupted growth prescribes. The upshot[^2] is that our societal framework eventually must face a mandatory departure from the current model-a piece of knowledge we should all lodge into the backs of our minds. Subsequent chapters will address applications to economic and population growth-including more realistic logistic growth curves, then pivot toward nailing down limits imposed by our finite planet.

(sec:expgrowth:bacteria)=
# Bacteria in a Jar

One hallmark of exponential growth is that the time it takes to double in size, or the doubling time, is constant. An important and convenient concept we will repeatedly use in this chapter is the rule of 70:

```{note} Definition: Rule of 70
The doubling time associated with a percentage growth rate is just 70 divided by the percentage rate. A 1% growth rate doubles in 70 years, while a 2% rate doubles in 35 years, and a 10% rate doubles in 7 years. It also works for other timescales: if pandemic cases are increasing at a rate of 3.5% per day, the doubling time is 20 days.
```

[^1]: ... a nod to Al Bartlett, who worked to raise awareness about exponential growth

[^2]: The word "upshot" means final result or bottom-line. Each chapter has an Upshot at the end.

Note that any growth, however slow, can be characterized by a doubling time, even if the process does not involve discrete steps of doubling.

We will see how the rule of 70 arises mathematically later in this chapter. But first, it is more important to understand the *consequences*. To make the math simple, let's say that a town's size doubles every 10 years (which by the rule of 70 corresponds to a 7% growth rate, incidentally). Starting in the year 1900 at 100 residents, we expect town population to be 200 in 1910, 400 in 1920, 800 in 1930, eventually climbing to over 100,000 by the year 2000 (see [](#table:expgrowth:popgrowth)). Unabated 7% growth would result in the town reaching the current world population just 260 years after the experiment began.

But let's explore an example that often reveals our faulty intuition around exponential growth. Here, we imagine a jar rich in resources, seeded with just the right number of bacteria so that if each bacterium splits every 10 minutes, the jar will become full of bacteria in exactly 24 hours. The experiment starts right at midnight. The question is: at what time will the jar be half full?

Think about this on your own for a minute. Normal intuition might suggest a half-full jar at noon halfway along the experiment. But what happens if we work backwards? The jar is full at midnight, and doubles every ten minutes. So what time is it half full?

The answer is one doubling-time before midnight, or 11:50 PM. [](#fig:expgrowth:bacteriajar) illustrates the story. At 11 PM, the jar is at one-64th capacity, or 1.7% full. So, for the first 23 of 24 hours, the jar looks basically empty. All the action happens at the end, in dramatic fashion.

```{table} Example 7% growth progression.
:label: table:expgrowth:popgrowth
:align: center
| Year | Population |
| :----: | ----------: |
| 1900 | 100        |
| 1910 | 200        |
| 1920 | 400        |
| 1930 | 800        |
| 1940 | 1 600      |
| :    | :          |
| 2000 | 102 400    |
```

10 minutes is perhaps a little fast for biology, but we're looking for easy understanding and picking convenient numbers. In practice, 20-30 minutes may be more realistic. We will also ignore deaths for this "toy" example, although the net effect only changes the rate and not the overall behavior.
```{figure} ../figures/Ch01_ExponentialGrowth/BacteriaJar.svg
:label: fig:expgrowth:bacteriajar
:align: center
:width: 100%
:alt: The last 90 minutes in the sequence of bacteria (green) growing in a jar, doubling every 10 minutes. For the first 22.5 hours, hardly anything would be visible. Note that the upward rise of green "bars" makes an exponential curve.
The last 90 minutes in the sequence of bacteria (green) growing in a jar, doubling every 10 minutes. For the first 22.5 hours, hardly anything would be visible. Note that the upward rise of green "bars" makes an exponential curve.
```

Now let's imagine another illustrative scenario in connection with our jar of bacteria. The time is 11:30 PM: one-half hour before the end. The jar is one-eighth full. A thoughtful member of the culture projects the future and decides that more uninhabited resource-laden jars must be discovered in short order if the culture is to continue its trajectory. Imagine for a second the disbelief expressed by probably the vast majority of other inhabitants: the jar is far from full, and has served for 141 generations - a seeming eternity. Nonetheless, this explorer returns reporting three other equal-sized food-filled jars within easy reach. A hero's welcome! How much longer will the culture be able to continue growing? What's your answer?

The population doubles every ten minutes. If the original jar is filled at 12:00, the population doubles to fill the second jar by 12:10. Another doubling fills all four by 12:20. The celebration is short-lived.

Now we draw the inevitable parallels. A planet that has served us for countless generations, and has seemed effectively infinite - imponderably large - makes it difficult for us to conceive of hitting limits. Are we half-full now? One-fourth? One-eighth? All three options are scary, to different degrees. At a 2% rate of growth (in resource use), the doubling time is 35 years, and we only have about a century, even if at 1/8 full right now.[^3]

In relation to the bacteria parable, we've already done a fair bit of exploring. We have no more jars. One planet rhymes with jars, but it is hostile to human life, has no food, and is not within easy reach. We have no meaningful outlet.[^4] And even if we ignore the practical hardships, how much time would a second planet buy us anyway for uninterrupted growth? Another 35 years?

# Exponential Math

```{hint} Advice on Reading Math

This section is among the most mathematically sophisticated in the book. Don't let it intimidate you: just calmly take it in. Realize that exponential growth obeys an unchanging set of rules, and can be covered in just a few pages. Your brain can absorb it all if you give it a chance. Read paragraphs multiple times and find that each pass can add to your comprehension. Equations are just shorthand sentences[^5] capturing the essence of the concepts being covered, so rather than reading them as algorithms to file and use later when solving problems, work to comprehend the meaning behind each one and its reason for being a part of the development. In this way, what follows is not a disorganized jumble, recklessly bouncing between math and words, but one continuous development of thought expressed in two languages at once. The Preface offers additional thoughts related to this theme, and the appendix [](#app:matheq) provides a math refresher.
```

The essential feature of exponential growth is that the scale goes as the power of some base (just some number) raised to the time interval. In the doubling sequence, we start at 1x the original scale, then go to 2x, then 4x, then 8x, etc. At each time interval, we multiply by 2 (the base). After 5 such intervals, for instance, we have $2\times 2\times 2\times 2\times 2 = 2^5 = 32$. More generally, after $n$ doubling times, we have increased by a factor of $2^n$, where $2$ is the base, and $n$ is the number of doubling times. We might formalize this as

$$
\label{eq:expgrowth:M}
M = 2^n = 2^{t/t_2},
$$

[^3]: If we're at 1/8 right now and double every 35 years, we will be at 1/4 in 35 years, 1/2 in 70 years, and full in 105 years.

[^4]: [](#chap:spacecolonization) addresses space realities.

[^5]: Unlike words/language, the symbols chosen for equations are just labels and carry no intrinsic meaning, so electing to use $x, n, t, b, M$, etc. reflect arbitrary choices and can be substituted at will, if done consistently. The content is in the structure of the equation/sentence.

where $M$ represents the multiplicative scale, $t$ is the elapsed time, and $t_2$ is the symbol we choose to represent the doubling time - so that $n = t/t_2$ is just "counting" the number of doubling times.

For instance, doubling has $M = 2$, tripling has $M = 3$, and increasing by 29% would mean $M = 1.29$.

```{exercise} Interest Example
:label: ex:expgrowth:interest
A bank account accumulates interest in the same way as described above. Consider an account that you deposit \$100, and the account accrues interest at 2\% annually. If no other money is added to the account, what is the balance after
* 1 year?
* 2 years?
* 3 years?
* 35 years?
```
```{solution} ex:expgrowth:interest
:label: soln:expgrowth:interest
:class: dropdown
The same multiplicative process happens in a bank account accumulating interest. Let's consider that you deposit \$100 into a bank account bearing 2\% annual interest. At the end of one year, you'll have \$102, which is 1.02 times the original amount. For the next year, it is 1.02 times \$102, or \$104.04, which is the original \$100 times $1.02 \times 1.02$. Then in three years it will be \$106.18, or \$100 times $1.02\times 1.02\times 1.02=1.02^3$. Having sussed out the pattern, after 35 years it would be $\$100 \times 1.02^{35}$, which happens to come to \$199.99. Notice that doubling in 35 years at 2\% exactly obeys the rule of 70.

| year | b^n    | dollars |
| ---: | ----: | :------: |
| 0    | 1.00   | $100.00 |
| 1    | 1.02   | $102.00 |
| 2    | 1.0404 | $104.04 |
| 3    | 1.0612 | $106.12 |
| :    | :      | :       |
| 10   | 1.2190 | $121.90 |
| :    | :      | :       |
| :    | :      | :       |
| 35   | 1.9999 | $199.99 |
```

The pattern whether doubling, or applying interest as in [](#ex:expgrowth:interest) is that we multiply a chain of the same number, the base, over and over. This is the same as raising the base to some power - the power equaling how many times the base appears in the chain to get our overall factor. Therefore, if we designate the base as $b$ and the number of times it appears as $n$, we have

$$
\label{eq:expgrowth:baseton}
M = b^n.
$$

Now we are going to play a math trick[^6] that will help us compute various useful attributes of growth. The exponential and natural logarithm are inverse functions, each undoing the other. So $\ln (e^x) = x$ and $e^{\ln~x} = x$. We can use this trick to express the number $2$ as $e^{\ln~2}$, or any base number $b = e^{\ln~b}$. For the special case of $b = 2$ (doubling), we then have:

$$
\label{eq:expgrowth:doubling}
M = 2^{t/t_2} = (e^{\ln 2})^{t/t_2} = e^{t \ln 2/t_2},
$$

where we started with Eq. {eq}`eq:expgrowth:doubling`, re-expressed the number $2$, and then applied the rule that raising a power to another power is the same as multiplying the powers to form a single one. By employing such tricks, we could cast any base to a power, like $b^x$ as some exponential function $e^{x \ln~b}$, and thus can transform any "power" relationship into an exponential using base $e\approx 2.7183$. Casting Eq. {eq}`eq:expgrowth:baseton` in this form:

$$
\label{eq:expgrowth:Mbn}
M = b^n = e^{n \ln b}.
$$

If we want to go backwards, and compute the time to reach a certain $M$ factor, we can take the natural logarithm of both sides to learn that

$$
\label{eq:expgrowth:logM}
\ln M = n \ln b,
$$

so that the number of applications of base, $b$, needed to achieve multiplicative factor $M$ is found by solving Eq. {eq}`eq:expgrowth:logM` for $n$, in which case we get: $n = \ln M/\ln b$.


[^6]: By trick, we do not mean to imply anything devious or untoward: just a cute manipulation that can bring additional insight or make something easier.

```{exercise} Try It!
:label: ex:expgrowth:tryb
Try it on a calculator for several examples of $b$ that you concoct (make it real for yourself!).
```
```{solution} ex:expgrowth:tryb
:label: soln:expgrowth:tryb
:class: dropdown
If I choose $b=5$ and plug $e^{\ln~5}$ into my calculator, I get $5$.
```

```{exercise} Powers of Powers
:label: ex:expgrowth:powerpower
Consider 
$$\left( 5^3\right)^4$$
* Write this as a sequence of multiplications of $5$.
* How many fives are you multiplying? Write this as a single five with an exponent.
* Use a calculator to compare the two values above.
```
```{solution} ex:expgrowth:powerpower
:label: soln:expgrowth:powerpower
:class: dropdown
* We get four multiplications of $5\times 5\times 5$.
$$\left( 5^3\right)^4=\left(5\times 5\times 5\right)\cdot\left(5\times 5\times 5\right)\cdot\left(5\times 5\times 5\right)\cdot\left(5\times 5\times 5\right)= $$

* This is twelve multiplications of five or $5^{12}$. 
* The result of both is $244 140 625$.

So we effectively just multiplied the two exponents 3 and 4 to get the 12. It always works. Often, one need not memorize math rules: quick experimentation reveals how and why it works.
```

```{tip} Example
The time it would take to increase by a factor of $1 000$ ($M = 1000$) at a rate of $1.07$ (annual growth rate of $7\%$; $b = 1.07$) is 

$$n &= \frac{\ln M}{\ln b}\\
n &= \frac{\ln 1000}{\ln 1.07}\\
n &= \frac{6.908}{0.068}\\
n &= 102~{\rm years}
$$
```

The rule of 70 can be recovered[^7] by setting the multiplicative factor, $M$, to 2. Comparing to interest accumulation described by $(1 + p)^t$, where $p$ is the annual interest (0.02 for 2%, e.g.) and $t$ is the number of years, Eq. {eq}`eq:expgrowth:Mbn` can be re-expressed by substituting $b = 1 + p$ and $n = t$ as the number of years, then equating the result to the doubling time representation in Eq. {eq}`eq:expgrowth:doubling` to form

$$
\label{eq:expgrowth:etoln}
M = e^{t \ln(1+p)} = e^{t \ln 2/t_2}.
$$

From this expression, we can gather that $\ln(1 + p) = \ln 2/t_2$ by equating the exponents, and then see that the doubling time, $t_2$, can be solved as

$$
\label{eq:expgrowth:t2}
t_2 = \ln 2/\ln(1+ p).
$$

For small values of $p$ (much smaller than 1), the natural log of $1 + p$ is approximately $p$. In other words, when $p = 0.02$, $\ln 1.02 \approx 0.02\approx p$. This is part of the reason why we chose $e$ as our base, as it is mathematically "natural." Since $\ln 2 \approx 0.693\approx 0.70$, the doubling time, $t_2$, is approximately 70 divided by the annual growth rate, $p$, in percent. So the reason it's a rule of 70 for doubling (and not a rule of 60 or 80) is basically because the natural log of 2 (representing doubling) is roughly 0.70. 

```{tip} Example
To tie some things together, let's look at a quantitative case that can be used to validate how various pieces relate to each other. We will describe a 5% annual growth rate.

The rule of 70 indicates a 14 year doubling time, so that we could define $t_2$ appearing in Eqs. {eq}`eq:expgrowth:M`, {eq}`eq:expgrowth:doubling`, {eq}`eq:expgrowth:etoln`, and {eq}`eq:expgrowth:t2` to be 14 years. Calculating exactly using Eq. {eq}`eq:expgrowth:t2` yields 14.2 years.

To evaluate growth in 10 years, we could use Eq. {eq}`eq:expgrowth:M` with $t = 10$ and $t_2 = 14.2$ to suggest $M = 1.63$, meaning a 63% increase in size (1.63 times as large as at the start). Or we could apply Eq. {eq}`eq:expgrowth:baseton` using $b = 1.05$ and $n = 10$ to get the exact same result. Note that we have freedom to define the base as 1.05 or 2, and the corresponding number of steps ($n$) as 10 or $t/t_2 = 0.704$, respectively, and get the same answer. In terms of the exponential form in Eq. {eq}`eq:expgrowth:Mbn`, either pair of $b$ and $n$ produces $e^{0.488}$.

If we wanted to work backwards and ask when the amount is 3 times the original ($M = 3$), we could use Eq. {eq}`eq:expgrowth:logM` to find that $n$ is 22.5 steps at $b = 1.05$ (thus 22.5 years, since this base is the yearly increase). Had we used $b = 2$, we would compute $n = 1.58$, meaning that the scale would reach 3x after 1.58 doubling times, or $1.58t_2 = 22.5$ years.

We can check the result using Eq. {eq}`eq:expgrowth:etoln` by putting in $t = 22.5$ and $p = 0.05$ or $t_2 = 14.2$ in the latter form.
```

The same result happens if using $log_{10}$ instead of $\ln$: try it!

[^7]: What follows is a high-brow symbolic approach, but the same effective result can be achieved by setting $M = 2$ in Eq. {eq}`eq:expgrowth:logM` and solving for $n$.

Don't view this as a recipe for solving problems but as a way to romp through the section and help piece it together.

More generally, we are not confined to any particular base, $b$, having just seized upon two convenient and relevant possibil- ities. If we wanted $b = 10$, we would have $n = 0.211$, for example. In this case, the interpretation is that our ten-year point is 21.1% of the way to a factor-of-ten multiplication, so that 47.4 years at 5% growth results in a factor of 10 growth.

(sec:expgrowth:expenergyextrap)=
# Exponential Energy Extrapolation

Having established some basic principles of exponential growth, it's time for a first look at how we can use the math to argue about limits to our expectations. We'll concentrate on energy use. The United States Energy Information Administration (EIA) provides information on energy use from 1949 to the present. An appendix (E1: [@USEIA]) presents an approximate
account of energy use from 1635-1945. [](#fig:expgrowth:energyproduction) displays this full range of history.
```{figure} ../figures/Ch01_ExponentialGrowth/EnergyProduction.png
:label: fig:expgrowth:energyproduction
:align: center
:width: 100%
:alt: U.S. energy over almost 400 years, showing a dramatic rise due almost entirely to fossil fuels. The red curve is an exponential fit.
U.S. energy over almost 400 years, showing a dramatic rise due almost entirely to fossil fuels. The red curve is an exponential fit.
```

We use U.S. data simply to illustrate the more broadly applicable global growth trend. Even countries far behind the U.S. show growing energy use often faster than the 2-3% charac-
teristic of U.S. history. To explore worldwide data over more recent years, select various countries in the Gapminder interactive in [](#interact:expgrowth:gapmind). You may need to expand the interactive to have the full range of selections.
:::{iframe}//www.gapminder.org/tools/?embedded=true#$model$markers$bubble$encoding$y$data$concept=energy_use_per_person&source=sg&space@=geo&=time;;&scale$domain:null&zoomed:null&type:null;;&x$data$concept=time&space@=time;;&scale$domain:null&zoomed:null&type:null;;&frame$speed:1200&value=2015;&trail$data$filter$markers$usa=1960;;;;;;;;&chart-type=bubbles&url=v2
:label: interact:expgrowth:gapmind
:width: 100%
:align: center
:placeholder: ../figures/Ch01_ExponentialGrowth/gapminder.jpg
Gapminder: An interactive website for global data.
:::


Note that the energy rate at the left edge of [](#fig:expgrowth:energyproduction) becomes almost invisibly small. Presenting the data on a logarithmic plot, as in [](#fig:expgrowth:energyproductionlog), we can better see the entire trajectory. On such a plot, exponentials become straight lines. The trend is remarkably consistent with an exponential (red line) for most of the history, at a rate of about 2% per year. Note that this total effect includes population growth, but population has not grown as fast as energy, so that per-capita energy has also risen. This makes sense: our lives today are vastly more energetically rich than lives of yesteryear, on a per-person basis.

The astute reader might note a departure from the exponential fit in past years. This only reinforces the primary point of this chapter that sustaining exponential growth indefinitely is absurd and will not happen. If growth is destined to stop, perhaps we are beginning to experience its limits well before the theoretical timescales developed in this chapter.

Having established that energy growth over the past several is well-described by an exponential, we can explore the implications of continuing this trend forward. Present-day global energy production rate is approximately $18\times 10^{12}$ Watts (18 TW). Watts is a unit of power, which is a rate of energy. [](#chap:energyandpower) will cover the units more thoroughly. We adopt a convenient growth rate of 2.3% per year for this exercise. We pick this for two reasons: 
1. It is in agreement with the historical trend, so will not over-exaggerate the
2. This rate produces the mathematical convenience of a factor of 10 increase every century.[^8]
```{figure} ../figures/Ch01_ExponentialGrowth/EnergyProductionLog.png
:label: fig:expgrowth:energyproductionlog
:align: center
:width: 100%
:alt: Energy trajectory in the U.S. over almost 400 years. The red line is an exponential fit at a 2% growth rate, which appears linear
on a logarithmic plot.
Energy trajectory in the U.S. over almost 400 years. The red line is an exponential fit at a 2% growth rate, which appears linear
on a logarithmic plot.
```

What follows is a flight of fancy that quickly becomes absurd, but we will chase it to staggering levels of absurdity just because it is fun, instructive, and mind-blowing. Bear in mind that what follows should not be taken as predictions[^9] of our future: rather, we can use the absurdity to predict how our future *will not* look!

The sun deposits energy at Earth's surface at a rate of about 1000 W/m<sup>2</sup> (1000 Watts per square meter; we'll reach a better understanding for
these units in [](#chap:energypower)). Ignoring clouds, the projected area intercepting the sun's rays is just $A = \pi R_{\oplus}^2$, where $R_{\oplus}$ is the radius of the earth, around 6400 km. Roughly a quarter of the earth's surface is land, and adding it all up we get about $30\times 10^{15}$ W hitting land. Approximate numbers are perfectly fine for this exercise. If we put solar panels on every square meter of land converting sunlight to electrical energy at 20% efficiency,[^10] we keep $6\times 10^{15}$ W. This is a little over 300 times the current global energy usage rate of 18 TW. What an encouraging number! Lots of margin. How long before our growth would get us here? After one century, we're 10 times higher, and 100 times higher after two centuries. It would take about 2.5 centuries (250 years) to hit this limit. Then no more energy growth. The merits of various alternative energy sources will be treated in later chapters, so do not use this chapter to form opinions on the usefulness of solar power, for instance.

But wait, why not also float panels on all of the ocean, and also magically improve performance to 100%? Doing this, we can capture a whopping $130\times 10^{15}$ W, over 7000 times our current energy consumption rate. Now we're talking about maxing out in just under 400 years. Each factor of ten is a century, so a factor of 10000 would be four factors of ten ($10^4$), taking four centuries.

So within 400 years, we would be at the point of using every scrap of solar energy hitting the planet at 100% efficiency. But our planet is a tiny speck in space. Why not capture *all* the light put out by the sun, in a sphere surrounding the sun (called a Dyson sphere; see [](#box:expgrowth:dyson))? Now we're talking some real power! The sun puts out $4\times 10^{26}$ W. If it were a light bulb, this would be its label (putting the 100 W standard incandescent bulb to shame). So the number is enormous. But the math is actually pretty easy to grasp.[^11] Every century gets another factor of ten. To go from where we are now ($18\times 10^{12}$ W) to the solar regime is about 14 orders-of-magnitude. So in 1400 years,[^12] we would be at $18\times 10^{26}$ W, which is about 4.5 times the solar output. Therefore we would use the entire sun's output in a time shorter than the 2000-year run of our current calendar.

[^8]: Fundamentally, this relates to the fact that the natural log of 10 is 2.30. The analog of Eq. {eq}`eq:expgrowth:t2` using 10 in place of 2 and $p = 0.023$ for 2.3% growth rate will produce a factor-of-ten timescale $t_{10}\approx 100$ years.
[^9]: Do not interpret this section as pre-dictions of how our future *will* go.
[^10]: 20% is on the higher end for typical solar panels.

```{hint} Dyson Sphere Construction
:label: box:expgrowth:dyson

If we took the material comprising the entire Earth (or Venus) and created a sphere around the sun at the current Earth-Sun distance, it would be a shell less than 4 mm thick! And it's not necessarily ideal material stock for building a high-tech sphere and solar panels. The earth's atmosphere distributed over this area would be 0.015 m thick. Don't hold your breath waiting for this to happen.
```
Bypassing boring realism, we recognize that our sun is not the only star in the Milky Way galaxy. In fact, we estimate our galaxy to contain roughly 100 billion stars! This seems infinite. A billion seconds is just over 30 years, so no one could count to 100 billion in a lifetime. But let's see: 100 billion is 10<sup>11</sup>. Immediately, we see that we buy another 11 centuries at our 2.3% rate. So it takes 1,100 years to go from consuming our entire sun to all the stars in our galaxy! That's 2,500 years from now, adding the two timescales, and still a civilization-relevant time period. Leave aside the pesky fact that the scale of our galaxy is 100,000 light years, so that we can't possibly *get* to all the stars within a 2,500 year timeframe. So even as a mathematical exercise, physics places yet another limit on how long we could conceivably expect to maintain our current energy growth trajectory.

The unhinged game can continue, pretending we could capture all the light put out by all the stars in all the galaxies in the visible universe. Because the visible universe contains about 100 billion galaxies, we buy another 1,100 years. We can go even further, imagining converting all matter (stars, gas, dust) into pure energy ($E = mc^2$), not limiting ourselves to only the light output from stars as we have so far. Even playing these unhinged games, we would exhaust all the matter in the visible universe within 5,000 years at a 2.3% rate. The exponential is a cruel beast. [](#table:expgrowth:energytimescales) summarizes the results. By coincidence, the visible universe has about as many galaxies as our galaxy has stars. By "visible" universe, we mean everything within 13.8 billion light years, which is as far as light has been able to travel since the Big Bang (see [](#sec:appDtangents:universeedge)).

The point is not to take seriously the timescales for conquering the sun or the galaxy. But the very absurdity of the exercise serves to emphasize the impossibility of our continuing exponential growth in energy. All kinds of reasons will preclude continued energy growth, including the fact that human population cannot continue indefinite growth on this planet. We will address space colonization fantasies in [Chapter 4](#chap:spacecolonization).

[^11]: Math becomes easier if you blur your vision a bit and do not demand lots of precision. In this case, we essentially ignore everything but the exponent, recognizing that each century will increment it by 1, at our chosen 2.3% rate.

[^12]: In this case, the "real" answer would be 1,335 years, but why fret over the details for little gain or qualitative difference in the outcome?


```{table} Energy limit timescales.
:label: table:expgrowth:energytimescales
:align: center
| Utilizing          | years until |
| ------------------ | -----------: |
| Solar, land, 20%   | 250         |
| Solar, earth, 100% | 390         |
| Entire Sun         | 1400       |
| Entire Galaxy      | 2500       |
| Light in Universe  | 3600       |
| Mass in Universe   | 5000       |
```

# Thermodynamic Consequences

Physics places another relevant constraint on growth rate, and that concerns waste heat. Essentially all of our energy expenditures end up as heat. Obviously many of our activities directly involve the production of heat: ovens, stoves, toasters, heaters, clothes dryers, etc. But even cooling devices are net heat generators. Anything that uses power from an electrical outlet ends up creating net heat in the environment, with very few exceptions. A car moving down the road gets you from place A to place B, but has stirred the air,[^13] heated the engine and surrounding air, and deposited heat into the brake pads and rotors, tires and road. Our metabolic energy mostly goes to maintaining body temperature. But even our own physical activity tends to end up as heat in the environment. The only exceptions would be beaming energy out of the earth environment (e.g., light or radio) or putting energy into storage (eventually to be converted to heat). But such exceptions do not amount to much, quantitatively.

Some time, go feel the exhaust air from an air-conditioning unit, or the heat produced at the back and bottom of a refrigerator. Even though these devices perform a cooling function, they make more heat than cool.

[^13]: Stirred-up air eventually grinds to a halt due to viscosity/friction, becoming heat.

What happens to all of this waste heat? If it all stayed on Earth, the temperature would climb and climb. But the heat does have an escape path: infrared radiation[^14] to space. The earth is in an approximate thermodynamic equilibrium: solar energy is deposited, and infrared radiation balances the input to result in steady net energy. As we will see in [Chapter 5](#chap:energypower), the rate at which energy flows is called power, so that we can describe energy flows into and out of the earth system in terms of power. Physics has a well-defined and simple rule for how much power a body radiates, called the Stefan-Boltzmann law:[^15]

[^14]: ... a form of electromagnetic radiation

[^15]: ... leaving out something called *emissivity*, not relevant for our purposes

$$
\label{eq:expgrowth:stefan}
P = A_{surf} \sigma \left(T_{hot}^4 - T_{cold}^4\right).
$$

$P$ is the power radiated, $A_{surf}$ is the surface area, $T_{hot}$ is the temperature of the radiating object in Kelvin[^16] (very important!), $T_{cold}$ is the temperature of the environment (also Kelvin), and $\sigma$ is the Stefan-Boltzmann constant: $\sigma = 5.67 \times 10{-8}~{\rm W/m^2/K^4}$.[^17] Note that the law operates on the difference of the fourth powers of two temperatures.

```{exercise} Radiation Example
:label: ex:expgrowth:blackbody
A table in a room in which the table and walls are all at the same temperature does not experience net radiation flow since the two temperatures to the fourth power subtract to equal zero. In this case, as much radiation leaves the table for the walls as arrives from the walls to the table. But a room-temperature object at 300 K radiates approximately 450 W per square meter to the coldness of space. Show this is true by calculating Eq. {eq}`eq:expgrowth:stefan` with $T_{hot}=300~{\rm K}$ and $T_{cold}=0~{\rm K}$. Let $A_{surf} = 1~{\rm m^2}$.
```
```{solution} ex:expgrowth:blackbody
:label: ex:expgrowth:blackbodysoln
:class: dropdown
$$
P &= A_{surf} \sigma \left(T_{hot}^4 - T_{cold}^4\right)\\
\\
P &= 1 \times 5.67\times 10^{-8} \left(300^4 - 0^4\right)\\
\\
P &= 5.67\times 10^{-8} \left(8.1\times 10^9\right)\\
\\
P &= 459.27~{\rm W}
$$
```
[^16]: Conversions to Kelvin from Celsius (or Fahrenheit) go like:
$T(K) = T(C) + 273.15$;
$T(C) = (T(F) - 32) / 1.8$

[^17]: It's actually an easy constant to remember: 5-6-7-8 (but must remember the minus sign on the exponent).

Because space is so cold (tens of Kelvin, effectively, unless exposed to the sun), the fourth power of such a small number pales so *much* in comparison to the fourth power of a number like 300 that we can safely ignore it for radiation to space:

$$
\label{eq:expgrowth:stefansimple}
P_{space} \approx A_{surf}\sigma T^{4},
$$

where we now just have a single temperature: that of the warm body in space.

Earth reaches an equilibrium so that power-in equals power-out.[^18] If more power is dumped onto the planet, then the temperature rises until $\sigma T^{4}$ climbs to match. The relation in Eq. {eq}`eq:expgrowth:stefansimple` is fundamentally important to Earth's temperature balance, and applies pretty universally, as highlighted in [](#box:expgrowth:everthingradiates).

```{hint} Everything Radiates
:label: box:expgrowth:everthingradiates
The same relation (Eq. {eq}`eq:expgrowth:stefan`) governs the surface of the sun, light bulb filaments, glowing coals, and even the human body. While the human body expends metabolic energy at a similar rate to an incandescent light bulb (about 100 W), one is *much* hotter than the other because the surface areas are vastly different.
```
```{figure} ../figures/Ch01_ExponentialGrowth/EarthAbsorbsSun.jpeg
:label: fig:expgrowth:sunonearth
:width: 100%
:align: center
:alt: Earth-shown here in northern hemisphere summer-intercepts sunlight across the projected area of the Earth's disk ($\pi R^2$), while radiating from the entire surface area, which is four times larger ($4\pi R^2$).
Earth-shown here in northern hemisphere summer-intercepts sunlight across the projected area of the Earth's disk ($\pi R^2$), while radiating from the entire surface area, which is four times larger ($4\pi R^2$).
```

To evaluate the expected temperature of the earth, we know that the sun delivers 1360 W/m<sup>2</sup> to the *top* of the earth's atmosphere ([](doi:10.1029/2010GL045777)) (a bit less reaches the ground). This 1360 W/m<sup>2</sup>, known as the solar constant, is the incident energy rate (power), or the *flux*, of sunlight incident on Earth. We also know that about 29.3% of this is reflected by clouds, snow, and to a lesser extent water and terrain. So the earth system *absorbs* about 960 W/m<sup>2</sup>. It absorbs this energy onto the area facing the sun: a projected disk of area $A_{proj} = \pi R_{\bigoplus}^{2}$. But the total surface area of the earth is four times this (the surface area of a sphere is $4\pi R^2$), all of it participating in the radiation to space ([](#fig:expgrowth:sunonearth). Equating the input and output for equilibrium conditions:

$$
\label{eq:expgrowth:earthP}
P_{in} = 0.707 \times 1360 \text{ W/m}^2 \times \pi R_{\bigoplus}^{2} = P_{out} = 4\pi R_{\bigoplus}^{2}\sigma T^{4},
$$
The 0.707 factor represents absorbed fraction after 29.3% is reflected. We can rearrange to isolate temperature, satisfying
$$
\label{eq:expgrowth:earthstefan}
T^{4} = \frac{0.707 \times 1360 \text{ W/m}^2}{4\sigma}
$$

[^18]: Climate change is due to greenhouse gases blocking the escape of some radiation to space, presently causing a ~0.1% imbalance that [Chapter 9](#chap:climatechange) will address.

Solving for $T$ yields $T=255~{\rm K}$, or -18°C (about 0°F). This is cold - too cold. We observe the average temperature of Earth to be about 288 K, or 15°C (59°F). The difference of 33°C is due to greenhouse gases - mostly H<sub>2</sub>O - impacting the thermal balance by preventing most radiation from escaping directly to space. We'll cover this more extensively in [Chapter 9](#chap:climatechange).

Armed with Eq. {eq}`eq:expgrowth:earthstefan`, we can now estimate the impact of waste heat on Earth's equilibrium temperature. Using the solar input as a baseline, we can add increasing input using the exponential scheme from the previous section: starting today at 18 TW and increasing at 2.3% per year (a factor of 10 each century). It is useful to express the human input in the same terms as the solar input so that we can just add to the numerator in Eq. {eq}`eq:expgrowth:earthstefan`. In this context, our current 18 TW into the projected area $\pi R^2$ adds 0.14 W/m<sup>2</sup> to the solar input (a trivial amount, today), but then increases by a factor of ten each century. Taking this in one-century chunks, the resulting temperatures - adding in the 33 K from greenhouse gases - follow the evolution shown in [](#table:expgrowth:DT). At first, the effect is unimportant, but in 300 years far outstrips global warming, and reaches boiling temperature in a little over 400 years! If we kept going (not possible), Earth's temperature would exceed the surface temperature of the sun inside of 1,000 years!
```{table} At a constant energy growth rate of 2.3% per year, the temperature climb from waste heat (not CO<sub>2</sub> emissions) is slow at first, but becomes preposterous within a few-hundred years. Water boils in just over 400 years, and by 900 years Earth is hotter than the sun! The scenario of continued growth is obviously absurd.
:label: table:expgrowth:DT
:align: center
| Years | Power Density (W/m<sup>2</sup>) | T (K) | ΔT (C) |
| -----: | --------------------: | -----: | ------: |
| 100   | 1.4                  | 288.1  | 0.1    |
| 200   | 14.0                 | 288.9  | ~1     |
| 300   | 140.0                | 296.9  | ~9     |
| 400   | 1400.0               | 344.0  | 56     |
| 417   | 2070.0               | 373.0  | 100    |
| 1000  | 1.4 x 10<sup>9</sup> | 8600.0 | 8300  |
```

A potential inconsistency in our treatment is that we based our exploration of energy scale on solar energy as a prelude to stellar energy capture. But in the thermodynamic treatment, we implicitly added our power source to the existing solar input. If the sun is the source, we should not double-count its contribution. Nonetheless, continued, relentless growth would eventually demand a departure from solar capture on Earth and drive the same thermodynamic challenges regardless. Synthesizing the messages: we can't continue 2.3% growth for more than a few centuries using sunlight on Earth. And if we invent something new and different to replace the fully-tapped solar potential, it too will reach thermodynamic limits within a few centuries.

Connecting some ideas, we found in the previous section that we would be consuming the sun's entire output in 1400 years at the 2.3% growth rate. It stands to reason that if we used a sun's worth of energy confined to the surface of the earth, the (smaller) surface would necessarily be hotter than the sun (in 1,400 years), just like a light bulb filament is hotter than human skin despite putting out the same power - owing to the difference in area.[^19]

One key aspect of this thermal radiation scenario is that it does not depend on the form of power source. It could in principle be fossil fuels, nuclear fission, nuclear fusion, or some form of energy we have not yet realized and may not even have named! Whatever it is, it will have to obey thermodynamics. Thus, thermodynamics puts a time limit on energy growth on this planet.

[^19]: This can be gleaned from Eq. {eq}`eq:expgrowth:stefan` or Eq. {eq}`eq:expgrowth:stefansimple`.

# Upshot: Physics Limits Physical Growth

We saw in this chapter that unabated growth leads to absurd results. First, we calibrated our intuition in the context of bacteria in jars. The key point is that the jar is half full one doubling time before it is full. While this seems obvious, it delays the drama to the very end, acting fast to impose hard limits and catch the inhabitants by surprise. The conditions that persisted for many generations - thus taken for granted - suddenly change completely.

Next, we found that continuing a modest growth rate in energy becomes hopelessly absurd in a matter of centuries. Then we saw another side to this coin, in the context of thermal consequences on the surface of the earth if energy growth continues.

Was the exercise pointless, since the math leads to absurdity? Is the math wrong? No, it's immensely valuable to learn that our assumption of continued growth (and application of the corresponding correct math) fails to make sense, ultimately. The logical conclusion is that growth cannot continue indefinitely.

In the end, physics puts a timeline on expectations with respect to growth in energy on Earth. Maybe the ~300 year scale is not alarming enough. But it imposes a hard barrier against preserving our historical growth rate. In reality, other practicalities are likely to assert themselves before these hard limits are reached. We can therefore expect our growth phase to end well within a few hundred years. Given that the growth phase has lasted for far longer than that, we can say that we are closer to the end of the saga than to the beginning, yet the world is not collectively preparing for such a new reality. This seems unwise, and we will evaluate related concerns in subsequent chapters.

Note that a deviation from the assumed steady 2.3% growth rate changes all the numbers, and therein may lie the solution: ramp down growth!

Many factors will intercede to limit growth in both population and resource use: resource scarcity, pollution, aquifer depletion and water availability, climate change, warfare, fisheries collapse, a limited amount of arable land (declining due to desertification), deforestation, disease, to name a few. The point is only reinforced. By some means or another, we should view the present period of physical growth as a temporary phase: a brief episode in the longer human saga. A number of these issues will be addressed in subsequent chapters.

# Problems

Hint: for problems that require solving temperature when it appears as $T^4$, you'll need to take the fourth root, which is the same as raising to the 1/4 power. So use the $y^x$ button (or equivalent) and raise to the 0.25 power. You can check this technique by comparing the square root of a number to the result of raising that number to the 0.5 power. Another technique for the fourth root is to take the square root twice in a row.

1.  Verify the claim in the text that the town of 100 residents in 1900 reaches approximately 100,000 in the year 2000 if the doubling time is 10 years.
2.  Fill out [](#table:expgrowth:popgrowth) for the missing decades between 1940 and 2000.
3.  Our example town from the text starting at 100 people in the year 1900 and doubling every 10 years was said to take about 260 years (26 doubling times) to reach world population. Verify that the population indeed would approach 7 billion in 260 years (when the year would be 2160), by any means you wish.[^20]
4.  Use Eq. {eq}`eq:expgrowth:logM` with $b = 2$ to figure out exactly how many years - via a computation of doubling times, which may not be an integer - our example town from the text would take to reach 7 billion people.
	* Hint: $\ln$ is the natural log function found on scientific calculators (sometimes as LN).
	* Hint: $M$ is the ratio of the final population to the initial population.
5.  If our example town, which doubles every 10 years, reaches a population of 7 billion in 260 years, how many years before it reaches 14 billion?
6.  In a classic story, a king is asked to offer a payment as follows: place one grain of rice on one square of a chess board (64 squares), then two on the next square, four on the next, 8 on the next, and double the previous on each subsequent square. The king agrees, not comprehending exponential growth. But the final number (adding all the grains) is one less than 2<sup>64</sup>. How many grains is this? 
	* To get 2,000 kcal of metabolic content per day, a person would need to eat 30,000 grains of rice each day. The amount of rice computed for this problem would feed the current world population for 240 years, which you are encouraged to check for yourself!
7.  In the bacteria example of [%s](#sec:expgrowth:bacteria), how many doubling times are present in the 24 hour experiment (how many times did the population double)?
8.  A one-liter jar would hold about 10<sup>16</sup> bacteria. Based on the number of doubling times in our 24-hour experiment, show by calculation that our setup was woefully unrealistic: that even if we started with a single bacterium, we would have far more than 10<sup>16</sup> bacteria after 24 hours if doubling every 10 minutes.
9.  If a one-liter jar holds 10<sup>16</sup> bacteria, how many bacteria would we start in the jar so that the jar reaches full capacity after 24 hours if we increase the doubling time to a more modest/realistic 30 minutes?
	* Roughly 10 bacteria fit within a cubic micron (tiny), so you would not be able to see this tiny starting amount.
10. A more dramatic, if entirely unrealistic, version of the bacteria-jar story is having the population double every minute. Again, we start the jar with the right amount of bacteria so that the jar will be full 24 hours later, at midnight. At what time is the jar half full now?
11. In the more dramatic bacteria-jar scenario in which doubling happens every minute and reaches single-jar capacity at midnight, at what time will the colony have to cease expansion if an explorer finds three more equivalent jars in which they are allowed to expand without interruption/delay?
12. What is the doubling time associated with 3.5% annual growth?
13. Using Eq. {eq}`eq:expgrowth:logM` and showing work, what annual growth rate, in percent, leads to the mathematically convenient factor-of-ten growth every century?
	* Hint: the exponential, $e^x$, "undoes" the natural logarithm.
14. Use Eq. {eq}`eq:expgrowth:logM` with $b = 1 + p$ to figure out how long it takes to increase our energy by a factor of 10 if the growth rate is closer to the historical value of 2.9% ($p = 0.029$). Using 2.3% as we did in the chapter examples puts this at 100 years.[^21]
15. Extrapolating a constant growth rate in energy is motivated by historical performance. During this period, population was also growing, albeit not as fast. If population were to double every 50 years,[^22] how many people would Earth host when we hit the energy/thermodynamic limits in roughly 300 years?
	* We are unlikely to reach such a number for a host of other reasons.
16. In extrapolating a 2.3% growth rate in energy, we came to the absurd conclusion that we consume all the light from all the stars in the Milky Way galaxy within 2500 years. How much longer would it take to energetically conquer 100 more "nearby" galaxies, assuming they are identical to our own?
	* Ignoring the fact that it impossible to get to them fast enough, even at light speed.
17. In the spirit of outlandish extrapolations, if we carry forward a 2.3% growth rate (10x per century), how long would it take to go from our current 18 TW ($18\times 10^{12}~{\rm W}$) consumption to annihilating an entire earth-mass planet every year, converting its mass into pure energy using $E = mc^2$? Things to know: Earth's mass is $6\times 10^{24}~{\rm kg}$; $c = 3\times 10^8~{\rm m/s}$; the result is in Joules, and one Watt is one Joule per second.
	* Hint: Dividing the number of Joules asso- ciated with Earth's mass by the number of seconds in a year gives the number of Watts being consumed. You may wish to compare the result to the timescale before we would use the power output of all stars in the Milky Way galaxy?
18. Taking cues from the discussion of waste heat channels on page 10, describe some of the ways that all your energy output turns to heat when you go on a bicycle ride.
19. Your skin temperature is about 308 K, and the walls in a typical room are about 295 K. If you have about 1 m<sup>2</sup> of outward-facing surface area, how much power do you radiate as infrared radiation, in Watts? Compare this to the typical metabolic rate of 100 W.
	* Air convection also takes some heat away, but then clothing reduces both to bring us to equilibrium/comfort.
20. The moon absorbs 90% of the solar energy incident on it.[^23] How hot would you expect the surface to get under full sun? You don't need the factor of four here[^24] because the moon rotates very slowly under the sun and we're considering a patch experiencing overhead sunlight (rather than averaging over the sphere). Compare the result to boiling water temperature.
21. Venus is, ironically, colder than Earth as an infrared radiator. This is because Venus is covered in bright clouds, absorbing only 25% of the incident solar flux. Sunlight is more intense there due to it's being closer to the sun: it's almost double, at 2620 W/m<sup>2</sup>. Adapting Eq. {eq}`eq:expgrowth:earthstefan`, calculate the equilibrium temperature of Venus in the infrared and compare it to the Earth value of 255 K. The surface of Venus is much hotter than that of Earth owing to a runaway greenhouse condition. On Earth, the greenhouse boost is only 33 K, but on Venus it's hundreds of degrees.
22. Adapt Eq. {eq}`eq:expgrowth:earthstefan` to Mars to find its equilibrium temperature. The solar flux averages 590 W/m<sup>2</sup> there, and it absorbs 75% of incident sunlight. Express the answer in both Kelvin and Celsius, and put in context.
23. If a human body having an outward surface area of 1 m<sup>2</sup> continued to put out 100 W of metabolic power in the form of infrared radiation in the cold of space (naked; no sun), what would the equilibrium temperature be? Would this be comfortable (put in context)?
24. Verify the total solar power output of $4 \times 10^{26}~{\rm W}$ based on its surface temperature of 5800 K and radius of $7\times 10^{8}~{\rm m}$, using Eq. {eq}`eq:expgrowth:stefansimple`.
25. Verify that Earth would reach a temperature far in excess of boiling point of water[^25] after 500 years if today's power output (18 TW) increased by a factor of 10 each century.

[^20]: E.g., brute force doubling 26 times or using math to get straight at the answer.
[^21]: Hint: a good way to check your math. Note that if we were to use 2.9% instead of 2.3%, all of the time estimates in [%s](#sec:expgrowth:expenergyextrap) are reduced by the ratio of this question's answer to 100 years.
[^22]: This corresponds to a 1.4% growth rate, but you don't need to use this number in your calculation.
[^23]: ... incident at the same rate/flux as at Earth
[^24]: Referring to the 4 that shows up in Eqs. {eq}`eq:expgrowth:earthP` and {eq}`eq:expgrowth:earthstefan`.
[^25]: Water boils at 100°C, or 373 K.
