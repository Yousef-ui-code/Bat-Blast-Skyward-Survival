# Bat-Blast-Skyward-Survival

# Bat-Blast: Skyward Survival 🦇🔫

A 3D first-person survival game built in **Godot Engine**. 

## 🚀 Game Overview
Defend yourself against flying bat enemies! The game features a 3D environment, a scoring system, and first-person shooter mechanics.

## 🛠️ Main Code Logic (Project Mechanics)
The game is built using GDScript and focuses on these core systems:

### 1. Player Controller (`Player.gd`)
- **Movement:** Uses `CharacterBody2D` or `CharacterBody3D` (depending on project setup) to handle navigation across the map.
- **Shooting:** Instances a projectile at the `Gun` node's global position.
- **Camera:** A first-person camera setup attached to the player for aiming.

### 2. Enemy AI (`Enemy.gd`)
- **Tracking:** Enemies use `global_position.direction_to(player.global_position)` to find and move toward the player.
- **Health System:** Enemies have a `take_damage()` function that reduces health and triggers a death effect/score increase when it reaches zero.

### 3. Game Management
- **Score System:** A global variable that increases every time an enemy is defeated, updated via a UI Label.
- **Exporting:** Configured for Web (HTML5) playability via Godot's Export menu.

## 🕹️ Controls
- **Look:** Mouse Movement
- **Shoot:** Left Mouse Click
- **Move:** WASD Keys

## 📦 How to Build
1. Open the project in **Godot 4.x**.
2. Go to `Project > Export`.
3. Select the **Web (Runnable)** preset.
4. Export as `index.html` to run in a browser.

---
*Developed as part of the Hack Club Milky Way program.*
