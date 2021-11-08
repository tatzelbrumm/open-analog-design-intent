# open-analog-design-intent
Some notes to prepare a zoom with Mohamed Kassem

## Analog design engineer vs. software engineer mindset

### Software engineer

If in doubt, add an abstraction/virtualization layer

[***You can't argue with a root shell***](https://medium.com/@maradydd/when-nerds-collide-31895b01e68c#34a1)  
Software engineers have a constructivist, mathematician's mind set:

* unambiguous axioms
* programs are built like mathematical proofs

The root shell is **ground truth** for everything software designers build on top of it.

### Analog engineer

Every component/state variable is ***noisy***

[***You can't argue with a root shell***](https://medium.com/@maradydd/when-nerds-collide-31895b01e68c#34a1)  
A root shell is an abstraction based on the fiction of noiseless digital state variables. 
It is ***way*** too detached from  
**ground truth**: noisy, non-ideal **physical** devices.

For a successful analog design, **minimize** the number of state variables, because every added variable adds noise and distortion.

***Analog designers think in (sloppy) analogies***

#### Sloppy analogy: [Kolmogorov complexity](https://en.wikipedia.org/wiki/Kolmogorov_complexity)

[Kolmogorov complexity](https://en.wikipedia.org/wiki/Kolmogorov_complexity) is [defined](https://en.wikipedia.org/wiki/Kolmogorov_complexity#Definition) as:

> the complexity of a string is the length of the shortest possible description of the string in some fixed universal description language

Digital or software designers consider something like a root shell (or other description language they build) as fixed:  
you don't *Need To Know* what lies underneath the abstraction.

Analog designers can't afford ignoring virtualization and abstraction layers between a level of abstraction and physical devices:  
**Every abstraction or virtualization layer adds noise and distortion**

So, for an analog designer, a sloppy analogy of 

**Kolmogorov complexity (sloppy analog version)**

* The Kolmogorov complexity of a tool chain is the length of the sum of all descriptions (i.e., the number of manual pages) of the tools necessary to produce a tapeout ready design.
* If the documentation is incomplete, the Kolmogorov complexity also includes the length of the informal notes in forums like stackoverflow, slack, ... to fill the missing parts in the documentation.
* If different people contribute different tools, the Kolmogorov complexity also includes the specifications of any and all APIs between these tools.
* If different contributors make inconsistent implicit assumptions, the Kolmogorov complexity also includes all the communication necessary to resolve these inconsistencies.
* If different contributors are too busy to respond to any rando's obnoxious questions, the Kolmogorov complexity also includes whatever social engineering (like building reputation or aqcuiring formal credentials) is necessary that the contributors will actually listen to you.
* If the solutions of incomplete or inconsistent documentation of tools in the toolchain are to be found in discussion forums, the Kolmogorov complexity also includes whatever research is necessary to assess the quality of the tentative solutions or workarounds presented. Discussion forums tend to have a very bad SNDR: 
  * for every actual solution, there are 
  * about 5 solutions that almost work, 
  * 15 solutions that only kind of work for the presenter of the solution, and 
  * 40 wild guesses.

