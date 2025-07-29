# SS13 Object Prompt Cheat-Sheet  (v2.0)

This file tells the assistant **what to ignore, what to always show, what to confirm, and how to word tricky items**.  
Keep adding rows as new gear pops up.

---

## 0 · How to use  
1. **Load this file first** (CORE Step 0).  
2. When parsing shift-click text:  
   * Skip anything in § 1 unless user explicitly says otherwise.  
   * Always include items from § 2.  
   * If § 3 items appear, pause and ask the user.  
   * For objects in § 4, copy the prompt snippet verbatim to lock in correct rendering.

---

## 1 · Default Omit List  
*(ignore unless the user insists, because they rarely show in the sprite)*

- Security / command **bowman headsets**  
- **PDA** or wallet cartridge (unless name text requested)  
- **Seclite** flashlight (chest-clipped)  
- Unextended **MOD suit control unit**  
- Generic **security belt** (plain pouches, no heroic weapon)  
- **Holobadge** (single-pixel chest square)  
- **Standard satchel / backpack** (unless sprite back-view or user asks)  

---

## 2 · Always Render List — “tiny but iconic”  
*(include even if only 1–2 pixels in the sprite)*

- **Cigars / cigarettes / cigarillo**  
- Any type of **eyewear** (glasses, monocle, HUD shades, Sunscanners)  
- **Rings** or **wristwatches** that appear in text  
- **Gloves** — copy sprite colour; only force bright-red if text says so  

---

## 3 · Ask-the-User Items  
*(stop and confirm before image generation)*

| Trigger text / situation | Ask this question |
|--------------------------|-------------------|
| **ID badge** + user wants readable text | “Latin or Cyrillic? Text may blur—okay to show plain cartridge?” |
| **Gas mask** listed but sprite shows muzzle uncovered | “Gas mask is lowered on sprite—keep it off the face?” |
| **Bare torso or overly revealing outfit** | “Content filters prefer at least a sleeveless shirt; add one?” |
| **Cloak over armor with red cross** | “Cross symbol looks Medical—use security shield emblem instead?” |
| **Hardsuit colour unclear in text** | “Confirm hardsuit striping: black-blue, black-red, or blue-gold?” |

---

## 4 · Common Object Prompt Tips

### 4.1  Security HUD Sunglasses  
- **Sprite cues**: chunky black frame; dark lenses with **red→orange diagonal HUD glare**.  
- **Prompt snippet**  
  > “black security HUD sunglasses – dark lenses showing diagonal red-orange HUD glow”

- **Pitfalls**: renders as plain black shades or mirrored aviators; glare turns blue/green.

---

### 4.2  Sunscanners  
- **Sprite cues**: thick black sci-fi goggles; wide **orange horizontal HUD strip** across both eyes.  
- **Prompt snippet**  
  > “matte-black Sunscanner goggles with bright orange visor strip (no text)”

---

### 4.3  Bright-Red Combat Gloves  
*(Krav-Maga sprite variant)*  
- “bright red combat gloves covering the entire hand”

---

### 4.4  Generic Combat Gloves  
- Copy the **exact sprite colour** (black, grey, etc.).  
  > “dark-grey combat gloves” or “coal-black tactical gloves”

---

### 4.5  Disabler Energy Sidearm  
- **Sprite cues**: short grey carbine, cyan coil at muzzle.  
- Prompt snippet  
  > “compact grey disabler carbine holstered on chest, blue coil at barrel tip”

---

### 4.6  Stun Baton  
- “black telescopic stun baton hooked to belt”

---

### 4.7  Security Gas Mask  
- “matte-black security gas mask – dual side filters, boxy front grill”  
- *Skip entirely if mask not on face per § 3.*

---

### 4.8  Grey Cartridge ID Badge  
- **Default (no text)**  
  > “grey cartridge-style security ID badge with small red status light (no readable text)”  
- **If user wants name** → handle via § 3 ask.

---

### 4.9  Security Beret  
- “black security beret with gold shield patch, flat crown”

---

### 4.10  Hardsuit Colour-Striping Rule  
- Front-load the colour call-out:  
  > “black-blue security hardsuit” • “black-red tactical hardsuit” • “blue-gold command hardsuit”

---

### 4.11  Cloak-over-Armor Layering  
- Keep at least one **shoulder plate visible** so it reads as armor.  
- Swap red cross → security shield if department is not Medical.

---

_Add more objects below this line as we discover new repeat issues._  
