# Rules

* Keep it to lore, with exceptions.
* Custom Vehicles/BA/'Mech designs can only be from MegaMekLab or from Sarna.net.
* Tiles are considered 1.55 meters. Don't ask, it took a while. A long while.
* @Lord Rod, Lord of Rods [COM] for the vehicle speed rework, I approximated car width in meters as `0.4 * (tiles width) + 0.5<= 5`, or `2.5 + ( tiles - 5 ) * 0.15m` for larger vehicles.
* Damage is calculated using MegamekLab's damage values, times `(40/.18)`.
 `x * (40/.18)`, with x being the damage value.
* `On a standard mapsheet the hex size as originally printed is approximately 1.25 inches and depicts terrain 30 meters (roughly 100 feet) across.` And since each tile is 1.55 meters, each hex is 19 tiles.

Example:
> RAC/2 has a range of 18. 
> 
> `19 * 18 = 342`
> 
> Thus the RAC/2 has a range of 342 tiles.

* Dispersion is the weapon's BV divided by 1.55, with a limit of 200 for rifles and stuff like that, and shotguns having a limit of 500. Rockets have a limit of 150, with Artemis IV taking 100 off. Lasers have a max of 45.

