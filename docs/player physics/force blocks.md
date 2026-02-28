## Force Blocks

The acceleration in Vels from a force block without relative or range turned on can be calculated with the following equation.
$$
\Large
F=\tfrac{\operatorname{round}\left(\left(\tfrac{\cos(\theta_1)9x_1 \ + \ \cos(\theta_2)9x_2\ ...\ + \ \cos(\theta_n)9x_n}{40}\right) \ \cdot \ 1000 \right)}{1000}+A
\\
\text{Where \(x\) is the value of the force block, \(A\) is the acceleration from gravity*,}
\\
\text{\(n\) is the amount of force blocks that are being stacked, and \(\theta\) is the angle of rotation of the force block}
\\
\\
\text{*(refer to desmos graph in "Gamemodes" section)}
$$
The acceleration ends once the player is no longer touching the force block and it returns back to \(A\). If the player is touching two or more force blocks with no ForceIDs or different ForceIDs at once, then their accelerations get added up together, which is all added to the acceleration \(A\) as usual. However, if a force block causes the velocity to go past the maximum velocity, then the maximum velocity is temporarily increased by \(F\). Another way of saying that is the velocity is set to \(F\) rather than increase by \(F\) every tick. The force is also affected depending on the rotation of the force block.

The equation above can be simplified if there is no force block stacking.
$$
\Large
F=\tfrac{\operatorname{round}(\cos(\theta) \ \cdot \ 225x)}{1000}+A
$$
