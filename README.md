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
