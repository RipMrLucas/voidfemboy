# Changelog

English | [简体中文](https://github.com/Ripmrlucas/voidfemboy/blob/main/CHANGELOG_CN.md)

All notable changes to VoidFemboy. Versions before 0.1.0 were internal alphas;
the first public release is **0.1.0**.

## 0.2.0-alpha — tail, headphones & the station remap

Two supported lines: 1.20.1 (wider mod ecosystem) and 1.21.1. Same features,
same jar name — pick the one matching your game.

### New cosmetics
- **Femboi Tail** (Cute Menu cosmetic slot): physics-swayed chained tail with a
  white tip shell that stays white under any dye. The outfit's baked-in tail
  hides while one is worn, so they never double up.
- **Cat-Ear Headphones** (Cute Menu cosmetic slot): chunky cups, head-following
  band, two-step ears. Band, cups and ear bases dye; ear tips stay pale.
  Hidden in first person (they filled the screen).
- **Standalone hoodie** rebuilt (r2-1 design): kangaroo pocket, hood drape,
  sleeve hearts, stripes and cuffs, own texture. Sleeves hide while arm
  warmers are worn.

### Cute Station
- 7 body-grouped wells (headband / hoodie / warmers / thigh-highs / paw
  booties / tail / headphones) with leader traces to the doll.
- **Dye All** paints every worn piece in one click (armor included).
- The doll is item-driven: regions follow the piece covering them (thigh-highs
  -> thigh, booties -> paws, tops -> torso, dresses -> tiers), empty regions
  show hollow, and the chest well names itself Hoodie / Dress / Hoodie-Dress.

### Outfit logic
- The standalone **dress moved to the chest slot** (legs = thigh-highs only).
  Skirt panels render from exactly one piece; removing thigh-highs removes
  them for real now. Worlds with a dress still in legs: take it out once and
  put it in the chest well.
- Set bonus counts a dress top.

### Hoodie pocket
- The hoodie and hoodie-dress carry a **45-slot pocket** (9x5, keybind `N`
  toggles open/shut while worn). Contents ride the item through closing,
  relogging, unequipping and death.
- Retired the med/low detail variants entirely (the GPU handles full detail);
  `config/voidfemboy-detail.txt` is no longer read and can be deleted.

### Fixes
- Dye-all no longer undyes tail/ears; armor tints sync on dye-all.
- Title screen stops yanking Options/quit flows back to itself.
- Dress skirt visible again after the chest move (ring re-root).
- Retired the med/low detail variants entirely (the GPU handles full detail);
  `config/voidfemboy-detail.txt` is no longer read and can be deleted.

## 0.1.0 — first public release

The culmination of the alpha series. Highlights:

### Armor & cosmetics
- True-3D GeckoLib femboi wardrobe: cat-ear headband (helmet), hoodie-dress with
  a physics-driven pleated skirt + cat tail (chestplate), striped thigh-highs
  (leggings), and fluffy kitty-paw booties (boots).
- Paw booties are **silent** — no footstep sound.
- Full femboi set grants the cosmetic **Confidence** effect (custom icon).
- Void armor: galaxy-plated set stronger than diamond, emissive scrolling galaxy
  texture, Regeneration II + Strength II set bonus. Tuned so it doesn't over-glow
  under shaders.

### Dyeing
- **Cute Station** paper-doll dyeing block with a 16-color **rainbow** dye rack.
- Recolor per body part; **Clear** reverts to default; **Striped/Solid** toggle.
- Toggle stripes on the **held** piece with a keybind (default `N`) — no station
  needed.
- Dyeable white accents stay white on cool dyes; warm dyes (red/orange/yellow)
  get black stripes like real striped socks.
- Femboi item tooltips show the current color + striped/solid mode.

### UI
- Galaxy animated **title screen** with parallax hearts and sparkles.
- **Void Codex** recipe browser in the pause menu, over the galaxy backdrop.
- Cute Station and Codex scale sensibly on 1080p/4K.
- Pink-themed buttons throughout.

### World & recipes
- Void ore + Prism ore, void crystal → void ingot smelting.
- Crafting recipes for the whole wardrobe, void set, and the Cute Station.

### Secrets
- A little something for anyone who stares too long. :3

### Compatibility
- Minecraft 1.21.1–1.21.11, Fabric. Optional integration with First-person Model
  and JEI.
