# Age of War

[한국어](README.ko.md)

A top-down combat game where you fight waves of an enemy team in an arena full of obstacles. Made for a GameMaker community event.

<p>
  <img src="docs/screenshots/screenshot-1.png" width="306" alt="Gameplay">
</p>


## How to play

Download it from Releases and run it.

Move with WASD and aim with the mouse. Keys 1, 2 and 3 switch weapons.

| Key | Weapon |
|---|---|
| 1 | Pistol (50 damage) |
| 2 | Machine gun (10 damage) |
| 3 | Grenade |

The window title bar shows remaining lives, kills, and enemies left.


## How it works

The enemy unit's mortar combines a trail effect with explosion effects. While the shell is in the air, an alarm keeps dropping shadow objects behind it to leave a trail. Each dropped shadow uses its own alarm to lower `image_alpha` by 0.5 at a time and removes itself once the value goes below 0. On impact it creates one explosion at the landing point, then scatters five more at offsets picked with `choose(20,25,30,35)`, so the blast looks different every time.


## Files

| Path | Contents |
|---|---|
| `source/age-of-war.gmk` | Original project file |
| `source/split/` | Text tree produced by GmkSplitter |
| `docs/screenshots/` | Screenshots |
| Releases | Distributed build |


## License

CC BY-NC-ND 4.0. Unmodified copies may be shared for noncommercial purposes with attribution. Distributing modified versions and commercial use are not allowed. Bundled libraries, graphics, sounds, and maps made by other people keep their own rights. See [LICENSE](LICENSE).
