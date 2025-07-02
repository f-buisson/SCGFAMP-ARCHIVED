# FAQ – SCGFAMP (EN)

---

### "Air intake from the atmosphere", but it's an intake into a pressurized air chamber.

It's an intake into a partial vacuum air chamber (between 0.5 and 0.7 bar). Yes, this requires energy at the start to create this imbalance.

---

### "The magnets that are supposed to guide the 'rigid hollow body' are 'magic magnets' that act on the body when you want and no longer affect it when you don’t want them to. If the magnet is strong enough to pull the body through a spring hatch and to the side until it floats, it will always attract the body and keep it stuck."

I imagined, for the bottom hatch for example, a magnetic force that helps with the hatch passage. The mass undergoes gravity, so it arrives with weight and speed on the hatch and must open it while pushing back the water at the moment of opening because the water acts as resistance below this hatch. So to allow this, I added a magnet to gain enough force so that:

**F_air + (m × v) + F_magnet > F_water + F_spring + F_kickback + F_buffer_chamber**

- F_air: Air column pressure × hatch surface
- (m × v): Impulse of the mass (weight × velocity at the moment of contact)
- F_magnet: Magnetic attraction force acting only on the mass
- F_water: Dynamic resistance of water (almost instantaneous)
- F_buffer_chamber: pressure from the buffer chamber (which increases during lower hatch opening and decreases when the hatch closes or when the weight changes to the upper hatch column)
- F_spring: Spring force keeping the hatch closed
- F_kickback: Force to counter if the magnet is mechanically moved

And for it to work, F_magnet must be < buoyancy after immersion in water.

Either by having a weak magnet, or by controlling the attraction distance (when the hatch opens, move the magnet mechanically during passage to control its strength)

And for the upper hatch:

**F_water + F_magnet + F_buffer_chamber > F_air + F_spring + F_kickback**

- Air being compressible, it generates moderate resistance
- Water pressure (incompressible) plays a key role
- Archimedes’ thrust must be sufficient to offset the overall resistance
- And F_magnet must be < gravitational force acting on the mass

---

### "How do you get energy out of this?"

For now, I don’t extract any energy, I’m trying to see if it can cycle a few loops, find the problems and fix them, then I’ll add a way to recover weak energy in a non-critical point (example: if the upper hatch can handle a few newtons of extra resistance, I add a system there)

---

### "How do air and water return to their respective columns? Because with each hatch opening a part of the air and water switches columns."

I’ll try to explain how I envisioned the transfer of air and water in this system.

When a hatch opens, air rushes into the water column, yes, and it rises to the top of the water column where a purge valve is installed and ejects that air outside the system. This process creates a vacuum at the top of the water column once the air is gone.

At the same time as air goes into the water column, the water goes into the air column. Which means water accumulates at the bottom of the air column.

With the help of:
- air entering that column to balance internal pressure (air enters because air was ejected by the purge valve, so there’s less air in the system),
- the weight falling cyclically into the air column,
- and the vacuum created in the water column,

...this can provide the energy needed to push the water back through a one-way hatch (air impulse leak ejector) into its original column.

That’s how I saw the movement of air and water in this system.

---

If something is wrong or misunderstood on my part, I’m open to any criticism to move forward.