---
type: Combat
title: "Genshin Impact Combat System"
description: "Deep dive into Genshin Impact's real-time combat, elemental reaction matrix, team composition roles, and encounter mechanics."
tags:
  - combat
  - elemental-reactions
  - elemental-gauge-theory
  - team-building
timestamp: "2026-07-22T09:39:06Z"
game_id: "genshin-impact"
confidence: high
---

# Genshin Impact — Combat System

## Core Mechanics & Party Switching

Combat in Genshin Impact is active, real-time, and party-based. Players control a party of up to **4 characters**, swapping active control instantaneously (with a brief off-cooldown timer). Only one character is active on field at a time (except in specific co-op modes), but off-field skill deployables (e.g., Xiangling's Pyronado, Fischl's Oz, Xingqiu's Rainswords) persist when swapping, enabling compounding elemental interactions.

### Character Move Set
Each character possesses:
- **Normal / Charged / Plunging Attacks** (Physical or Elemental infused)
- **Elemental Skill (E):** Short/medium cooldown tactical abilities generating elemental particles.
- **Elemental Burst (Q):** High-impact ultimate ability requiring Energy accumulated from particles and time.

## The Elemental Reaction Matrix

Teyvat features **7 Elements**: Pyro (Fire), Hydro (Water), Anemo (Wind), Electro (Electricity), Dendro (Nature), Cryo (Ice), and Geo (Earth). Combining two or more elements triggers reactions with multiplicative or additive damage scaling and special utility effects.

| Reaction | Elements Involved | Effect / Mechanism |
| :--- | :--- | :--- |
| **Vaporize** | Pyro + Hydro | Multiplicative damage modifier (2.0x if Hydro triggers on Pyro; 1.5x if Pyro triggers on Hydro). |
| **Melt** | Pyro + Cryo | Multiplicative damage modifier (2.0x if Pyro triggers on Cryo; 1.5x if Cryo triggers on Pyro). |
| **Overloaded** | Pyro + Electro | AoE Pyro damage with high knockback; counts as poise damage. |
| **Superconduct** | Cryo + Electro | AoE Cryo damage + reduces physical RES by 40% for 12 seconds. |
| **Frozen / Shatter** | Hydro + Cryo | Immobilizes target. Physical heavy attacks on frozen targets deal Shatter damage. |
| **Electro-Charged** | Hydro + Electro | Continuous tick damage spread to nearby Hydro-affected targets. |
| **Swirl** | Anemo + Pyro/Hydro/Cryo/Electro | Spreads element to adjacent foes; shred RES when paired with Viridescent Venerer. |
| **Crystallize** | Geo + Pyro/Hydro/Cryo/Electro | Drops elemental shields absorbing damage matching element. |
| **Bloom / Hyperbloom / Burgeon** | Dendro + Hydro (+ Electro or Pyro) | Creates Dendro Cores; hitting core with Electro causes homing Hyperbloom; Pyro causes AoE Burgeon. |
| **Quicken / Aggravate / Spread** | Dendro + Electro | Quicken state adds flat bonus damage to subsequent Dendro (Spread) or Electro (Aggravate) hits. |

## Team Roles & Synergies

A standard competitive team composition typically balances four structural roles:
1. **On-Field Main DPS:** Character dealing primary damage during active field time (e.g., Neuvillette, Alhaitham, Hu Tao).
2. **Off-Field Sub-DPS:** Characters generating persistent elemental application and off-field damage (e.g., Furina, Yelan, Xiangling, Nahida).
3. **Support / Buffer:** Characters applying damage multipliers, resistance shreds, or crowd control (e.g., Kazuha, Bennett, Faruzan).
4. **Sustain / Shielder / Healer:** Defensive anchors preserving party HP and interruption resistance (e.g., Zhongli, Xianyun, Kokomi, Baizhu).

For details on how character gear and stats affect combat output, see [Progression](/progression.md).
