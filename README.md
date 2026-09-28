# Stasi's Minecraft Mods

This folder holds the ready-to-play release of **Stasi's Minecraft Mods**, a pack of home-made mods for
**Minecraft Java Edition 26.3** on **[Fabric](https://fabricmc.net/)**. You'll find dinosaurs in the forests, cities
full of drivable cars and police officers, real guns with iron sights, a drivable tank, a rocket to the Moon full of
aliens, a gate to the Underworld, cyclops caves, Spartan graveyards, giant mutant monsters and a slime bucket that lets
you ooze through walls.

**Release: 1.14.0** (`stasi-mods-1.14.0.zip`)

---

## What's in pack 1.14.0

| Mod | Version | In short |
|-----|---------|----------|
| **Cities** | `cities-1.8.0` | Villages become big cities with streets, shops and shopkeepers, drivable cars, police stations and **police officers** who shoot monsters and dinosaurs. You can join the police for emeralds. New worlds start in a city. |
| **Dinosaurs** | `dinos-1.6.0` | Nine dinosaurs: T-Rex, velociraptors, spinosaurus, dilophosaurus, pteranodons, triceratops, brachiosaurus, stegosaurus and ankylosaurus. **Every dinosaur attacks you on sight.** |
| **Underworld** | `underworld-1.15.0` | A blackstone-and-lava dimension ruled by the Demon Lord, plus the guns: M16, AK-47, Glock 19, Revolver, Uzi, pump Shotgun, Sniper Rifle, RPG-7 and grenades, with SWAT armor. |
| **Space** | `space-1.4.0` | A rocket ship to the Moon (low gravity, no air), alien armies, the Alien Citadel and its Lord, space weapons, space suits and nano armor. |
| **Mutants** | `mutants-1.0.0` | Rare giant night monsters (Mutant Zombie, Creeper, Skeleton and Spider) that drop powerful trophies. |
| **Warfare** | `warfare-1.0.0` | A drivable tank that fires explosive shells. |
| **Cyclops** | `cyclops-1.4.1` | A 300-HP cyclops that roams at night, plus Cyclops Caves full of over-powered loot. |
| **Spartoi Hoplites** | `hoplites-1.2.1` | Bronze-armored skeleton hoplites, the Dragon Tooth that summons them, and Spartan Graveyards. |
| **Slime Bucket** | `slime-1.0.0` | Drink it to ooze through walls up to three blocks thick for 60 seconds. |
| **Ruby** | `ruby-1.1.0` | A ruby gem, the sample mod the whole pack grew from. |
| Fabric API | `0.161.0+26.3` | Required library. Keep it in the `mods` folder. |

**Optional "realistic" look.** This is the look Stasi plays with:
[Sodium](https://modrinth.com/mod/sodium), [Iris](https://modrinth.com/mod/iris) and the
[Complementary Unbound](https://modrinth.com/shader/complementary-unbound) shader pack. The install scripts in the zip
download them from Modrinth and switch the shaders on. They aren't re-hosted here.

Every mod works on its own, so you can leave out any you don't want. Only Fabric API is needed by all of them.

### New in 1.14.0

- **Police officers guard every city.** Two are on duty in each police station, and about six patrol the streets near
  you. They shoot hostile mobs and every kind of dinosaur, never fire through players or villagers, and help each other.
  There's a Police Officer spawn egg. If you're in the police, killing an officer gets you fired.
- **Every dinosaur is hostile.** They attack you and police officers on sight. Only the hunters also chase animals.

### New in 1.13.0

- **Iron sights on every gun except the sniper.** Right-click brings the gun up to your eye, so you look through the
  rear sight at the front sight on your target, and the crosshair disappears while you aim.
  - Pistols (Glock, Uzi, Revolver) and the AK-47 and RPG-7: a notch and a post.
  - M16: a peep ring and a post.
  - Shotgun: a ring and a bead.
  - Sniper rifle: still uses its scope.
- **Wider, more detailed guns**, with pins, rivets, ejection ports, sight dots, cylinder flutes, vent ribs and more.

---

## Requirements

- **Minecraft Java Edition.** Bedrock, Windows 10/11 Edition and console versions won't work.
- Minecraft version **26.3 exactly**. The mods won't load on any other version.
- **Fabric Loader 0.19.5 or newer** for 26.3. The steps below show how to install it.
- For the shaders: a reasonably modern graphics card. You can switch them off at any time.

---

## Installation

### With the official Minecraft Launcher

**Step 1. Run Minecraft 26.3 once.**
Open the Minecraft Launcher and go to **Installations**, then **New installation**. Pick version **26.3**, save and press
**Play**. Quit once you reach the title screen.

**Step 2. Install Fabric.**
Download the installer from <https://fabricmc.net/use/installer/>.
- **Windows:** use the `.exe`.
- **Mac / Linux:** use the universal `.jar` and double-click it. If your Mac says it can't open the file, install Java
  from <https://adoptium.net> and try again.

Close the Minecraft Launcher, then set the installer to:
- the **Client** tab
- Minecraft Version: **26.3**
- Loader Version: **0.19.5** or newer
- **Create profile** ticked

Press **Install**.

**Step 3. Copy in the mods.**
Unzip **`stasi-mods-1.14.0.zip`** from this folder (unzip the `.zip`, **not** the `.jar` files inside). Then use either
the install script or copy the files by hand.

*With the install script.* It copies the mods, removes older versions of them, and downloads and switches on the
shaders.
- **Windows:** double-click `install.bat`.
- **Mac:** open **Terminal**, type `bash` followed by a space, drag `install.sh` onto the Terminal window and press
  **Enter**.
- **Linux:** run `bash install.sh` from the unzipped folder.

The scripts also work without the shaders (`install.sh --no-shaders` or `install.ps1 -NoShaders`). If your Minecraft
folder is somewhere unusual, give its path, e.g. `bash install.sh ~/Games/minecraft`.

*By hand.* Copy **every** `.jar` from the zip's `mods` folder into your Minecraft `mods` folder. If there's no `mods`
folder, create it.

| System | Minecraft folder | How to open it |
|--------|------------------|----------------|
| Windows | `%appdata%\.minecraft` | Press `Win+R`, paste the path, press Enter |
| Mac | `~/Library/Application Support/minecraft` | In Finder press `Cmd+Shift+G`, paste the path, press Enter |
| Linux | `~/.minecraft` | Open it in your file manager |

For the shaders by hand, follow the links in the zip's `INSTALL.txt`:
1. Put the Sodium and Iris `.jar` files in `mods`.
2. Put the Complementary Unbound `.zip` (don't unzip it) in a `shaderpacks` folder next to `mods`.
3. In game, go to **Options**, then **Video Settings**, then **Shader Packs**. Pick **ComplementaryUnbound_r5.9.3** and
   press **Apply**.

**Step 4. Play.**
In the Minecraft Launcher, pick the **`fabric-loader-26.3`** profile next to the green **Play** button and press
**Play**.

---

## Getting started in game

- **Where things are:** every mod's items are in the Creative inventory, in the **Combat**, **Tools & Utilities**,
  **Ingredients** and **Spawn Eggs** tabs. Everything except spawn eggs can also be crafted.
- **Cities:** make a **new world** to start in a city (older worlds keep their spawn point). To find another city, use
  `/locate structure cities:city`.
- **Join the police:** right-click the **Police Desk** (the gold-badge counter in every police station). You get a Glock,
  an Uzi, bullets and police armor. Killing monsters and dinosaurs inside a city pays emeralds, which you spend at the
  shops. `/job` shows your kills and pay.
- **Guns:**

  | Action | Control |
  |--------|---------|
  | Aim mode on / off | **Right-click** |
  | Shoot, from the hip or aimed | **Left-click** |
  | Full auto (M16, AK-47, Uzi) | **Hold left-click** |
  | Reload | **R** |

  Left-click never breaks blocks while you hold a gun.
- **Cars:**

  | Action | Control |
  |--------|---------|
  | Get in | **Right-click** the car |
  | Gas / brake / reverse | **W** / **S** |
  | Steer | **A** / **D** |
  | Horn | **Jump** |
  | Get out | **Sneak** |
  | Pick the car up | **Sneak** and punch it |

- **The Underworld:** build a **bone block** frame shaped like a nether portal and light it with **flint and steel**.
- **The Moon:** place the rocket and right-click it to board. **Hold jump** to climb past y = 250. Wear a full space suit
  or nano armor up there, or you'll run out of air.
- **Tank:**

  | Action | Control |
  |--------|---------|
  | Get in | **Right-click** the tank |
  | Drive | **W** / **S** |
  | Turn | **A** / **D** |
  | Aim | Look where you want to shoot |
  | Fire | **Hold left-click** |
  | Get out | **Sneak** |

- **Watch out:** dinosaurs now attack on sight, anywhere, including in worlds you already had.

---

## Updating

1. Get the newest `stasi-mods-<version>.zip`.
2. Install it the same way you did the first time. Re-running the install script removes the old jars for you.

**Never keep two versions of the same mod** in the `mods` folder (for example `cities-1.7.0.jar` and
`cities-1.8.0.jar`). The game will crash on launch.

## Uninstalling

Delete the mod's `.jar` from the `mods` folder. If a world used that mod's blocks or items, they turn into air, so
**back up your `saves` folder first**. When you next open that world, Minecraft shows a *"Missing content detected"*
warning once. Choose *"I Know What I'm Doing!"*.

---

## Troubleshooting

| Problem | What to check |
|---------|---------------|
| Game crashes on launch | Look for **two versions of the same mod** in `mods`, and for mods made for other Minecraft versions. Make sure you started the **`fabric-loader-26.3`** profile, not plain `26.3`, and that **Fabric API** is in `mods`. |
| Purple/black squares or missing items | A jar is damaged or was unzipped. Download it again and copy the `.jar` as it is. |
| No dinosaurs | Stand in a forest, plains, savanna, jungle or on a mountain for a minute. They spawn 24–64 blocks away. Check that the `spawn_mobs` game rule is on. Inside cities there are far fewer. |
| No aliens or mutants | They're monsters, so they don't appear on **Peaceful** or with `spawn_monsters` off. |
| No police officers | They patrol only **inside cities**, near you, at street level. Every police station also has two on duty. |
| No shaders / not "realistic" | You need `sodium-…` and `iris-…` in `mods` and `ComplementaryUnbound_r5.9.3.zip` in `shaderpacks`. Then go to **Options**, **Video Settings**, **Shader Packs**, pick it and press **Apply**. |
| Game is slow | Turn shaders off in **Shader Packs**, or lower render distance. |
| Still stuck | Send the newest file from the `crash-reports` folder (next to `mods`), or `logs/latest.log`, to Stasi. |

---

## License

MIT. Minecraft is a trademark of Mojang/Microsoft. This is an unofficial fan project.
