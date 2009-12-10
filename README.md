# Age of War

A top down combat game where you fight waves of an enemy team in an arena full of obstacles. Made for a GameMaker community event.

<p>
  <img src="docs/screenshots/screenshot-1.png" width="306" alt="Gameplay">
</p>


## How to play

Download from Releases and run it.

Move with WASD and aim with the mouse. Keys 1, 2 and 3 switch weapons.

| Key | Weapon |
|---|---|
| 1 | Pistol (50 damage) |
| 2 | Machine gun (10 damage) |
| 3 | Grenade |

Remaining lives, kills and enemies left are shown in the window title bar.


## How it works

The enemy unit's mortar combines a trail effect with a scattered explosion. While the shell is in the air, an alarm keeps dropping shadow objects behind it to leave a trail. Each shadow uses its own alarm to cut `image_alpha` by 0.5 until it drops below 0 and removes itself. On impact it creates one explosion at the landing point, then scatters five more at offsets picked with `choose(20,25,30,35)`, so every blast looks a little different.


## Files

| Path | Contents |
|---|---|
| `source/age-of-war.gmk` | Original project file |
| `source/split/` | Text tree produced by GmkSplitter |
| `docs/screenshots/` | Screenshots |
| Releases | Distributed build |


## License

CC BY-NC-ND 4.0. Unmodified copies may be shared for noncommercial purposes with attribution. Modified versions and commercial use are not allowed. Bundled libraries, graphics, sounds, and maps made by other people keep their own rights. See [LICENSE](LICENSE).
