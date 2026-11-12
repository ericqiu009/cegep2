# Module 8: Energy and Conservation

**Source:** [Lecture slides](../source/08_-_Energy.pdf) · Knight, *Physics for Scientists and Engineers*, 5th ed., §§9.2, 10.2–10.4, 10.6–10.7

## Knowledge map

```text
Conservative work → potential energy → mechanical energy (K + U)
Friction → thermal energy           External work → change in system energy
                         ↓
       Choose system boundary and apply energy equation
```

## Guiding questions

- How does conservative work relate to potential energy?
- Which energy equation fits the system and forces?
- When is mechanical energy conserved?

## Core ideas and equations

| Quantity | Meaning | Key relation |
|---|---|---|
| Kinetic energy | Energy of motion | $`K=\frac12 mv^2`$ |
| Gravitational potential | Object–Earth configuration near Earth's surface | $`U_G=mgy`$; $`\Delta U_G=mg(y_f-y_i)`$ |
| Spring potential | Spring's stretch or compression from equilibrium | $`U_{sp}=\frac12 k(\Delta s)^2`$ |
| Thermal energy from sliding friction | Mechanical energy transferred to thermal energy | $`\Delta E_{th}=f_k d=\mu_k N d`$ |
| Mechanical energy | Kinetic plus potential energy | $`E_{mech}=K+U_G+U_{sp}`$ |

For conservative forces, $`W_c=-\Delta U`$. The total energy equation is:

$$\Delta K+\Delta U_G+\Delta U_{sp}+\Delta E_{th}=W_{ext}$$

Here, $`W_{ext}`$ is work done on the system by forces outside its boundary. For gravity to be represented by $`U_G`$, include Earth in the system. Do not count the same force as both potential energy and external work.

> [!IMPORTANT]
> **Choose the system first.** An isolated system has $`W_{ext}=0`$, so its total energy is conserved. Mechanical energy alone is conserved only when there is no energy transferred into thermal energy (or other internal forms).

### Which equation should I use?

| Situation | Equation |
|---|---|
| Isolated, no friction | $`K_i+U_i=K_f+U_f`$ |
| Isolated, kinetic friction inside system | $`K_i+U_i=K_f+U_f+f_kd`$ |
| External work on system | $`K_i+U_i+W_{ext}=K_f+U_f+\Delta E_{th}`$ |

In the last two rows, include only the potential-energy terms relevant to the problem. Friction can be found from a free-body diagram: on an incline, $`N=mg\cos\theta`$ when there are no other perpendicular forces.

## Potential energy: details to remember

- **Gravity:** The zero height is arbitrary. Changing it shifts $`U_G`$, but not $`\Delta U_G`$ or a physical prediction.
- **Spring:** The zero is at the spring's equilibrium length, where $`\Delta s=0`$. Stretch and compression both give nonnegative $`U_{sp}`$.
- For springs, calculate the change as $`\Delta U_{sp}=\frac12k[(\Delta s_f)^2-(\Delta s_i)^2]`$; do not square the change in length.
- The slides say the calculus derivation of spring work and equivalent springs are outside this mechanics module.

## Problem-solving map

```text
Set system boundary → Mark initial and final states → Identify K, U, friction, and external work
                                                              ↓
                                      Choose the matching energy equation → Solve for unknown
```

Energy is useful when time is not requested and forces or acceleration vary along a path. For friction, determine the normal force and sliding distance; use the geometry of the path where needed.

## Examples and what they demonstrate

| Lecture example and context | Energy setup | Result |
|---|---|---:|
| **Watermelon:** dropped 11 m above street into a 3 m pothole. The 14 m total drop sets the speed; the street is just a convenient reference. | $`mg(14)=\frac12mv_f^2`$ | $`16.6\,\mathrm{m/s}`$ |
| **Sled, frictionless:** starts at 2.0 m/s and descends 5.0 m. Gravitational potential becomes kinetic energy. | $`v_f=\sqrt{v_i^2+2gh}`$ | $`10.1\,\mathrm{m/s}`$ |
| **Sled, with friction:** same hill, $`\mu_k=0.1`$, $`\theta=15^\circ`$. Some mechanical energy becomes thermal energy over the slope distance $`h/\sin\theta`$. | Include $`\mu_kmg\cos\theta\,(h/\sin\theta)`$ as thermal energy. | **Given data yield about 8.09 m/s; slide reports 9.92 m/s.** |
| **Spring lab:** a 0.500 kg mass stretches the spring 3.5 cm while hanging, then compresses it 2.7 cm on a frictionless table. Static equilibrium gives $`k=mg/\Delta y`$; then kinetic energy becomes spring energy. | $`\frac12mv^2=\frac12k(\Delta x)^2`$ | $`0.45\,\mathrm{m/s}`$ |
| **Jet and arrestor cable:** landing kinetic energy is absorbed by spring stretch and deck friction. | $`\frac12mv_i^2=\frac12kx^2+\mu_kmgd`$ | $`62.4\,\mathrm{m/s}`$ (121 knots) |
| **Skier:** drops 20.0 m on a frictionless slope, then stops on rough horizontal snow. Initial gravitational energy becomes thermal energy from friction. | $`mgh=\mu_kmgd`$ | $`90.9\,\mathrm{m}`$ |

> [!WARNING]
> **Slide 16 has an apparent answer error.** Substituting $`\mu_k=0.1`$ into the stated incline data gives $`v_f=\sqrt{v_i^2+2gh(1-\mu_k\cot\theta)}\approx8.09\,\mathrm{m/s}`$, not the slide's 9.92 m/s. Show the setup and check with your instructor if the expected answer matters.

## Connections to other modules

- [Module 7: Work](./07_-_Work.md): $`\Delta K=W_{tot}`$; replacing conservative work with $`-\Delta U`$ leads to the energy equation above.
- [Modules 5–6: Newton's laws and friction](./05_-_Newtons_Laws.md) and [friction and dynamics](./06_-_Friction_and_Dynamics.md): use force diagrams and $`f_k=\mu_kN`$ to find friction's thermal-energy contribution.
- Kinematics: energy can find speed without solving for time; for free fall it agrees with $`v_f^2=v_i^2+2g(y_i-y_f)`$.
- Momentum and collisions ([Module 9](./09_-_Momentum.md)): momentum conservation and mechanical-energy conservation are different rules. Isolated collisions conserve momentum; kinetic energy is conserved only in elastic collisions.
- Later electricity and magnetism: conservative electric forces also have potential energy.

## Likely exam questions

1. A dropped object falls through a specified height. Find its final speed using energy conservation.
2. Compare two choices of zero height and explain why $`\Delta U_G`$ is unchanged.
3. Find an object's speed after descending a rough incline, including the frictional energy loss.
4. Find a spring constant from a hanging mass, then use spring energy to find a moving mass's speed or maximum compression.
5. Choose a system boundary and write the energy equation without double-counting gravity or friction.
6. Explain the difference between conservation of total energy and conservation of mechanical energy.
