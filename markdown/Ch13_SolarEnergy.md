---
title: Chapter 13 - Solar Energy
banner: ../figures/Ch13_SolarEnergy/_page_0_Figure_0.jpeg
numbering:
  headings:
  heading_1:
    start: 14
kernelspec:
  name: python3
  display_name: 'Python 3'
---
(chap:solarenergy)= 
# Solar Energy

Now we come to the main attraction. As we saw in [Chapter](#page-183-0) [10,](#page-183-0) all of the strictly renewable energy options are ultimately derived from the sun. The two resources of the last two chapters—hydroelectricity and wind—represent tiny crumbs of the overall solar input to the planet.

Practically speaking, it is difficult to concoct ways to harness more than a few terawatts of power from hydroelectric or wind-based resources. Similar limitations apply to biologically-derived energy, geothermal, tidal, ocean currents, wave energy, etc. This may be worrisome considering that human society currently demands 18 TW. Meanwhile, the sun delivers 83,000 TW to the earth's surface (Fig. [10.1; p.167,](#page-186-0) [Table](#page-187-0) [10.2; p.168\)](#page-187-0). That's almost 5,000 times more than the demand. By the numbers, then, the sun seems to offer all we might ever need. In fact, the quantitative imbalance is so extreme as to make one wonder why we would ever mess around doing anything else.

Yet at present, the U.S. gets only about 0.9% of its energy from solar power, or 2.3% of its electricity. Similarly for the world, 1.2% of global energy is solar (2.1% of the electricity). It would seem to be vastly underutilized.

This chapter explains the nature of solar energy, its potential for use, practical considerations, and looks at the state of installations. While most of the focus is on [photovoltaic](#page-454-0) [\(PV\)](#page-454-0) panels that directly generate electricity from light, [solar thermal](#page-455-0) power generation is also covered.

# <span id="page-216-0"></span>**13.1 The Energy of Light**

[Sec.](#page-98-0) [5.10](#page-98-0) (p. [79\)](#page-98-0) introduced the basics of the energy of light. This section acts as a refresher and lays the foundation for the rest of the chapter.


Photovoltaic cells, showing grid contacts and crystal domains. Photo Credit: Tom Murphy

*<sup>©</sup> 2022 T. W. Murphy, Jr.; [Creative Commons Attribution-NonCommercial 4.0 International Lic.;](https://creativecommons.org/licenses/by-nc/4.0/) Freely available at: [https://escholarship.org/uc/energy\\_ambitions.](https://escholarship.org/uc/energy_ambitions)*

Light—a form of [electromagnetic radiation—](#page-445-0)is composed of [photons](#page-453-1)—individual particles of energy each having a characteristic [wavelength](#page-457-0)—what we might call color. Photons are such tiny quanta of energy that familiar environments are awash in unfathomably large numbers of them. A typical light bulb, for instance, emits quintillions<sup>1</sup> of photons every second.<span id="page-217-0"></span>**Definition 13.1.1** *The energy of a single photon, in various forms, is*
$$
E_{\text{photon}} = h\nu = \frac{hc}{\lambda} \approx \frac{2 \times 10^{-19} \text{ J}}{\lambda(\text{in } \mu\text{m})} = \frac{1.24 \text{ eV}}{\lambda(\text{in } \mu\text{m})},\tag{13.1}
$$

*where*  $h = 6.626 \times 10^{-34} \text{J} \cdot \text{s}$  *[\(Planck's constant\)](#page-453-2), and*  $\nu$  *is the [frequency](#page-447-0) of the light in [Hertz](#page-449-0) (Hz, or inverse seconds).*The second form  $(hc/\lambda)$  is useful, as we more commonly characterize the "color" of light by its [wavelength](#page-457-0),  $\lambda$ . The speed of light,  $c \approx 3 \times 10^8$  m/s, connects [frequency](#page-447-0) to wavelength via
$$
\lambda v = c. \tag{13.2}
$$

The third form in [Definition 13.1.1](#page-217-0) makes it easy to compute photon energy in Joules given the wavelength in [microns.](#page-451-0)<sup>2</sup> Visible light has a wavelength around 0.4–0.7  $\mu$ m (violet–to–red), so a typical photon energy, at 0.5  $\mu$ m, is about  $4 \times 10^{-19}$  J. It's a *tiny* number!**Example 13.1.1** About how many photons strike a 0.4 m<sup>2</sup> patch of sidewalk per second if the overhead sun is delivering 1,000 W/m<sup>2</sup> ?For the visible light characteristic of sunlight, we can use a convenient wavelength of 0.5  $\mu$ m, amounting to  $4 \times 10^{-19}$  J of energy per photon. The patch of sidewalk we describe receives light energy at a rate of 400 W or 400 J/s.[<sup>3</sup>](#page-10-3) How many  $4 \times 10^{-19}$  J photons does it take to amount to 400 J? Divide[<sup>4</sup>](#page-10-4) to get 10<sup>21</sup>.
[3](#page-10-3): . . . 0.4 m<sup>2</sup> times 1,000 W/m<sup>2</sup>
[4](#page-10-4): . . . or try reasoning it out: 10<sup>19</sup> of themThe final form in [Definition](#page-217-0) [13.1.1](#page-217-0) relates to the fact that photons frequently interact with electrons as we will see in [Section](#page-220-0) [13.3,](#page-220-0) making it convenient to convert to another energy unit called the [electron-volt,](#page-446-0) or [eV](#page-447-1) (introduced in Sec. [5.9; p.](#page-97-0) [78\)](#page-97-0). One electron volt is the energy it takes to move an [electron](#page-446-1) through an electric potential of one [Volt.](#page-457-1) The conversion is  $1 \text{ eV} = 1.602 \times 10^{-19} \text{ J}$ . For instance, the 0.5  $\mu$ m (blue-green) photon we used in the previous example would have an energy around 2.5 [eV.](#page-447-1)Why should we care about unthinkably small quantities of light? Three reasons come to mind:1. [Eq.](#page-217-1) [13.1](#page-217-1) elucidates that bluer <sup>5</sup> photons have higher energy than
red photons, which is important to know;
5: ... shorter wavelength<span id="page-217-1"></span>1: A quintillion is 10<sup>18</sup> of photons.2: One [micron,](#page-451-0) or micro-meter, abbreviated  $\mu$ m, is 10<sup>-6</sup> m.3: ... $0.4 m^2$  times  $1,000 W/m^2$ would make 4 J, so we need 100× more5: ...shorter wavelength

- 2. Individual photons interact with matter at the microscopic scale and are relevant to understanding solar photovoltaics and photosynthesis;
- 3. It's how nature really works.

## <span id="page-218-0"></span>**13.2 The Planck Spectrum**

We should first understand where photons originate, which will help us understand how solar panels work and their limitations. Until recent technological advances, [photons](#page-453-1) tended to come from *thermal* sources. It's true for the white-hot sun,<sup>6</sup> and true for flame and incandescent light which is just reflected sunlight bulb filaments.<sup>7</sup> Likewise, hot coals, electrical heating elements, and lava are all seen to glow. Physics tells us how such hot sources radiate, as covered by the next three equations. The first (with units) is:

$$
P = A\sigma T^{4} \text{ (W)}.
$$
 (13.3)

We already saw this equation in the context of Earth's energy balance in Sections [1.3](#page-29-0) and [9.2](#page-162-0). It is called the [Stefan–Boltzmann law,](#page-456-0) describing the total power (in W, or J/s) emitted from a surface whose area is  $A$  (in square meters) and temperature,  $T$  in Kelvin.<sup>8</sup> The constant,  $\sigma \approx 5.67 \times 10^{-8} \text{ W/m}^2/\text{K}^4$  is called the [Stefan–Boltzmann constant,](#page-456-1) and is easy to remember as 5-6-7-8.<sup>9</sup>  
9: The [Stefan–Boltzmann constant](#page-456-1) is actu-<span id="page-218-1"></span>
$$
B_{\lambda} = \frac{2\pi hc^2}{\lambda^5} \frac{1}{e^{hc/\lambda k_B T} - 1} \left(\frac{W/m^2}{m}\right),
$$
 (13.4)

[Eq. 13.4](#page-218-1) might look formidable, but only  $\lambda$  and  $T$  are variable. It describes the [Planck spectrum](#page-453-3), otherwise known as the [blackbody](#page-442-1)<sup>10</sup> spectrum. For some temperature,  $T$ , this function specifies how much power is emitted at each wavelength,  $\lambda$ . Three fundamental physical constants from key areas of physics make an appearance:  $c \approx 3 \times 10^8$  m/s is the familiar speed of light from relativity;  $h \approx 6.626 \times 10^{-34}$  J · s is [Planck's constant](#page-453-2) from quantum mechanics, and  $k_B \approx 1.38 \times 10^{-33}$  J · K is the [Boltzmann constant](#page-442-0) of thermodynamics.<sup>11</sup>
<sup>10</sup>: The term [blackbody](#page-442-1) effectively means a perfect emitter and absorber of thermal radiation.
<sup>11</sup>: This last one may be more familiar to<span id="page-218-2"></span>
$$
\lambda_{\text{max}} \approx \frac{2.898 \times 10^{-3}}{T(\text{in K})} (\text{m}).
$$

(13.5)

$$
\text{constant } R = k_B N_A \approx 8.31 \text{J/K/mol, where } N_{\text{A}} \approx 6.022 \times 10^{23} \text{ is Avogadro's number.}
$$

[Eq.](#page-218-2) [13.5](#page-218-2) is called the [Wien law](#page-457-2) and is a numerical solution identifying the peak of the [blackbody](#page-442-1) spectrum as a function of temperature. Higher temperatures mean higher kinetic energies at a microscopic scale, so that higher-energy (shorter-wavelength) photons can be produced. This is why as objects get hotter, they move from red to white, and eventually to a blue tint.

All this may seem overwhelming, but take a breath, then just look at [Figure](#page-219-0) [13.1.](#page-219-0) Everything so far in this section is captured by [Figure](#page-219-0) [13.1.](#page-219-0) 6: . . . and thus stars and even the moon,

<span id="page-218-3"></span>7: Modern lighting like fluorescent and LED sources rely on manipulating energy levels of electrons within atoms and crystals.

8: Recall that temperature in Kelvin is the temperature in Celsius plus 273 (273.15,

ally a witch's brew of more fundamental constants  $h$  [\(Planck's constant\)](#page-453-2),  $c$  (speed of light), and  $k_B$  (the [Boltzmann constant\)](#page-442-0) as  $\sigma = 2\pi^5 k_B^4/(15c^2h^3)$ .a perfect emitter and absorber of thermal radiation.

students in its chemistry form of the gas constant  $R = k_B N_A \approx 8.31 \text{ J/K/mol}$ , where*<sup>©</sup> 2022 T. W. Murphy, Jr.; [Creative Commons Attribution-NonCommercial 4.0 International Lic.;](https://creativecommons.org/licenses/by-nc/4.0/) Freely available at: [https://escholarship.org/uc/energy\\_ambitions.](https://escholarship.org/uc/energy_ambitions)*

<span id="page-219-0"></span>![](../figures/Ch13_SolarEnergy/_page_219_Figure_1.jpeg)

**Figure 13.1:** [Planck spectra,](#page-453-3) or [blackbody](#page-442-1) [spectra](#page-455-1) for three temperatures, indicating where the ultraviolet, visible, and infrared regions lie. The shapes of the three curves [\(spectra\)](#page-455-1) are described by [Eq.](#page-218-1) [13.4,](#page-218-1) the star locations are found by [Eq.13.5,](#page-218-2) and the total power radiated, per square meter of surface is the area under each curve, as captured in [Eq.](#page-218-3) [13.3.](#page-218-3) The dotted line relates to [Example](#page-219-1) [13.2.2.](#page-219-1) Note the 1e8 factor on the vertical axis, meaning that the axis goes from 0 to <sup>1</sup>.<sup>0</sup> <sup>×</sup> <sup>10</sup><sup>8</sup> <sup>W</sup>/m2/휇m.

The shape of each spectrum is a plot of the function in [Eq.](#page-218-1) [13.4](#page-218-1) for three different temperatures. If comparing output of [Eq.](#page-218-1) [13.4](#page-218-1) to [Figure](#page-219-0) [13.1,](#page-219-0) be aware that the units have been manipulated to favor [microns](#page-451-0) over meters.<sup>12</sup> 12: [Eq.](#page-218-1) [13.4](#page-218-1) uses units of meters for 휆, but

Let's come at this again with numbers to help us make sense of things. Looking at the curve (spectrum) for 6,000 K, we will verify that each equation makes some sense.

**Example 13.2.1** First, Eq. [13.5](#page-218-2) says that the wavelength where emission peaks should be about  $2.898 \times 10^{-3} / 6000 \approx 0.483 \times 10^{-6}$  m, or 0.483  $\mu$ m.Now look at the graph to see that the peak of the blue curve is indeed just short of 0.5 휇m, denoted by the red star at the top.

<span id="page-219-1"></span>**Example 13.2.2** Let's now verify a point on the [Planck spectrum,](#page-453-3) picking 6,000 K and 1 휇m to see if [Eq.](#page-218-1) [13.4](#page-218-1) lands in the same spot as indicated in [Figure](#page-219-0) [13.1.](#page-219-0)

If we go through the laborious exercise of plugging in numbers to [Eq.](#page-218-1) [13.4](#page-218-1) for  $T = 6000$  and  $\lambda = 1 \times 10^{-6}$  (1 µm), we find<sup>13</sup> the overall outcome is  $3.73 \times 10^{13}$  W/m<sup>2</sup> per *meter* of wavelength. Once we adjust by  $10^{-6}$  for the units on the plot (see earlier margin note), we expect  $0.373 \times 10^{8}$  W/m<sup>2</sup> per micron.Indeed, the blue curve passes through this value at a wavelength of 1 휇m, as indicated by the dotted line in [Figure](#page-219-0) [13.1.](#page-219-0)

[Figure](#page-219-0) [13.1](#page-219-0) uses [microns](#page-451-0) (휇m, or <sup>10</sup>−<sup>6</sup> m) for convenience. Also, [Eq.](#page-218-1) [13.4](#page-218-1) delivers an answer in units of W/m<sup>2</sup> per *meter* of wavelength, but for the plot we divided by 10<sup>6</sup> so it would be W/m<sup>2</sup> per *micron* of wavelength. By taking care of this detail, the area under each curve in [Figure](#page-219-0) [13.1](#page-219-0) should match <sup>휎</sup>푇 4 as in [Eq.](#page-218-3) [13.3.](#page-218-3)

(1  $\mu$ m), we find<sup>13</sup> the overall
of wavelength. Once we adjust
rlier margin note), we expect
<sup>13</sup>: Numerically, the numerator is 3.74  $\times$ 
10<sup>-16</sup>, the denominator is 10<sup>-30</sup>, and the
argument in the exponential is 2.4, so that
the second fraction is 0.1.**Example 13.2.3** Finally, to assess [Eq.](#page-218-3) [13.3,](#page-218-3) we can crudely estimate the area under the blue curve by drawing a rectangle that we think has about the same total area. We put the top of the rectangle at the top of the blue curve and ask how wide it would need to be to approximately match the area under the blue curve.

If we make it 0.5 휇m wide, it seems too thin: the area is smaller than what's under the blue curve. 1.0 휇m wide seems like too much area. So we pick something in the middle like 0.75 휇m [\(Figure](#page-220-1) [13.2\)](#page-220-1).

This choice makes the area about  $1.0 \times 10^8 \text{ W/m}^2/\mu\text{m}$  (value at the top of the rectangle) times  $0.75 \mu\text{m}$ , coming to  $7.5 \times 10^7 \text{ W/m}^2$ . Since this is power per area, we make a minor rearrangement of [Eq.](#page-218-3) [13.3](#page-218-3) to  $P/A = \sigma T^4$  and evaluate for  $T = 6000 \text{ K}$  to find  $7.35 \times 10^7 \text{ W/m}^2$ . Hey, not bad! So it all hangs together.Now that we've batted the equations around a little bit, like a cat might do if given a new mouse toy, let's absorb some key takeaways. First, as the source gets hotter, the area under the curve<sup>14</sup> increases *drastically*—as the *fourth-power* of 푇, according to [Eq.](#page-218-3) [13.3.](#page-218-3) This is seen in [Figure](#page-219-0) [13.1](#page-219-0) in that going from 3,000 K to 6,000 K<sup>15</sup> 15: . . . doubling temperature leads to a *tremendous* increase in area under the curve: 16 times, in fact.

Second, as an object gets hotter, it emits at shorter wavelengths, going from red-hot to yellow-hot to white-hot. The sun, at 5,800 K, peaks at 0.5 휇m, in the blue-green region. We don't see it as blue-green because it emits plenty of red light as well, making a *blend*. Notice how well the 6,000 K spectrum in [Figure](#page-219-0) [13.1](#page-219-0) covers the visible colors. A cooler star at 3,000 K has a red tint to it, since the 3,000 K spectrum [\(Figure](#page-220-2) [13.3\)](#page-220-2) shows a marked red-heavy tilt: blue is not as well represented as red is. Conversely, a hot star at 10,000 K will have a blue tint to it, since it peaks around 0.3휇m and has considerably more flux at the blue end of the spectrum than at the red end.

Finally, it is worth absorbing the overall lesson that photons from a glowing source emerge as a *distribution*, spanning a wide range of wavelengths (colors). This will turn out to be important in understanding why solar panels have the efficiencies that they do.

# <span id="page-220-0"></span>**13.3 Photovoltaics**

We are now prepared to dig into how [photovoltaic](#page-454-0) [\(PV\)](#page-454-0) panels actually work, and what governs panel efficiency.<sup>16</sup> 16: Solar thermal generation will be covered The word "photovoltaic" can be loosely read as: volts from photons, or electricity from light.

Various materials are used as the principal component in PV panels, but the vast majority are made of high-purity silicon, so we will speak in these terms alone. The basic physics will be the same for other materials as well. Getting too far into the weeds in describing the [semiconductor](#page-455-2)

<span id="page-220-1"></span>![](../figures/Ch13_SolarEnergy/_page_220_Figure_11.jpeg)

**Figure 13.2:** Attempts to crudely match the area under the 6000 K [Planck spectrum](#page-453-3) using rectangles of three different widths. The widest (1 휇m; dashed line) is too much area; the narrowest (0.5 휇m; dotted line) is too small. The middle (0.75 휇m; pink area) seems closest, by eye.

![](../figures/Ch13_SolarEnergy/_page_220_Figure_13.jpeg)

14: . . . total power emitted

<span id="page-220-2"></span>![](../figures/Ch13_SolarEnergy/_page_220_Figure_15.jpeg)

**Figure 13.3:** A 10,000 K star (or any [black](#page-442-1)[body\)](#page-442-1) has a spectrum that tilts blue in the visible spectrum, while a cooler star (object) at 3,000 K has a red slant. Spectra are normalized to the same peak for easier comparison.

in [Section](#page-237-0) [13.8.](#page-237-0)

physics is outside the scope of this course, but it is worth painting a general picture—enough to appreciate how much we can expect to get out of a PV panel.

<span id="page-221-1"></span>![](../figures/Ch13_SolarEnergy/_page_221_Figure_2.jpeg)

[Figure](#page-221-1) [13.4](#page-221-1) illustrates the basic scheme. The underlying idea is that adjoining two slabs of silicon into which small amounts of two kinds of impurities have been deliberately introduced<sup>[17](#page-450-0)</sup> that either contribute extra electrons (n-type, for negative charge donors) or create vacancies for electrons (p-type, for effective positive charge donors). Putting p-doped and n-doped materials together creates a [junction](#page-450-0)<sup>[18](#page-450-0)</sup> exhibiting a *contact potential*. The result is that "donated" [electrons](#page-446-1) right at the junction in the n-doped material decide to relocate across the junction to vacancies in the p-doped material, creating a wall of negative charge on the p-side of the junction and leaving behind ["holes"](#page-449-1) (missing electrons) effectively creating positive charges<sup>[19](#page-450-0)</sup> on the n-side of the junction. In the region right around the junction<sup>[20](#page-450-0)</sup> an electric field is set up between the separated charges. *Any electron wandering into this depletion region will be swept across the junction*, across the contact potential, and will contribute to a [current](#page-444-1) that is then driven around the external circuit to return to its p-side home.<sup>[21](#page-450-0)</sup> [Figure](#page-221-1) [13.4](#page-221-1) shows additional salient features that will be pointed out as the story develops below.  
<sup>17</sup>: ... either during or after the semicon-
ductor crystal growth; a process called
"doping"  

<sup>18</sup>: So-called p–n junctions form the basis
of diodes and transistors.  

<sup>19</sup>: When a (negatively-charged) electron
leaves an otherwise neutral medium, the
medium becomes more positively charged.  

<sup>20</sup>: ... called the "depletion region," as elec-
trons have been depleted from the portion
of the n-side adjacent to the junction  

<sup>21</sup>: Once it is "home," the electron will fill a
vacancy created by a sun-liberated electron
to end the journey#### <span id="page-221-0"></span>**13.3.1 Theoretical Efficiency of Photovoltaics**

We will now follow the fate of one [photon](#page-453-1) as it encounters the photovoltaic material. Doing so will expose the physical process of photovoltaics and simultaneously track losses to elucidate efficiency expectations.

The basic scheme is that a photon knocks an [electron](#page-446-1) away from an atom in the PV cell, and this electron has some chance of being swept across the junction upon which it contributes to a useful [current](#page-444-1).<sup>22</sup> The goal is to get an electron across the line. It is not unlike some sports where crossing a line is the goal, but many factors are lined up defending against successful attainment of this goal. Efficiency is related to the chance that a photon will produce a "win."**Figure 13.4:** PV cell structure and function. <sup>A</sup> [junction](#page-450-0) between 푛–doped and 푝–doped [semiconductors](#page-455-2) sets up an electric field across the junction. If an electron promoted to the [conduction band](#page-444-0) by an incoming [pho](#page-453-1)[ton](#page-453-1) wanders into the junction, it is swept across (red arrow) and successfully contributes to current. Electrons do not contribute if created above the junction—as is more probable for blue photons that are not likely to penetrate as far. Electrons do not contribute to the external (useful) [current](#page-444-1) if they [recombine](#page-454-1) (fill a [hole\)](#page-449-1) before finding the junction (red "poof").

ductor crystal growth; a process called ["doping"](#page-445-1)

of diodes and transistors.

19: When a (negatively-charged) electron leaves an otherwise neutral medium, the

20: . . . called the "depletion region," as electrons have been depleted from the portion of the 푛-side adjacent to the junction

vacancy created by a sun-liberated electron to end the journey.

<sup>22</sup> 22: Current is just flow of charge, and in this case is just movement of electrons through the external circuit.

A photon leaves the hot solar surface aimed right at a PV panel on Earth. The photon can be any "color," distributed according to the Planck spectrum<sup>23</sup> in [Figure 13.1.](#page-219-0) The most probable wavelength for a 5,800 K [blackbody](#page-442-1)—according to [Eq. 13.5](#page-218-2)—is ~0.5  $\mu$ m, but it could reasonably be anywhere from 0.2–3  $\mu$ m. The atmosphere will knock out (absorb or scatter) most of the ultraviolet light before it reaches the panel, and some of the infrared light is absorbed in the atmosphere as well. But almost 75% of the energy<sup>24</sup> makes it to the panel. What happens next depends on the wavelength.
<sup>23</sup>: The spectrum can be thought of as a probability distribution for photon wavelength, if picking out one photon.
<sup>24</sup>: This is roughly 1,000 W/m<sup>2</sup> out of the 1,360 W/m<sup>2</sup> incident at the top of the atmosphere (the solar constant which will hoFirst, we must understand something about the silicon material. The atoms in a typical silicon PV cell are arranged in an orderly lattice, grown as a single crystal. Expensive panels have mono-crystalline silicon, meaning that each 15 cm square cell comprising the panel is a thin slice of one giant crystal. Less expensive poly-crystalline (or multi-crystalline) panels have cells that are a patchwork<sup>25</sup> of randomly-oriented crystals at the millimeter to centimeter scale. But microscopically, both types are orderly crystals. Silicon has four electrons in its valence shell (outermost shell), so that a "happy" silicon atom is home to a four-outer-electron family. These electrons are said to exist in the valence band.<sup>26</sup> But provided a sufficient energy kick, an electron can leave home and enter the conduction band,<sup>27</sup> where it can freely move through the crystal and can potentially contribute to an electric current, if it finds the junction. The threshold energy level to promote an electron from the valence to the conduction band is called the band gap,<sup>28</sup> which for silicon is 1.1 eV ( $1.8 \times 10^{-19}$  J).
Infrared photons at a wavelength of 휆 > <sup>1</sup>.<sup>1</sup> <sup>휇</sup>m have an energy of 퐸 <sup>&</sup>lt; <sup>1</sup>.<sup>1</sup> eV,<sup>29</sup> 29: That<sup>휆</sup> <sup>=</sup> <sup>1</sup>.<sup>1</sup> <sup>휇</sup>m happens to correspond according to [Eq.](#page-217-1) [13.1.](#page-217-1) The energy falls below the [band](#page-441-0) [gap](#page-441-0) of silicon, and as such is not capable of promoting an electron within the silicon from the [valence band](#page-457-3) to the [conduction band.](#page-444-0) These longer-wavelength photons sail right through the silicon crystal as if it were transparent glass. Since these photons are not absorbed, the part of the incident energy in the infrared beyond 1.1 휇m is lost. For the solar spectrum, this amounts to 23%, and is portrayed in [Figure](#page-223-0) [13.5.](#page-223-0)

For the 77% of sunlight whose photons *are* energetic enough to bump an electron into the conduction band,<sup>[30](#page-221-1)</sup> it's game-on, right? Well, not so fast—literally. Photons whose energy is *higher* than 1.1 eV have more energy than is needed to lift the electron into the conduction band. It only takes 1.1 eV to promote the electron, so a blue-green photon at 0.5  $\mu$ m ( $\sim$  2.5 eV) has an excess of about 1.4 eV. The lucky electron is not just lifted out, but is given a huge boost in the process, rocketing out of the atom. It's going too fast! It knocks into atoms in the crystal and generally shakes things up a bit before settling down. We call this heat, or thermal energy:<sup>[31](#page-456-2)</sup> its excess kinetic energy is transferred to vibrations (randomized kinetic energy of atoms) in the crystal lattice. The blue curve in [Figure 13.5](#page-223-0) reflects this loss: we get to keep all the energy at 1.1  $\mu$ m (1.1 eV), thus the blue curve joins the overall black curve here.
<sup>[30](#page-221-1)</sup>: ... denoted as e<sup>-</sup> in [Figure 13.4](#page-221-1)
<sup>[31](#page-456-2)</sup>: Solar panels in the sun get pretty hot.probability distribution for photon wavelength, if picking out one photon.

1,360 W/m<sup>2</sup> incident at the top of the atmosphere (the [solar constant,](#page-455-3) which will be derived in [Section](#page-225-0) [13.4\)](#page-225-0).page [197.](#page-216-1)

26: The term "band" is used to describe energy levels. The valence band is a lower energy level.

27: ... higher energy level

valence band energy levels

to 1.1 eV is a numerical coincidence, but perhaps convenient, in that remembering 1.1 for silicon covers it from both directions.

−

31: Solar panels in the sun get pretty hot.

<span id="page-223-0"></span>![](../figures/Ch13_SolarEnergy/_page_223_Figure_1.jpeg)

But as the wavelength gets shorter and the energy gets higher, a greater fraction is lost to heat. Overall, 33% of the incident photon energy is lost to heat as the boosted electrons rattle the crystal before being tamed.

Now we're down to 44% of the original incident energy in the form of conduction-promoted electrons that have shaken off their excess kinetic energy. But then here's the rub: electrons are dumb. They don't know which way to go to find the junction, so aimlessly bounce around the lattice, in a motion called a random walk.<sup>32</sup> wander into the junction, where they are swept across<sup>33</sup> and contribute to external current. Others fall into an electron vacancy (a [hole\)](#page-449-1) in a process called [recombination:](#page-454-1) game over.<sup>34</sup> Roughly speaking, about 34: . . . red "poof" in [Figure](#page-221-1) [13.4](#page-221-1) three-quarters<sup>35</sup> of the electrons get lucky by wandering into the junction before being swallowed by a hole. So of the 44% available, we keep 32% (called the Shockley-Queisser limit [\[86\]](#page-436-0)).

Another significant loss arises because some photons are absorbed in the very top layer above the junction, so that the resulting electrons do not have the opportunity to be swept across the junction to contribute to useful energy. The shorter the wavelength, the shallower the photon is likely to penetrate into the cell.<sup>36</sup> Meanwhile, photons around 1 휇m are likely to penetrate deep—well past the junction—making it less likely that the liberated electrons will find the junction before settling into a new home (lattice site) via [recombination.](#page-454-1) [Figure](#page-221-1) [13.4](#page-221-1) reflects this color-dependence, and also depicts one electron from the blue photon being generated above the junction, which will not have an opportunity to do useful work by crossing the junction.

In total, the basic physics of a PV cell is such that 20% efficiency is a reasonable expectation for practical implementations.<sup>37</sup> Indeed, commercial silicon-based PV panels tend to be 15–20% efficient, not far from the theoretical maximum. This may seem like a low number, but don't be disappointed! Biology has only managed to achieve 6%

**Figure 13.5:** Energy budget in silicon PV cell. The areas of the four regions represent the fraction of the total incident energy going to each domain. All light at wavelengths longer than 1.1 휇m (infrared; 23%) passes through the silicon without being absorbed. The photons that *are* absorbed give excess kinetic energy to electrons, losing 33% of the incident energy as heat. This effect is progressively more pronounced the shorter the wavelength. Of the remaining 44%, about a quarter disappear as electrons ["recombine"](#page-454-1) with vacancies [\(holes\)](#page-449-1) in the silicon before getting a chance to contribute to a useful current by crossing the [junction,](#page-450-0) leaving 32% as the maximum theoretical efficiency.

32: . . . sometimes called drunken walk, de-Some get lucky and picted as meandering paths in [Figure](#page-221-1) [13.4](#page-221-1)

33: . . . red arrow in [Figure](#page-221-1) [13.4](#page-221-1)

34: ...red “poof” in Figure 13.4

35: Naïvely, 50% are lucky and wander up to the junction, and 50% make the wrong choice and go down. But even those initially going down still have a chance to wander back up to the junction before time expires and they [recombine,](#page-454-1) so that effectively 75% make it.

36: Any given photon has a probability distribution of being absorbed as a function of depth. Blue photons *can* penetrate deep, but are more likely to be absorbed near the front surface. A 1 휇m photon *can* be absorbed near the front surface, but it is more likely to penetrate deeper into the silicon.

37: Fancy, very expensive multi-junction PV cells may be used for special applications like in space, where size and weight are extremely important and cost is less of a limitation. These devices can reach efficiencies approaching 50% by stacking multiple junctions at different [band gaps,](#page-441-0) better utilizing light across the spectrum.

efficiency in the best-case photosynthesis (algae). PV technology beats that by a factor of three! And as we'll see in [Section](#page-232-0) [13.6,](#page-232-0) the only thing higher efficiency really does—besides driving up the price—is it makes the footprint (area occupied) smaller for the same power delivery. But it's already small enough to comfortably fit on most roofs, so efficiency is not a chief limitation at this point.

<span id="page-224-0"></span>![](../figures/Ch13_SolarEnergy/_page_224_Figure_2.jpeg)

**Figure 13.6:** [PV](#page-454-0) panels (modules) are constructed of typically 18, 36, 54, or 72 cells in series, two of which are depicted here. Cells are usually ∼15 cm squares layered exactly as depicted in [Figure](#page-221-1) [13.4.](#page-221-1) The bottom sides are covered by a continuous metal contact and the tops host a fine grid of metal contacts that minimize blockage of incident sunlight. Each cell presents ∼0.5 V, arranged *in series* to add up to tens of volts per panel. To accomplish this, the top grid of one cell is connected to the bottom contact on the next, all down the line.

PV panels are usually constructed of many individual PV cells wired in series, as depicted in [Figure](#page-224-0) [13.6.](#page-224-0) Each cell delivers maximum power when it's at a voltage around 0.45 V, and cells are usually arranged in strings of 18, adding to about 8 V. Panels commonly have 2, 3, or 4 such strings of 18—thus 36, 54, or 72 cells total—becoming 16 V, 24 V, or 32 V devices at peak power. [Figure](#page-224-1) [13.7](#page-224-1) shows typical performance curves for a PV cell (or whole panel) operating in various light levels. Recalling from [Eq.](#page-96-0) [5.2](#page-96-0) (p. [77\)](#page-96-0) that electrical power is current times voltage, the power put out by a PV panel can be found as the area of the rectangle formed from the origin to the operating point somewhere on the curve. The point that maximizes area (power) is shown in [Figure](#page-224-1) [13.7](#page-224-1) as the "maximum power point." A battery being charged might hold the panel to a lower voltage, whose corresponding rectangle has a smaller area, thus operating at less than the panel's maximum power.One serious downside of panels is that because cells are wired in series, partial shading of a *single* cell limits the [current](#page-444-1) the whole panel delivers to that of the *weakest link* in the chain. In other words, 17 of 18 cells in a chain might be in full sun, but if the shadow from a roof vent, chimney, or tree shades one cell and limits its current to 10% of its full value, the whole chain<sup>38</sup> 38: . . . because in series, each cell shares is knocked to 10%. Bypass diodes can isolate problem sections, but usually in chunks of 18–24 cells, so that the panel can still be seriously impaired by partial shading. Connecting panels in series also creates vulnerability to partial shadowing. This problem is sometimes mitigated via

#### **Box 13.1: Why Not Parallel?** in parallel.

Given the downsides of series connection of cells, why not connect cells in *parallel*—the only other option for connecting many cells together?

<span id="page-224-1"></span>![](../figures/Ch13_SolarEnergy/_page_224_Figure_8.jpeg)

**Figure 13.7:** Current–voltage ( $I$ – $V$ ) curve for a [PV](#page-454-0) cell. The cell in full sunlight will operate somewhere on the thick blue curve, and on a lower red curve under weaker illumination. The maximum power point (mppt) is about 0.45 V for silicon, while the nominal design might be for 0.35 V so that a 36-cell panel is sized to charge a 12 V battery. Rectangle area is proportional to [power](#page-453-4) delivered, since  $P = IV$ .the same current

micro-inverters: each panel has an inverter so that higher-voltage outputs are combined Series combination adds voltages, keeping the same common current. Parallel combination shares a common (low) voltage but adds currents. The same power (푃 <sup>=</sup> 퐼푉) obtains either way. But two problems arise from a parallel combination of cells. First, the ∼0.5 V voltage is too small to be useful for most devices. Second, the power lost in connecting wires scales as the square of current, so designing a system with a large current is asking for trouble.<sup>39</sup> 39: Making things worse, the voltage drop

That said, PV installations often combine panels in both series *and* parallel—like 10 panels in series in parallel to another 10 in series. By this time, the voltage is plenty high to offset the losses.

## <span id="page-225-0"></span>**13.4 Insolation**

Let's start our journey from the physics principles we covered in [Section](#page-218-0) 13.2. The sun's surface is a sweltering 5,770 K, meaning that it emits  $\sigma T^4 \approx 6.3 \times 10^7 \text{ W/m}^2$  over its surface. The sun's radius is about 109 times that of the earth's,<sup>40</sup> which itself is 6,378 km at the equator. Multiplying the radiation intensity by the area gives total power output:  $4\pi R_{\odot}^2 \sigma T^4 \approx 3.82 \times 10^{26} \text{ W}$ . That's one bright bulb!
  
40: Why this convoluted path? Context. Building from pieces we are more likely to know/remember better engages our understanding and ownership of the material.Sunlight spreads out uniformly into a sphere expanding from the sun. By the time it reaches Earth, the sphere has a radius equal to the Earth–Sun distance, which is  $r_{\oplus\odot} = 1.496 \times 10^{11}$  m.[<sup>41</sup>](#page-431-0) Spreading  $3.82 \times 10^{26}$  W over a sphere of area  $4\pi r_{\oplus\odot}^2$  computes to 1,360 W/m<sup>2</sup>. That's what we call the [solar constant](#page-455-3) [\[4\]](#page-431-0), and it's a number worth committing to memory.[<sup>42</sup>](#page-431-0)Earth intercepts sunlight over the *projected* area presented to the sun: a about context. disk of area  $\pi R_{\oplus}^2$ . Bright features like clouds and snow reflect the light See Fig. [9.6](#page-163-0) [\(p.144\)](#page-163-0) for a visual example. back to space without being absorbed, and even darker surfaces reflect *some* of the light. In all, 29.3% of the incoming light is reflected, leaving 960 W/m<sup>2</sup> absorbed by the  $\pi R_{\oplus}^2$  projected area of the planet. But now averaging the 960 W/m<sup>2</sup> input over the  $4\pi R_{\oplus}^2$  *surface area* of Earth cuts the number down by a factor of four,<sup>43</sup> to 240 W/m<sup>2</sup>.High latitude sites suffer more from low sun angles, and obviously cloudier locations will receive less sun at the surface. Taking weather into account, a decent number for the average amount of power from sunlight reaching the ground is about 200 W/m<sup>2</sup>. This is called [insolation](#page-450-1)<sup>44</sup>:—the "sol" part of the word stemming from solar.
overhead, so the amount of light hitting each
square meter of land is reduced when the
sun's rays are slanting in at an angle.
<sup>44</sup>: ... also called global horizontal irradi-
ance<span id="page-225-1"></span>

| Solar Flux Context                    | W/m²   |
|---------------------------------------|--------|
| Arriving at Earth                     | 1,360  |
| Full, overhead sun (no clouds)        | ~1,000 |
| Absorbed by $\pi R_{\oplus}^2$        | 960    |
| Absorbed by $4\pi R_{\oplus}^2$       | 240    |
| Typical insolation, includes weather  | ~200   |
| Typical delivered by 15% efficient PV | 30     |

in the lines is proportional to current, diminishing an already small voltage to even less by the time it gets to its application.

Building from pieces we are more likely to know/remember better engages our *understanding* and ownership of the material.

41: . . . ∼150 million kilometers, or 1 [AU](#page-441-1)

42: See: isn't it satisfying to know that the number *comes from somewhere*? It's not just a random fact, but *connects to other pieces*. That's what the earlier margin note meant

See Fig. 9.6 (p. 144) for a visual example.

43: We can understand this factor of four as two separate factor-of-2 effects determining how much solar power a particular location receives: one is simply day vs. night: half the time the sun is not up. The other half relates to the fact that the sun is not always *overhead*, so the amount of light hitting each square meter of land is reduced when the sun's rays are slanting in at an angle.

ance

**Table 13.1:** Summary of solar power densities. Full overhead sun can be larger than the global absorbed number because the global number includes reflection from clouds, while overhead direct sun corresponds to a local cloud-free condition.

[Table](#page-225-1) [13.1](#page-225-1) summarizes these various power densities, the last line being typical insolation multiplied by 0.15 to represent the yield from a 15% efficient photovoltaic panel lying flat in a location receiving an insolation of 200 W/m<sup>2</sup> . [Figure](#page-226-0) [13.8](#page-226-0) shows global insolation, variations arising from a combination of latitude and weather.

<span id="page-226-0"></span>![](../figures/Ch13_SolarEnergy/_page_226_Figure_2.jpeg)

**Figure 13.8:** Insolation onto locally horizontal surfaces for the world (for flat plates facing directly upward), in units of W/m<sup>2</sup> and kWh/m2/day. The area of the blue square in the middle of the Atlantic ocean is enough to satisfy current global energy demand, using 15% efficient solar collection (but distributed, of course). Source: [The World Bank.](#page-373-0)

<span id="page-226-1"></span>![](../figures/Ch13_SolarEnergy/_page_226_Figure_4.jpeg)

**Figure 13.9:** Horizontal insolation for the U.S. for a flat plate facing directly upward. Native units for the graphic are in kWh/m2/day, the break-points between colors running from 4.0 to 5.75 kWh/m2/day in steps of 0.25. These values can be converted to W/m<sup>2</sup> by multiplying by 1,000 W/kW and dividing by 24 h/day. Annotations are added once in each color band (in black or yellow) to indicate the equivalent measure in W/m<sup>2</sup> [\[87\]](#page-436-1). Alaska is not even close to scale. From [NREL.](#page-374-0)

[Figure](#page-226-1) [13.9](#page-226-1) shows the variation of insolation across the U.S. The latitude effect is evident, but also weather/clouds make a mark, giving the southwest desert the highest solar potential. Even so, the variation from best to worst locations<sup>45</sup> 45: . . . e.g., 250 vs. 150 <sup>W</sup>/m<sup>2</sup> is *not even a factor of two*.

Figures [13.8](#page-226-0) and [13.9](#page-226-1) are in the context of a flat surface.<sup>46</sup> For solar panels, it makes sense to tilt them to an angle equaling the site latitude and oriented toward the south.<sup>47</sup> The noon-time sun is always high in
47: ... toward the south for northern hemisphere locations; a more generally correct way to say it would be "toward the equator"45: ... e.g., 250 vs. 150 W/m²

47: . . . toward the south for northern hemisphere locations; a more generally correct

<sup>46: . . .</sup> as is the definition of [insolation](#page-450-1)

the sky near the equator, so panels there should lie flat.<sup>48</sup> But at high 48: . . . point mostly up northern latitudes, the sun is lower toward the southern horizon, so the panels should tilt up to best face the sun. Tilting at an angle equal to the latitude is the best compromise, as [Figure](#page-227-0) [13.10](#page-227-0) illustrates.

<span id="page-227-0"></span>![](../figures/Ch13_SolarEnergy/_page_227_Figure_2.jpeg)

![](../figures/Ch13_SolarEnergy/_page_227_Figure_3.jpeg)

<span id="page-227-1"></span>![](../figures/Ch13_SolarEnergy/_page_227_Figure_4.jpeg)

Tilting panels toward the equator at an angle equal to site latitude optimizes annual yield, and the results are shown in [Figure](#page-227-1) [13.11.](#page-227-1) Note that the numbers in [Figure](#page-227-1) [13.11](#page-227-1) are not strictly [insolations,](#page-450-1) since that's defined as what reaches *flat* ground. In this case, the area (square meters) is that of the *panel*, not of the *land*.

The fact that the numbers in [Figure](#page-227-1) [13.11](#page-227-1) are higher than in [Figure](#page-226-1) [13.9](#page-226-1) is not to say that the land offers more solar energy if the panels are tilted: just that an individual panel can get more light. But in this case, panels need to be spaced out to avoid shadowing,<sup>49</sup> 49: . . . which can be more devastating than as [Figure](#page-228-0) [13.12](#page-228-0) illustrates.

Some applications need to track the sun, like those that concentrate solar power, and only work when the sun is not blocked by clouds.<sup>50</sup> 50: Photovoltaics still produce 10–50% of This brings us to [Figure](#page-228-1) [13.13,](#page-228-1) showing the potential per square meter of collector (mirror or lens) used for the concentration (the topic of [Section](#page-238-0) [13.8.2\)](#page-238-0). The same pattern holds, in that the desert southwest dominates. But a look at the numbers indicates that the cloudier regions are not much better than just a flat panel facing upward (as is the case for [Figure](#page-226-1) [13.9\)](#page-226-1). In the southwest, where skies are often cloud-free, the boost can be

**Figure 13.11:** Solar potential for flat panels tilted to latitude, oriented south—relevant to PV panel installations. The graphic is presented in units of kWh/m<sup>2</sup>/day, the breakpoints between colors running from 3.0 to 6.5 kWh/m<sup>2</sup>/day in steps of 0.5. Annotations are added once in each color band (in black or yellow) to indicate the equivalent measure in W/m<sup>2</sup> [\[87\]](#page-436-1). From [NREL.](#page-374-1)just fractional area blocked, due to series arrangement of cells in panel modules

full capacity under cloudy skies during daylight hours, depending on how thick the clouds are: daylight still means photons.

<span id="page-228-0"></span>![](../figures/Ch13_SolarEnergy/_page_228_Figure_0.jpeg)

**Figure 13.12:** On a fixed piece of land receiving a fixed amount of sunshine at a slant angle, the amount of energy received is independent of whether the panels are flat or tilted. Just tilting the flat panels up (middle) results in self-shading. It makes the most sense to tilt and separate panels (right), one benefit being that fewer panels are needed to collect the same incident energy.

about 30% over the flat, upward-facing panel. Concentration schemes make less sense away from such regions.

<span id="page-228-1"></span>![](../figures/Ch13_SolarEnergy/_page_228_Figure_3.jpeg)

Stepping back, let's appreciate a few big-picture facets from these maps. First, numbers tend to be in the general neighborhood of 150–300 W/m<sup>2</sup>. Burn this range in—it's a useful context. Second, the variation from the most solar-intense places in the contiguous U.S. to the weakest areas<sup>[51](#page-10-51)</sup> is not more than a factor of two on an annual basis. This is astounding. The Mojave desert in California and the rain-forest Olympic Peninsula in Washington would seem to be practically day vs. night with respect to solar illumination. But not so much: only a factor of two.<sup>[52](#page-10-52)</sup> Part of what this means is that if storage over *annual* timescales could be realized, solar power would become practical almost everywhere.<sup>[53](#page-10-53)</sup>
  

<sup>[51](#page-10-51)</sup>: ... ignoring Arctic-leaning Alaska
  

<sup>[52](#page-10-52)</sup>: The northwest benefits from long summer days when clouds are also less likely.
  

<sup>[53](#page-10-53)</sup>: This would require huge storage capac-#### <span id="page-228-2"></span>**Box 13.2: Hours of Full-Sun Equivalent**

A useful take-away comes from the native units used in the three maps presented here: kWh/m<sup>2</sup>/day, as opposed to our preferred W/m<sup>2</sup>. Although they look different at a glance, kWh is a unit of energy, so kWh/day is a power, just like W. Since a kilowatt is 1,000 W and a day is 24 h, 1 kWh/day is 1,000 Wh/24 h = 41.67 W.<sup>54</sup> So we can multiply 6 kWh/m<sup>2</sup>/day by 41.67 to get 250 W/m<sup>2</sup>.**Figure 13.13:** Solar potential for tracking panels, facing directly toward the sun's position and requiring a cloud-free view of the sun (concentrating collectors). The graphic is presented in units of kWh/m2/day, the break-points between colors running from 4.0 to 7.5 kWh/m2/day in steps of 0.5. Annotations are added once in each color band (in black or yellow) to indicate the equivalent measure in W/m<sup>2</sup> [\[87\]](#page-436-1). From [NREL.](#page-374-2)

51: ...ignoring Arctic-leaning Alaska

mer days when clouds are also less likely.

ity: giant batteries, for instance.

54: The hours in numerator and denominator cancel, since the [kilowatt-hour](#page-450-2) is kW *times* hours.

But the main purpose of this box is to point out the following. Full overhead sunshine bathes the ground in about 1,000 W/m<sup>2</sup> . So if you could contrive to keep the sun directly overhead for 5 hours, you'd get 5 kWh of solar energy for each square meter on the ground. Therefore, if your site is listed as getting 5 kWh/m2/day, it's the *equivalent* amount you'd get from 5 hours of direct overhead sun.<sup>56</sup> 56: This equivalence relies on the conve-

1,000 <sup>W</sup>/m<sup>2</sup> What *actually* happens is that the day is longer than 5 hours, but . It would not work otherwise. for much of the day the sun is at a lower angle so that the panel is not directly illuminated, and weather can also interfere. This leads to a concept of full-sun-equivalent-hours. A site getting an annual average of 5.4 kWh/m2/day might be said to get 5.4 hours of full-sun-equivalent each day. It's a pretty useful metric.

[Box](#page-228-2) [13.2](#page-228-2) leads to a crucial bit of understanding on characterizing a PV system. Panels are rated on what they would deliver when illuminated by 1,000 W/m<sup>2</sup> at a temperature of 25<sup>o</sup>C.<sup>57</sup> So the measure in kWh/m<sup>2</sup>/day, or full-sun-equivalent hours tells you effectively what fraction of a day the panel will operate at its rated capacity.<span id="page-229-2"></span>**Example 13.4.1** A 250 W panel at a location getting 4.8 kWh/m2/day, or 4.8 full-sun-equivalent hours, is basically operating at 250 W for 4.8 hours out of every 24, or 20% of the time. So the panel delivers an *average* power of 50 W, not 250 W.<sup>58</sup> 58: We would need to apply a de-rating of

The 250 W rating is referred to as "peak" Watts, sometimes denoted 250 Wp. Panels are sold this way, and now cost about \$0.50/Wp.

A 30-year study by the National Renewable Energy Lab [\[88\]](#page-436-2) initiated in 1960 characterized solar potential across the U.S. and produced detailed statistics on what each location might expect to collect each month for panels in different orientations. [Table 13.2](#page-229-0) is a subset of the complete data for St. Louis, Missouri.<sup>59</sup> All cases in [Table 13.2](#page-229-0) correspond to a panel facing south, at various tilts (including flat, at 0° and vertical at 90°; other tilts are relative to the site latitude of  $\theta \approx 39$ °). From this, we see that tilting the panel at the site latitude delivers an annual average of 4.8 kWh/m<sup>2</sup>/day, matching the graphic expectation from [Figure 13.11](#page-227-1). Also shown is the monthly breakdown and how different tilts translate to performance. We will visit this table again in [Section 13.6](#page-232-0) to help us establish an appropriate size for a residential installation.<span id="page-229-0"></span>

| Angle     | Jan | Feb | Mar | Apr | May | Jun | Jul | Aug | Sep | Oct | Nov | Dec | Year |
|-----------|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|------|
| 0°        | 2.2 | 2.9 | 3.9 | 5.0 | 5.9 | 6.4 | 6.4 | 5.7 | 4.6 | 3.5 | 2.3 | 1.8 | 4.2  |
| $θ$ - 15° | 3.2 | 3.8 | 4.6 | 5.4 | 5.9 | 6.3 | 6.3 | 6.0 | 5.3 | 4.5 | 3.2 | 2.7 | 4.8  |
| $θ$       | 3.6 | 4.2 | 4.7 | 5.3 | 5.6 | 5.8 | 5.9 | 5.7 | 5.3 | 4.8 | 3.5 | 3.1 | 4.8  |
| $θ$ + 15° | 3.8 | 4.3 | 4.6 | 4.9 | 4.9 | 5.0 | 5.1 | 5.2 | 5.1 | 4.8 | 3.7 | 3.3 | 4.6  |
| 90°       | 3.5 | 3.7 | 3.4 | 3.1 | 2.6 | 2.4 | 2.6 | 3.0 | 3.5 | 3.8 | 3.2 | 3.0 | 3.2  |

<sup>55</sup> 55: It's 1,360 W/m<sup>2</sup> at the top of the atmosphere, and the atmosphere blocks/scatters some of the wavelengths outside the visible part of the spectrum.

nient fact that full overhead sun is about

57: The 1,000 W/m<sup>2</sup> is reasonable, but a photovoltaic panel in full sun will be about 30–40◦C hotter than its surroundings (it gets hot!), so it would have to be very cold outside to meet the specification of 25◦C panel temperature. Solar panel performance wanes when hot, and will only reach 85–90% of rated capacity in typical conditions.

0.85 to 0.9 to account for typical PV temperatures in the sun, bringing the panel to about 45 W average power.

(1994), *Solar Radiation Data Manual for Flat-Plate and Concentrating Collectors*

U.S.

<span id="page-229-1"></span>![](../figures/Ch13_SolarEnergy/_page_229_Figure_14.jpeg)

**Figure 13.14:** Panel tilts for [Table](#page-229-0) [13.2,](#page-229-0) for 휃 = <sup>39</sup>◦ .

**Table 13.2:** Solar exposure (kWh/m2/day) for a south-facing panel in St. Louis, MO, at various panel tilts (휃 is latitude, which happens to be 39◦ for St. Louis). 0 ◦ means a panel lying flat, pointing straight up (like on a flat roof), and 90◦ means vertical, like on a (south-facing) wall (see [Figure](#page-229-1) [13.14\)](#page-229-1).

## <span id="page-230-0"></span>**13.5 The Incredible Solar Potential**

The potential of sunlight can be assessed by pieces we have already seen. Multiplying the [solar constant](#page-455-3) of 1,360 W/m<sup>2</sup> by the projected area of Earth ( $\pi R_{\oplus}^2$ ) and by 0.707 to account for the 29.3% reflection loss, we compute that Earth absorbs solar energy at a rate of  $1.23 \times 10^{17}$  W, or 123,000 TW (1 TW is 10<sup>12</sup> W). Compared to the 18 TW societal scale, that's *huge*! Notice that the non-reflected entries back in Table [10.2](#page-187-0) [\(p. 168\)](#page-187-0) add<sup>60</sup> to this same value.Placing solar panels on just 10% of the land (itself 29% of Earth's surface area) capturing the incoming energy<sup>61</sup> at 15% efficiency would produce 61: . . . out of the 123,000 TW total solar power at ∼500 TW: about 25 times today's 18 TW usage rate. This, in turn, means that our current energy demand could be met by covering only 0.4% of land<sup>62</sup> with photovoltaic panels: see [Figure](#page-226-0) [13.8](#page-226-0) for a visual 62: . . . 1/25 of the 10% starting point representation of how much this is. Solar is the *only* currently-available resource that can come anywhere *close* to satisfying our current energy appetite.<sup>63</sup> 63: As we have seen, global wind may be And it exceeds our demand by such a huge margin! We therefore have reason to be excited about solar energy: the raw numbers are great news, indeed.

So it seems like a done deal. Solar. Let's get started! Wait, why aren't we there yet?

Naturally, solar has some downsides. First, the cost. Panel cost has dropped to something like \$0.50 or less per peak-Watt. To get 10 TW of delivered (average) power at typical locations getting 20% capacity factor<sup>64</sup> would require about 50 TW<sub>p</sub> [\(Example](#page-229-2) [13.4.1](#page-229-2) defines  $W_p$ ), costing 25 trillion dollars. The cost of other necessary components and installation double the cost for utility-scale projects [\[89\]](#page-436-3), bringing the cost to \$50 trillion.<sup>65</sup> The global annual economy is not quite twice this. To outfit the world with the requisite number of panels would take about 60% of the economy for a year, or 6% over 10 years, or 1.5% continuously.<sup>66</sup> For comparison, the world goes through 30 billion [barrels](#page-442-2) of oil each year at a cost of \$50/bbl, meaning \$1.5 trillion per year. Installing enough panels to fully satisfy demand would cost three-decades-worth of the *entire* global petroleum budget. So it's not going to happen fast. To put things on a personal scale, Americans use power at a rate of 10,000 W. To cover this, we would need about 50 kW<sub>p</sub> of panel per person, costing \$50k per person.<sup>67</sup> When can we expect your payment?Another daunting realization is that even though only 0.4% of the land is needed to match today's demand, this is comparable to the amount of area currently covered by roads and buildings. A road trip across the country conveys a sense for how vast (and boring) all that pavement can be. And pavement is a fancy form of dirt. It is true that PV panels are *also* an ultra-pure, ultra-fancy form of dirt. But it's a different level of high-tech. It becomes hard to fathom that much PV around the world.

by the surface and atmosphere, respectively

61: ... out of the 123,000 TW total

62: ...1/25 of the 10% starting point

limited to a few TW, and global hydropower would be hard-pressed to reach 2 TW.

64: 20% of 24 hours corresponds to 4.8 full-

65: The cost over the ∼40 year lifetime of the panels is already competitive with conventional means, but when fuel cost is zero, *all* the cost is up-front, which presents a significant barrier.

66: . . . based on 40 year effort, at which point the first panels need replacing

Americans use presently is in thermal form (fossil fuels), at ∼35% efficiency. For nonheating applications that can use electricity, solar has an advantage. On the other hand, mitigating intermittency via storage requires a larger PV installation by as much as a factor of two. For the purposes of a crude estimate, we'll call it even and say that 10 kW per capita from PV would cover the entire demand 100% of the time.

A major impediment to solar power is its **intermittency**. [Figure](#page-231-0) [13.15](#page-231-0) shows 31 days of solar capture, along with typical state-wide electricity demand. The two do not look very similar: not well matched. Demand is far more constant than the solar input, which is obviously zero at night. Even the peaks do not line up well, since demand is highest in the evening, well after solar input has faded away.<sup>68</sup> 68: Recall that wind has a similar problem (Fig. [12.6; p.190\)](#page-209-0).

<span id="page-231-0"></span>![](../figures/Ch13_SolarEnergy/_page_231_Figure_3.jpeg)

**Figure 13.15:** Solar input (red) and electricity demand (blue) look nothing alike. Solar data from the author's home begins 31 March 2020, while demand is for California. Tick marks denote the start of each date, at midnight. April 22–27 are essentially perfect cloudless days, while the earlier part of the month had rainy periods. Note that even a very rainy day (April 10) provides *some* solar power (15% as much as a full-sun day). Intermittent clouds cause the "hair" seen on some days. The [capacity factor](#page-443-0) for the month is 19%, while the perfect six days near the end perform at 27% capacity. From this, we infer that weather caused the yield to be 70% what it would have been had every day been cloudless.

Storage is required in order to mitigate the intermittency, allowing the choppy solar input to satisfy the demand curve of [Figure](#page-231-0) [13.15.](#page-231-0) We don't have good solutions for seasonal storage,<sup>69</sup> so a complete reliance on solar energy would necessitate over-building the system to handle months of low-sun conditions through winter (see the annual variation in [Table](#page-229-0) [13.2\)](#page-229-0), making it cost all that much more.  
<sup>69</sup>: It's not a matter of how long the energyFinally, all energy is not equivalent and substitutable. Solar PV cannot power passenger airplanes or power our cars down the road real-time (only via storage).<sup>70</sup> For all its potential, the hangups are serious enough that more than 60 years after the first demonstration of a photovoltaic cell, less than 1% of our energy derives from this ultra-abundant source.  
70: It is possible to build a solar-powered#### <span id="page-231-1"></span>**Box 13.3: Why no Solar Planes?**

Consider that full overhead sun delivers 1,000 W/m<sup>2</sup>. The top surface area of a typical commercial airplane (Boeing 737) is about 450 m<sup>2</sup>. If outfitted with the most expensive space-worthy multi-junction PV cells getting 50% efficiency, the plane would capture about 500 W/m<sup>2</sup> and a total of 225 kW. Sounds like a lot! The problem is that a Boeing 737 spends about 7 MW while cruising (and more during the climb). We're shy by a factor of about 25, even in optimal<sup>[71](#note-71)</sup> conditions! Any solar-powered airplane<sup>[72](#note-72)</sup> would be very light and very slow by air travel standards. See also Box [17.1 \(p. 290\)](#page-309-0) on the difficulty of battery-powered planes.is stored, but a matter of sufficient *capacity* to store *enough* excess energy in summer for use during the darker winter.

aircraft or car, but not airplanes and cars as we know them (see [Box](#page-231-1) [13.3\)](#page-231-1). We can consider such things to be "cute" demonstrations, rather than a viable path to substitution.

71: An airplane will not always have full overhead sun!

72: If your niece or nephew draws a solar plane in crayon, just smile, say it's very nice, put it on the refrigerator, and cry inside.

Cars have a similar problem: a top area around 10 m<sup>2</sup> equipped with the most expensive PV money can buy would get 5 kW, or less than 7 horsepower. That's about 20 times less powerful than typical cars, so again: light and slow.## <span id="page-232-0"></span>**13.6 Residential Solar Considerations**

Despite these drawbacks, it can still make a lot of sense<sup>[73](#page-7-1)</sup> to invest in solar photovoltaics for the home. We'll explore sizing and cost in this section.#### <span id="page-232-1"></span>**13.6.1 Configurations**

A typical household uses much or most of its energy when the sun is not shining: lighting, cooking, evening entertainment, charging an electric vehicle, etc. To get around this, the system would need to have local storage,<sup>74</sup> 74: . . . batteries: expensive, require mainteor be tied to the regional electrical grid so that excess production can be exported in the daytime and electricity produced by the utility used at night or when household demand exceeds solar production. The overwhelming majority of solar installations in the U.S. are [grid tied,](#page-448-0) and very few mess with batteries, which can double the cost of a system and need replacement before the system has paid for itself in electricity bill savings.

#### **Box 13.4: Disappointing Dependence**

A disappointing surprise to many who "go solar" is that their house has no power when the electrical service to the house is disrupted even in the light of day. A [grid tied](#page-448-0) system *needs* the grid to operate. Safety concerns prohibit PV systems from continuing to energize a disabled grid.

Only "off-grid" battery systems continue to work in these scenarios, but then the disappointment shifts to the price tag, maintenance, and replacement of worn-out batteries after a few thousand cycles.

While a description of the components and practical workings are beyond the scope of this book, students might be interested in an article the author wrote after first getting started tinkering with PV systems [\[90\]](#page-436-4): Murphy (2008), "Home photovoltaic".## <span id="page-232-2"></span>**13.6.2 Sizing and Cost**

How large does an installation need to be? If the goal is to cover annual or monthly electricity use in a grid-tied system, the only two pieces of information needed are the typical electricity consumption in the an off-grid PV system he built: a solar enthusiast when it comes down to it.

nance, and periodic replacement

systems for physicists"

relevant period and the average solar input at that location for the period of interest.

The first can be surmised from electricity bills, usually giving a monthly total usage in kWh. We can get an approximate average scale from Fig. [7.2](#page-124-0) [\(p.105\),](#page-124-0) which indicates that 42% of residential energy (11.9 [qBtu](#page-454-2) per year) is from electricity. That's 5 qBtu, or  $5.3 \times 10^{18}$  J in one year ( $3.156 \times 10^7$  s), or 167 GW. Distributed among 130 million households in the U.S.,<sup>[75](#page-124-0)</sup> average household electricity consumption is 1,285 W. Applied over 24 hours, this makes for just over 30 [kilowatt-hour](#page-451-1) (kWh) per day for an average household.<sup>[76](#page-124-0)</sup>The next piece is solar potential at the location of interest. We'll use the excerpted data from [\[88\]](#page-436-2) [\[88\]](#page-436-2): National Renewable Energy Lab for St. Louis, Missouri found in [Table](#page-229-0) [13.2.](#page-229-0)

<span id="page-233-0"></span>**Example 13.6.1** Let's design a grid-tied PV system for an average U.S. household in an average<sup>77</sup> U.S. city (St. Louis). We'll orient the panels facing south and tilted to the site latitude (39°) and purchase PV panels at 18% efficiency (pretty typical).  
<sup>77</sup>: ...solar-wise[Table](#page-229-0) [13.2](#page-229-0) indicates that for this configuration we can expect an annual average of 4.8 kWh/m<sup>2</sup>/day of input. If we're shooting for 30 kWh per day, we would need 6.25 m<sup>2</sup> of panel operating at 100% efficiency.<sup>[78](#page-229-1)</sup> 78: . . . Divide 30 kWh/day byBut 18% panels will require about 35 m<sup>2</sup> of panel,<sup>79</sup> which would be a square array about 6 meters on a side (about 20 feet) or a rectangle 5 by 7 meters, etc. The total area (400 square feet) is much smaller than a typical house footprint, so that's good news.But panels are not marketed by the square meter. They are sold in terms of peak Watts: what the panel would deliver in 1,000 W/m<sup>2</sup> sunlight (see [Example](#page-229-2) [13.4.1\)](#page-229-2). How do we convert? Two ways are instructive.

**Example 13.6.2** In one method, we multiply the 35 square-meter area from [Example](#page-233-0) [13.6.1](#page-233-0) by 1,000 W/m<sup>2</sup> and then by the PV efficiency (18% in this example) to get how much would be delivered: 6.3 kW.

Alternatively, we could adopt the interpretation of 4.8 kWh/m2/day as the equivalent full-sun hours operating at peak output [\(Box](#page-228-2) [13.2\)](#page-228-2). To get our target 30 kWh in 4.8 hours of full-sun-equivalent, we would need to produce 6.25 kW for those 4.8 hours.<sup>80</sup> 80: 6.25 kW times 4.8 hours is 30 kWh.

We get the same answer either way, which is a good check.<sup>81</sup> 81: The math is actually just the same, but

We should assume that the panels will not achieve their rated potential due to the facts that:

- I The 25◦C specification is almost never realized for a PV panel in the sun: PV panels in the sun get hot, and less efficient as a result;
- I The panels will get a little dirty;

75: . . . makes sense for a population of 330 million: translates to 2.5 people per household, on average

76: This is another case where students might suggest replacing this whole paragraph with the result. The point is to build connections, context, and tools to apply previous knowledge.

(1994), *Solar Radiation Data Manual for Flat-Plate and Concentrating Collectors*

77: ...solar-wise

4.8 kWh/m2/day 79: . . . Divide 6.25 m<sup>2</sup> which would be a by 0.18

80: 6.25 kW times 4.8 hours is 30 kWh.

we rearranged the order and interpretation.

I The equipment that converts panel output to [AC](#page-441-2) electricity is not 100% efficient.

So it's a good idea to bump the number up by 20% or so, and order a 7.5 kW PV system for the case under study. A typical full cost (panels, electrical converters, installation) lately runs just shy of \$3 per peak Watt [\(Figure](#page-234-1) [13.16\)](#page-234-1), which in this case brings the price tag to roughly \$20k. If electricity costs \$0.15 per kWh—approximately the national average—each 30 kWh day costs \$4.5, accumulating to \$20k after 12 years. Federal and state incentives can make the [payback time](#page-453-5) shorter.

What would these numbers become if trying to meet monthly instead of annual demands? December is usually the worst month for PV in the northern hemisphere, when the sun is lowest in the south, and the days are shortest. [Table](#page-229-0) [13.2](#page-229-0) backs this up, showing 3.1 kWh/m2/day for the chosen panel orientation in December. This is about two-thirds the annual average, so we would need to increase the size of the system (and thus cost and [payback time\)](#page-453-5) by a factor of 1.5 to produce enough in December.<sup>82</sup>

If sizing for an off-grid system, we need to factor in some inefficiency for battery charge/discharge and design for poorer months, so should increase by another factor of at least 1.5. The cost of batteries can be rather large, too. A good rule of thumb is to have at least three days of storage in the event of no solar input for several days during a stormy period. For our 30 kWh per day target, we would want about 100 kWh of storage. As an easy way to get a cost estimate for storage, the Tesla powerwall 2 is 13.5 kWh<sup>83</sup> and costs about \$7k apiece. If we follow along, the cost of 83: . . . so we would need about 8 the off-grid PV system for 30 kWh/day at an installation cost of \$3/W will be 7500 W <sup>×</sup> <sup>1</sup>.<sup>5</sup> <sup>×</sup> <sup>1</sup>.<sup>5</sup> <sup>×</sup> \$3 <sup>≈</sup> \$50k for panels/installation plus \$56k for batteries.<sup>84</sup> Then the batteries may be in need of replacement every roughly doubling the total cost. 10–15 years.<sup>85</sup>

If this seems rather alarming, don't worry—there's a trick to making it sand full charge cycles. much more affordable/practical: **don't demand 30 kWh per day**! Even though we picked 30 kWh/day due to the fact that it is the average American electricity demand, it is a worthwhile challenge<sup>86</sup> to seek ways 86: See [Chapter](#page-347-0) [20](#page-347-0) for examples. to use *far* less energy than the average. Trying to make solar fit our present expectations may be the wrong approach. Also, expecting to get away from fossil fuels *and* have it be cheaper may be unrealistic.

# <span id="page-234-0"></span>**13.7 Photovoltaic Installations**

The [Energy Information Administration's](#page-445-2) [Electric Power Monthly](#page-446-2) (EPM) [\[85\]](#page-436-6) provides detailed statistics on power generation in the U.S. Pho- *Electric power monthly* tovoltaic data is available in the [EPM'](#page-446-2)s tables 1.17.B and 6.2.B. In the usual way, we first look at installed capacity, based on the actual average *delivered* power. [Figure](#page-235-0) [13.17](#page-235-0) shows the situation in the U.S. California is

<span id="page-234-1"></span>![](../figures/Ch13_SolarEnergy/_page_234_Figure_9.jpeg)

**Figure 13.16:** Evolving price of PV installation per peak Watt. Yellow is for the panels; the two blues for electronics; peach is labor; and hashed is for the utility hookup, inspection, taxes, profits [\[89,](#page-436-3) [91\]](#page-436-5). From [NREL.](#page-374-3)

82: . . . resulting in over-production in summer

83: ...so we would need about 8

84: It is often the case that battery cost is comparable to the rest of the system,

85: Good batteries generally last a few thou-

86: See Chapter 20 for examples.

[\[85\]](#page-436-6): U.S. Energy Inform. Admin. (2020),

<span id="page-235-0"></span>![](../figures/Ch13_SolarEnergy/_page_235_Figure_1.jpeg)

rocking it! The average solar power in California was 4.3 GW in 2018, far ahead of the next biggest: North Carolina at 0.82 GW. For California, this is 13% of its electricity. But electricity production is 38% of all energy in the U.S., so we might say that California gets about 5% of all its energy from solar. This is far ahead of other states.<sup>87</sup> The U.S. as a whole gets about 0.9% of its energy from solar. [87](#page-9-1): North Carolina got about 5% of its electricity from solar in 2018, or less than 2% of<span id="page-235-1"></span>![](../figures/Ch13_SolarEnergy/_page_235_Figure_3.jpeg)

Next, we divide by area to get power density from photovoltaic installations. A site having an insolation of 200 W/m<sup>2</sup> and 15% efficient panels has access to 30 W/m<sup>2</sup> of production capability [\(Table](#page-225-1) [13.1\)](#page-225-1). [Figure](#page-235-1) [13.18](#page-235-1) shows how much we're actually getting. New Jersey has its moment in the sun, here. A few sites (NJ, MA) are pushing<sup>88</sup> 15 mW/m<sup>2</sup>, which is a factor of 2,000 lower than the full potential. What this says is that only 1/2,000 of the land (0.05%) is covered by solar panels. This sort-of makes sense, right?On a per-population basis [\(Figure](#page-236-1) [13.19\)](#page-236-1), Nevada shines brightest, at 180 W per person.<sup>89</sup> 89: . . . still small compared to the American The southwestern U.S. is doing well overall, as is North Carolina on this measure.

Finally, we look at [capacity factor:](#page-443-0) how much was generated compared to installed capacity [\(Figure](#page-236-2) [13.20\)](#page-236-2). We expect something like 20%, corresponding to 4.8 full-sun-equivalent hours per day. The best states top out at about 0.27, equating to about 6.5 full-sun-equivalent hours per day. States at higher latitude and/or having more clouds will do

**Figure 13.17:** Photovoltaic power production by state, in GW, in 2018.

tricity from solar in 2018, or less than 2% of all its energy.

**Figure 13.18:** Photovoltaic power production areal density by state, in milliwatts per square meter.

for hydroelectricity in Washington state (Fig. [11.6; p. 179](#page-198-0)) and  $17 \text{ mW/m}^2$  for wind in Iowa (Fig. [12.9; p.192](#page-211-0)).metric of 10,000 W/person

<span id="page-236-2"></span><span id="page-236-1"></span>![](../figures/Ch13_SolarEnergy/_page_236_Figure_1.jpeg)

<span id="page-236-3"></span>more poorly on this measure. Alaska clocks in just over 0.1, mapping to about 2.5 hours per day, on average.

| Country | installed<br>(GWp) | average<br>(GW) | % of all<br>energy | global share<br>(%) |
|---------|--------------------|-----------------|--------------------|---------------------|
| China   | 175                | ∼18             | 1.2                | 27                  |
| U.S.    | 62                 | 10.6            | 0.9                | 16                  |
| Japan   | 56                 | 6.5             | 3.5                | 10                  |
| Germany | 46                 | 5.0             | 3.3                | 7.5                 |
| India   | 27                 | 4.1             | 1.5                | 6                   |
| World   | 510                | 67              | 1.5                | 100                 |

Globally, two-thirds of the photovoltaic capacity is represented by five countries, shown in [Table](#page-236-3) [13.3.](#page-236-3) Note that delivered power is significantly lower than installed capacity because of the low [capacity factor](#page-443-0) for solar.

#### <span id="page-236-0"></span>**13.7.1 Pros and Cons of Photovoltaics**

Before advancing to solar thermal generation, let's summarize the major advantages and disadvantages of solar [photovoltaics.](#page-453-0) First, the good stuff:

I PV taps into a super-abundant resource—the only renewable that has such a margin;

*© 2022 T. W. Murphy, Jr.; [Creative Commons Attribution-NonCommercial 4.0 International Lic.;](https://creativecommons.org/licenses/by-nc/4.0/) Freely available at: [https://escholarship.org/uc/energy\\_ambitions.](https://escholarship.org/uc/energy_ambitions)*

**Figure 13.19:** Per capita photovoltaic power production by state, in Watts per person.

**Figure 13.20:** Photovoltaic capacity factors by state. While we see lots of darker green, it's because everybody has similarly *low* numbers, due to unavoidable nighttime and low sun angles. Somebody tell Wyoming, North Dakota, and Alabama to get with the program!

**Table 13.3:** Top five global producers of [PV](#page-454-0) power in 2018, accounting for two-thirds of the world's total production [\[92,](#page-436-7) [93\]](#page-436-8). The installed PV corresponds to peak watts (Wp), or production in full overhead sun.

- I PV technology has no moving parts or steam; panels are robust and last a long time;
- I PV is one of the few resources that can fit on a rooftop and provide self-contained electricity generation;
- I PV efficiency is rather good: close to theoretical expectations and much better than biology has managed at getting energy from sunlight;
- I PV technology works well, and despite expense has been deployed on rooftops across the world;
- I Life-cycle CO<sup>2</sup> [emissions](#page-451-2) are 15 times smaller than that of traditional fossil fuel electricity [\[68\]](#page-435-0); [\[68\]](#page-435-0): (2020), *Life Cycle GHG Emissions*
- I PV is often a good solution when utility electricity is far away.

And now the less attractive aspects:

- I PV is intermittent, and not well-matched to energy demand; it would be hard to "balance" the electrical grid if too much of the input came from such an intermittent source, and storage is difficult;
- <sup>I</sup> PV is still expensive<sup>90</sup> 90: Cost *has* been a major barrier, but may relative to prevailing energy resources especially important in terms of up-front cost;
- I Electricity alone is not well-suited to many of our current energy demands, like transportation and industrial heat/processing;
- I Stand-alone operation requires batteries, at least doubling the cost and adding maintenance/replacement demands;
- I Even partial shading can be disproportionally disruptive;
- I PV manufacturing involves environmentally unfriendly chemicals;
- I PV deployment can harm habitats if installed in undeveloped areas.

# <span id="page-237-0"></span>**13.8 Solar Thermal**

[Photovoltaics](#page-453-0) [\(Section](#page-220-0) [13.3\)](#page-220-0) convert sunlight directly into electricity, but this is not the only way to harness energy from the sun. Solar energy can also be used for *heat*. We'll first have a brief look at home heating, then turn to electricity generation from solar heat.

## <span id="page-237-1"></span>**13.8.1 Passive Solar Heat**

Full sun delivers something like 1,000 W/m<sup>2</sup> at the earth's surface. Now imagine a window in a house intercepting 1.5 m<sup>2</sup> of sunlight, in effect admitting 1,500 W into the home—like a space heater, and it's free! Depending on window construction, some of the infrared energy may be blocked, so maybe not all 1,000 W/m<sup>2</sup> will make it inside, but a sizable portion will. Clever design has south-facing windows for receiving low-angle winter sun, but an overhang to keep out the high summer sun

cease to be so as prices fall further.

91: ... dark rock or brick works well

[\(Figure](#page-238-1) [13.21\)](#page-238-1). A dark and massive absorber<sup>91</sup> inside the house capturing 91: . . . dark rock or brick works well the heat can continue to provide warmth through the evening hours. The Passive House designs mentioned in the context of [Box](#page-106-0) [6.1](#page-106-0) (p. [87\)](#page-106-0) attempt to maximize solar capture so that little active heating is required.

<span id="page-238-1"></span>![](../figures/Ch13_SolarEnergy/_page_238_Figure_3.jpeg)

**Figure 13.21:** A well-designed house has thick walls, thick insulation, and doublepaned windows. Even better, it can have south-facing windows that admit sunlight in the winter but not in the summer (the overhang shields the window). A large, dark thermal mass—stone or brick works well can absorb energy and continue to release heat into the evening.

#### <span id="page-238-0"></span>**13.8.2 Solar Thermal Electricity**

While 1,000 W/m<sup>2</sup> is nice, the power is too diffuse to get anything very hot and create a large enough  $\Delta T$  to allow the operation of an efficient heat engine (Sec. [6.4; p. 88\)](#page-107-0). More complex arrangements can *concentrate* solar power—think of a magnifying glass—to heat up a liquid in pipes. [Figure 13.22](#page-238-2) shows an example of a parabolic reflector that can track the sun to concentrate light onto the energy-absorbing central pipe. This shape can be extruded along a long cylinder—a “trough”—following the pipe.<span id="page-238-2"></span>![](../figures/Ch13_SolarEnergy/_page_238_Figure_7.jpeg)

**Figure 13.22:** Solar trough cross sections showing the focusing of sunlight onto a central pipe. The troughs can be oriented to follow the sun.

<span id="page-238-3"></span>![](../figures/Ch13_SolarEnergy/_page_238_Figure_9.jpeg)

**Figure 13.23:** A common solar thermal power scheme uses parabolic "trough" reflectors to focus sunlight onto a central pipe, which carries oil that can be heated to very high temperatures for making steam to run a traditional electrical power plant very much like that of [Fig.](#page-109-0) [6.2](#page-109-0) (p. [90\)](#page-109-0). Optional thermal storage can save heat for later use.

[Figure](#page-238-3) [13.23](#page-238-3) shows a schematic representation of a typical [solar thermal](#page-455-4) [\(ST\)](#page-455-4) collector, and a picture of one appears in [Figure](#page-239-0) [13.24.](#page-239-0) A curved reflector tilts to track the sun, concentrating light onto a long pipe in

<span id="page-239-0"></span>**Figure 13.24:** Parabolic trough-based [ST](#page-455-4) plant, in which part of the power generation facility is seen in the background. Reflectors must be spaced out to prevent

<span id="page-239-1"></span>self-shadowing. From [U.S. DoE.](#page-374-4)

front of the reflector carrying a fluid (usually oil) that can be heated to a high temperature by the absorbed sunlight. The hot oil pipes can then be run through water to boil it and make steam, thereafter driving a traditional steam power plant. Such [ST](#page-455-4) arrangements are sometimes called [concentrated solar power](#page-444-2) (CSP). Another common variant—called a "power tower"—is shown in [Figure](#page-239-1) [13.25,](#page-239-1) in which an array of steerable flat mirrors on the ground direct sunlight to the top of a central tower to make steam.

As for efficiency, solar thermal is at face value similar to PV: 15–20% is fairly typical. Broken down, roughly 50–75% of the available energy successfully transfers to the fluid, and then the heat engine delivers about 25–30% efficiency. But these numbers only apply if we count just the area of the reflective *collector*. Because they have to track the sun, and self-shadowing is to be avoided, only a small amount of the *land area* is occupied by the reflectors. Characterization of real facilities indicates that only 3% of the solar energy hitting the patch of land corresponding to the power plant is exported in the form of electrical energy.

But efficiency is not everything. 3% of a gigantic resource like solar energy input can still be tremendously large. It translates to over 6 W/m<sup>2</sup> for a standard insolation of 200 W/m<sup>2</sup>, which is about thirty-times better than wind, per land area. While a field of [PV](#page-454-0) panels outperform an [ST](#page-455-4) installation by a factor of 5–6, the technologically simpler solar thermal designs can be more cost effective than PV. Reflectors and oil pipes are low-tech cheap devices, compared to photovoltaic material. The production cost for solar thermal is estimated to be about \$0.06/kWh, which is lower than the typical retail cost of electricity, but still a factor of two higher than fossil fuel electricity production costs.One disadvantage of solar thermal is that concentration only works when the sun itself is visible in the sky: no obscuring clouds. One way to think of it is: if you can't see your shadow, solar concentration will not work. Meanwhile, PV panels will still produce a meaningful amount of daytime electricity from the bright sky and clouds even if the sun itself is not "out."

Balancing this disadvantage is the fact that solar thermal has some built-in storage capacity, in that the heated oil can be “banked” for some hours<sup>92</sup> and continue to produce electricity even during the passage of a cloud or for a few hours into the evening. In this sense, it can better match the peak of electrical demand (early evening: [Figure 13.15\)](#page-231-0) than can PV, which goes to zero once the sun sets. <sup>92</sup>: . . . thus the “optional storage” block in [Figure 13.23](#page-231-0)As seen in [Figure](#page-228-1) [13.13,](#page-228-1) the desert southwest is the best place in the U.S. for solar thermal electricity generation. It makes sense that deserts would be good spots, since effective concentration requires no interference from clouds. Incidentally, transmitting electricity over intermediate distances (across regions) is fairly efficient: typically better than 90% for distances shorter than ∼1,000 km.

![](../figures/Ch13_SolarEnergy/_page_239_Picture_7.jpeg)

[Figure](#page-238-3) [13.23](#page-238-3)

In terms of implementation, solar thermal is a small player. In 2018, only four states produced solar thermal power, 68% from California and 22% from Arizona. [Table](#page-240-2) [13.4](#page-240-2) provides some context, comparing [ST](#page-455-4) to [PV](#page-454-0) in each of the four states that have any solar thermal. For the entire U.S., less than 0.1% of electricity derives from solar thermal, and PV is about 25 times bigger on the whole. Globally, ST averages about 1.1 GW<sup>93</sup> (2016), about half in Spain and a third in the U.S.<sup>94</sup>

<span id="page-240-2"></span>

| State      | ST MW avg. | ST % elec. | PV MW avg. | PV % elec. | ST/PV % |
|------------|------------|------------|------------|------------|---------|
| California | 281        | 1.25       | 4,285      | 19.0       | 6.6     |
| Arizona    | 89         | 0.08       | 765        | 5.1        | 11.6    |
| Nevada     | 35         | 0.09       | 552        | 12.1       | 6.3     |
| Florida    | 6          | 0.002      | 326        | 1.2        | 1.8     |
| U.S. total | 410        | 0.086      | 10,565     | 2.2        | 3.9     |

## <span id="page-240-0"></span>**13.8.3 Pros and Cons of Solar Thermal**

Summarizing the pros and cons for [solar thermal](#page-455-4) [\(ST\)](#page-455-4), starting with the good aspects:

- I ST taps into a super-abundant resource—the only renewable that has such a margin;
- I ST technology is low-tech and inexpensive, using well-developed power plant technologies;
- I ST has built-in short-term storage capacity for covering evening power demands;
- I Life-cycle CO<sup>2</sup> [emissions](#page-451-2) are 20 times smaller than that of traditional fossil fuel electricity [\[68\]](#page-435-0). [\[68\]](#page-435-0): (2020), *Life Cycle GHG Emissions*

And the less great stuff:

- I ST requires direct sunlight; intolerant of clouds;
- I ST is only possible at utility-scale, requiring a power plant;
- I ST has a lower land-area efficiency than PV panels;
- I Some disruption will be imposed on the local environment/habitat.

# <span id="page-240-1"></span>**13.9 Upshot for Solar**

Hands down, Pros and cons are listed separately for [PV](#page-454-0) solar is *the only renewable resource* capable of matching our current societal energy demand. Not only can it reach 18 TW, it can exceed the mark by orders of magnitude. Finding space for panels is not a limitation. The efficiency of PV panels is perfectly respectable based on physics expectations, and beats the best that biology has done by a factor of 3–4. The efficiency is high enough that roof space tends to be more than sufficient to satisfy the demands of individual houses.

93: . . . 0.006% of global demand

94: . . . therefore not much left in the rest of the world

**Table 13.4:** Solar Thermal (ST) generation in the U.S. in 2018, compared to photovoltaic (PV); MW is megawatts.

and [ST](#page-455-4) in [Section](#page-236-0) [13.7.1](#page-236-0) and [Section](#page-240-0) [13.8.3,](#page-240-0) respectively.

Holding solar back is its intermittency<sup>[95](#page-9-9)</sup> and high up-front cost. Intermittency can be solved by battery storage, but this can double the cost and require maintenance and periodic battery replacement. Additionally—as for many of our renewable options—all of our society's demands<sup>[96](#page-9-9)</sup> are not well met by electricity generation.
  

<sup>[95](#page-9-9)</sup>: ... low capacity factor that is weather-dependent
  

<sup>[96](#page-9-9)</sup>: ... like transportation and industrial processingSizing up a PV installation is fairly straightforward. Having first determined how many kWh per day are to be produced, on average, divide this by the kWh/m<sup>2</sup>/day value for the site,[<sup>97</sup>](#page-448-0) which is essentially the [97](#page-448-0): ... either annual or monthly number of hours of full-sun[<sup>98</sup>](#page-448-0) [98](#page-448-0): 1,000 W/m<sup>2</sup> equivalent, and tends to be in the 4–6 hour ballpark. This says how many kilowatts the array should produce in full sun (peak Watts). For instance, if only 10 kWh/day are needed,[<sup>99</sup>](#page-448-0) [99](#page-448-0): ... because you are careful about energy and the region in question gets 5 kWh/m<sup>2</sup>/day, the system needs to operate at a peak power of 2 kW<sub>p</sub>, costing about \$6k to purchase and install ([grid](#page-448-0) [tied\)](#page-448-0). Inflating by 20% offsets unaccounted losses[<sup>100</sup>](#page-448-0) [100](#page-448-0): ... hot, dirty panels and conversion to better match real conditions.Solar thermal energy is another way to run a traditional steam-based power plant, using relatively low-tech mirrors and pipes to concentrate solar energy into a heat-carrying fluid that can later make steam. Effective efficiencies are relatively low,<sup>101</sup> 101: 3% of solar energy hitting the plant but on the bright side, the low-tech nature makes it fairly cheap, and the technique can accommodate some degree of thermal storage for use some hours into the evening. Anything<sup>102</sup> 102: . . . even if the efficiency is modest or starting from solar input has the potential to be a major player, given the low ∼100,000 TW scale of solar energy incident upon the earth.

## <span id="page-241-0"></span>**13.10 Problems**

- 1. If we had two monochromatic (single-wavelength) light sources—a green one at <sup>휆</sup> <sup>=</sup> <sup>0</sup>.<sup>5</sup> <sup>휇</sup>m and a near-infrared one at <sup>휆</sup> <sup>=</sup> <sup>1</sup>.<sup>0</sup> <sup>휇</sup>m each emitting photons at an energy rate of 1 W,<sup>103</sup> how does 103: Hint: recall that 1 W is 1 J/s. the number of photons emerging per second from each source compare? Is it the same number for each because both are 1 W sources, or is it a different number—and by what factor, if so?
- <span id="page-241-1"></span>2. Overhead sunlight arrives on the surface of the earth at an intensity of about 1,000 W/m<sup>2</sup> . How many photons per second strike a solar panel whose area is 1.6 square meters, if the typical wavelength is <sup>휆</sup> <sup>=</sup> <sup>0</sup>.<sup>5</sup> <sup>휇</sup>m?
- <span id="page-241-2"></span>3. Using the setup in [Problem](#page-241-1) [2,](#page-241-1) how many photons enter your pupil every second if you look directly at the sun? When doing so, your pupil restricts to a diameter of about 2 mm.
- 4. The dimmest stars we can see with our eyes are thirteen orders-ofmagnitude<sup>104</sup> 104: <sup>10</sup>−<sup>13</sup> dimmer than the intensity of the sun. Building off times of [Problem](#page-241-2) [3,](#page-241-2) how many photons enter your eye per second at this edge of detectability?

dependent

processing

97: . . . either annual or monthly

 $98: 1,000 W/m^2$ expenditures

efficiencies

area ends up as electricity

102: ...even if the efficiency is modest or
low

103: Hint: recall that 1 W is 1 J/s.

104:  $10^{-13}$  times

- <span id="page-242-0"></span>5. Warm humans at ∼300 K and glowing-hot light bulb filaments at ∼2,400 K both radiate according to [Eq.](#page-218-3) [13.3.](#page-218-3) How much more power per unit area (W/m<sup>2</sup> ) does an incandescent filament emit compared to human skin, roughly?
- 6. The outcome of [Problem](#page-242-0) [5](#page-242-0) indicates that a hot light bulb filament emits thousands of times more power per unit area than human skin. Yet both a human and a light bulb may emit a similar amount of light<sup>105</sup> 105: Humans emit in the infrared, so we —both around 100 W. Explain how both things can be true?
- 7. At what wavelength does the Wien Law say the Planck spectrum will peak for a temperature of 4,500 K? Express your answer in microns and compare to [Figure](#page-219-0) [13.1](#page-219-0) for confirmation.
- 8. Human bodies also glow by the same physics as the sun or a light bulb filament, only it is too far out in the infrared for the human eye to see. For familiar objects (and human skin) all in the neighborhood of 300 K, what is the *approximate* wavelength of peak [blackbody](#page-442-1) radiation, in microns?
- 9. We might describe the efficiency of a light bulb as the fraction of its total light output that falls within the *visible* range. If using a *thermal* source<sup>106</sup> 106: . . . like the sun or an incandescent light why would you expect it to be impossible to reach 100% efficiency at any source temperature, based on what [Figure](#page-219-0) [13.1](#page-219-0) shows?
- 10. Using a technique similar to that in the text, approximate the height and width of a rectangle that has comparable area to the spectrum for 푇 <sup>=</sup> <sup>4500</sup> K in [Figure](#page-219-0) [13.1.](#page-219-0) Compute the area of your rectangle and compare to the expectation from <sup>휎</sup>푇 4 .
- 11. What are two reasons that blue photons are disadvantaged in terms of having their energy contribute to useful current in silicon photovoltaics?
- 12. Which photons are most responsible for heating up a silicon photovoltaic panel in full sun: blue photons or infrared photons (beyond 1.1 휇m)?
- 13. If a blue photon having 3.3 [electron-volt](#page-446-0) of energy liberates an electron in silicon, whose [band gap](#page-441-0) is 1.1 eV" what fraction of the photon's energy is "kept" by the electron once it settles down from the excess?<sup>107</sup>
- 14. If a 2.5 [electron-volt](#page-446-0) photon liberates an electron from silicon with a 1.1 eV band gap, how much [kinetic energy](#page-450-3) does the emerging electron have? Express in both eV and Joules, and then determine the velocity of the electron if the electron mass is 9 × 10−<sup>31</sup> kg.
- 15. Briefly summarize the sequence of events<sup>108</sup> 108: . . . consistent with the relevant physics, that results in a

don't see it with our eyes.

*i* Note that the spectrum is spread over so many microns and we're being approximate about the temperature, so relax your answer to an easy, round number.

bulb; one that obeys [Eq.](#page-218-1) [13.4](#page-218-1)

107: The rest going into excess kinetic energy which just heats up the PV cell.

of course

successful contribution to PV current, starting with a green photon leaving the sun and ending with an electron crossing the junction.

- 16. Many people have an instinctive reaction to discount the < 20% PV panel efficiency as disappointingly low—perhaps thinking they should hold out for higher. Present a multi-point argument about why the efficiency is actually pretty good, and why in practice it is plenty good enough to be practical.
- 17. If aiming for a particular power output<sup>109</sup> from a PV array, describe 109: Make up your own number if it helps. explicitly/quantitatively how PV panel efficiency interacts with the physical size (area) of the array. For instance, what happens if the efficiency doubles or is cut in half, while keeping the same target output?
- 18. Make the connection between [Figure](#page-221-1) [13.4](#page-221-1) and [Figure](#page-224-0) [13.6](#page-224-0) by drawing a zoom-in of the bottom left corner of one of the cells in [Figure](#page-224-0) [13.6.](#page-224-0)
- 19. [Figure](#page-224-1) [13.7](#page-224-1) shows operational curves of a PV cell for different levels of illumination. If the illumination is low and the panel continues to operate at maximum power,<sup>110</sup> which changes the 110: . . . largest rectangle that fits in curve most compared to full-sun operation: the voltage or the current? Why might lower light (fewer photons) directly connect to a lower current based on the physics of PV operation?
- 20. Replicate the calculation on page [206](#page-225-0) (showing work) that starts with the surface of the sun being 5,770 K and finds that we receive 1,360 W/m<sup>2</sup> at Earth.
- 21. According to [Figure](#page-226-0) [13.8,](#page-226-0) which continent appears to have the most solar potential? How would you rate China? Do the largest populations and/or largest energy consumers in the world tend to be well-aligned to the best solar resources?
- 22. Examine [Figure](#page-226-1) [13.9](#page-226-1) to determine the insolation at the "four corners" location where Arizona, New Mexico, Utah, and Colorado touch. Just using this location as an unambiguous Express this in both kWh/m2/day and in W/m<sup>2</sup> , showing how to convert from one to the other.
- 23. What is a typical value for hours of full-sun-equivalent<sup>111</sup> of solar 111: . . . full sun meaning 1,000 <sup>W</sup>/m<sup>2</sup> exposure in the U.S. based on the map and native units in [Figure](#page-226-1) [13.9?](#page-226-1) Explain how you arrive at this.
- <span id="page-243-0"></span>24. A 30 year study by the National Renewable Energy Lab<sup>112</sup> indicates 112: . . . called the Redbook study: [\[88\]](#page-436-2) that in San Diego, a typical year delivers an annual average of 5.0 kWh/m2/day of insolation for a flat panel facing straight up. Convert this to W/m<sup>2</sup> .
- 25. The same study mentioned in [Problem](#page-243-0) [24](#page-243-0) finds that worst year in San Diego delivered an annual average of 4.7 kWh/m2/day

109: Make up your own number if it helps.

110. ... largest rectangle that fits in curve

spot on the map.

111: ...full sun meaning 1,000 W/m²

112: . . . called the Redbook study: [88]

and the best gave 5.2 kWh/m<sup>2</sup>/day for a flat horizontal panel. What, then, is the range of annual average insolation values in units of W/m<sup>2</sup> for San Diego, and what percentage variation is this, roughly (in round numbers)?<span id="page-244-0"></span>26. The study from [Problem](#page-243-0) [24](#page-243-0) finds that a flat panel facing south and tilted at various angles<sup>113</sup> 113: . . . where we use <sup>휃</sup> to represent the site relative to the horizontal produce the following annual average yields in units of kWh/m2/day:

| Angle          | Jan | Feb | Mar | Apr | May | Jun | Jul | Aug | Sep | Oct | Nov | Dec | Year |
|----------------|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|------|
| 0°             | 3.1 | 3.9 | 4.9 | 6.1 | 6.3 | 6.4 | 6.9 | 6.5 | 5.4 | 4.4 | 3.4 | 2.9 | 5.0  |
| $\theta - 15°$ | 4.1 | 4.8 | 5.6 | 6.4 | 6.3 | 6.3 | 6.8 | 6.7 | 6.0 | 5.3 | 4.5 | 3.9 | 5.6  |
| $\theta$       | 4.7 | 5.3 | 5.8 | 6.3 | 5.9 | 5.8 | 6.4 | 6.5 | 6.1 | 5.7 | 5.1 | 4.6 | 5.7  |
| $\theta + 15°$ | 5.1 | 5.5 | 5.7 | 5.9 | 5.2 | 5.1 | 5.6 | 5.9 | 5.8 | 5.8 | 5.4 | 5.0 | 5.5  |
| 90°            | 4.5 | 4.3 | 3.9 | 3.2 | 2.4 | 2.1 | 2.2 | 2.9 | 3.6 | 4.4 | 4.6 | 4.5 | 3.5  |

What tilt delivers the best yield for the year, and how much better is this (in percent) than a flat plate facing straight up? What tilt appears to result in minimal seasonal variation?

- 27. What if you adjusted the tilt of panels throughout the season to maximize yield? Reproduce the table above, but only writing in the highest number for each month.<sup>114</sup> 114: The pattern will "graph out" the tilt . What average does this track produce for the year, and how much improvement (in percent) does this represent compared to the best fixed-tilt performance?
- 28. If typical insolation is 200 W/m<sup>2</sup> , how much land area would be needed for a 15% efficient flat PV array supplying an average of 10 kW of power—which is the U.S. individual share? If arranged in a square, how large is the side-length of this array? Compare its size or area to something familiar.
- 29. If typical insolation is 200 W/m<sup>2</sup> , how much land area would be needed for a 15% efficient flat PV array supplying an average of 10,000 W for every person in the U.S. (population 330 million). If arranged in a square, how large is the side-length of this array? Draw it on top of a state of your choice, to scale.
- 30. Based on what is presented in the text,<sup>115</sup> 115: . . . also fine to bring in prior/outside why is solar power still such a minor player if it is so hugely abundant and the technology has been around for a long time? What are some of the challenges?
- 31. You look at a PV panel and mentally estimate it to measure about 0.8 m by 1.5 m. Knowing that PV panels tend to be 15–20% efficient, you guess that it is 18% efficient. How much power would you expect it to deliver in full sun (1,000 W/m<sup>2</sup> incident)?
- <span id="page-244-1"></span>32. According to the table in [Problem](#page-244-0) [26,](#page-244-0) San Diego can expect an annual average solar yield of 5.7 kWh/m2/day when the panel is tilted to the site latitude and facing south.<sup>116</sup> If a household seeks 116: . . . absent any shadows, of course to produce a modest 8 kWh per day using 16% efficient panels,

adjustments over time.

*i* This exercise provides insight into PV at a personal-scale that would cover an American's total *share* of energy demand across all sectors.

*i* This exercise provides insight into the total PV area needed to cover America's *total* energy demand across all sectors.

knowledge

116: ...absent any shadows, of course

latitude—32.<sup>7</sup> ◦ for San Diego

how large will the array need to be? Express as an area in square
meters, and in side length for a square of the same area. It is a good practice to round the final size up
a bit to make sure additional inefficiencies- 33. Using the parameters from [Problem](#page-244-1) [32,](#page-244-1) interpreting the solar yield as daily hours of peak-sun-equivalent (at solar exposure of 1 kW/m<sup>2</sup> ) what should the array size be in terms of peak Watts in order to deliver 8 kWh per day? How much would the system cost to install at \$3.00 per Wp?
- 34. One way to look at solar [payback time](#page-453-5) time is to note that an installed system will cost something like \$3,000 for each kW<sup>p</sup> (peak capacity), and that you'll produce <sup>푥</sup> kWh from that 1 kW<sup>p</sup> array if your region gets 푥 hours of full-sun-equivalent on average. Since each kWh of electricity costs something like \$0.15, it becomes straightforward to compute the value per day as \$0.15푥, and determine how long to match the \$3k investment. The result is independent of the actual array size, depending only on the cost per Wp, the solar yield at your location, and the cost of electricity. What would the payback time be, in years, if the cost is \$3/Wp, the yield is 6 hours per day of full-sun-equivalent, and electricity in your region costs \$0.15/kWh?
- 35. From [Table](#page-236-3) [13.3,](#page-236-3) compute the [capacity factors](#page-443-0) for the countries listed, and for the whole world, based on average vs. installed power. What is a characteristic range of numbers, and why<sup>118</sup> 118: Hint: a large part is insolation vs. overis it so low? Which country does the best, and which does the worst? What clues does [Figure](#page-226-0) [13.8](#page-226-0) offer as an explanation?
- 36. How much power would a large window measuring 2 m wide and 1.5 m tall admit if the sun were shining straight<sup>119</sup> 119: . . . e.g., what is the most one might into the window from a cloudless sky? How many [kilowatt-hours](#page-450-2) does this translate to over a four hour period, and how much is it worth monetarily compared to electricity at \$0.15/kWh?
- 37. Solar photovoltaics are practical for individual homes, but solar thermal is only to be found in large utility-scale installations. What is the practical reason why we should not expect solar thermal installations on peoples' rooftops for electricity generation?
- 38. Solar thermal has a fairly low efficiency in terms of land area of about 3%, compared to 15–20% for PV. Many would shake their heads and say that's too low to be of any use. What is the counter-argument that it may be fine?

a bit to make sure additional inefficiencies do not prevent reaching the goal.

<sup>117</sup> 117: . . . consistent with the first sentence

head sun.

expect for direct sun?