<div align="center">
  <img height="150" src="https://media.tenor.com/B1_FyTTUcxkAAAAi/clown-ss14.gif"  />
</div>

###

<div align="center">
  <img src="https://station14.ru/images/8/8f/%D0%9A%D0%BB%D0%BE%D1%83%D0%BD.png" height="25" alt="3"  />
  <img src="https://station14.ru/images/8/8f/%D0%9A%D0%BB%D0%BE%D1%83%D0%BD.png" height="25" alt="4"  />
  <img src="https://station14.ru/images/8/8f/%D0%9A%D0%BB%D0%BE%D1%83%D0%BD.png" height="25" alt="5"  />
  <img src="https://station14.ru/images/8/8f/%D0%9A%D0%BB%D0%BE%D1%83%D0%BD.png" height="25" alt="6"  />
  <img src="https://station14.ru/images/8/8f/%D0%9A%D0%BB%D0%BE%D1%83%D0%BD.png" height="25" alt="7"  />
  <img src="https://station14.ru/images/8/8f/%D0%9A%D0%BB%D0%BE%D1%83%D0%BD.png" height="25" alt="8"  />
  <img src="https://station14.ru/images/8/8f/%D0%9A%D0%BB%D0%BE%D1%83%D0%BD.png" height="25" alt="9"  />
  <img src="https://station14.ru/images/8/8f/%D0%9A%D0%BB%D0%BE%D1%83%D0%BD.png" height="25" alt="10"  />
  <img src="https://station14.ru/images/8/8f/%D0%9A%D0%BB%D0%BE%D1%83%D0%BD.png" height="25" alt="11"  />
  <img src="https://station14.ru/images/8/8f/%D0%9A%D0%BB%D0%BE%D1%83%D0%BD.png" height="25" alt="12"  />
</div>

###


<h1 align="center">dashnatn</h1>

###
```js
 type: entity
  name: corrupted corgi
  parent: [ MobCorgi, MobCombat ]
  id: MobCorgiNarsi
  description: Ian! No!
  components:
  - type: Sprite
    drawdepth: Mobs
    sprite: Mobs/Pets/corgi.rsi
    layers:
    - map: ["enum.DamageStateVisualLayers.Base"]
      state: narsian
  - type: DamageStateVisuals
    states:
      Alive:
        Base: narsian
      Critical:
        Base: narsian_dead
      Dead:
        Base: narsian_dead
  - type: MeleeWeapon
    soundHit:
        path: /Audio/Effects/bite.ogg
    angle: 0
    animation: WeaponArcBite
    damage:
      types:
        Piercing: 5
        Slash: 5
  - type: InputMover
  - type: MobMover
  - type: HTN
    rootTask:
      task: SimpleHostileCompound
  - type: NpcFactionMember
    factions:
    - SimpleHostile
  - type: InteractionPopup
    successChance: 0
    interactSuccessString: petting-success-corrupted-corgi
    interactFailureString: petting-failure-corrupted-corgi
  - type: Grammar
    attributes:
      gender: epicene
  - type: Bloodstream
    bloodReagent: DemonsBlood
  - type: Damageable
    damageContainer: BiologicalMetaphysical
    damageModifierSet: Infernal
  - type: Temperature
    heatDamageThreshold: 4000
    coldDamageThreshold: 260
    currentTemperature: 310.15
    coldDamage:
      types:
        Cold : 1
    specificHeat: 42
    heatDamage:
      types:
        Heat : 1
```
