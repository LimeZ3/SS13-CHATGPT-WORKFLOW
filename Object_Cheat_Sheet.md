# SS13 Object Prompt Cheat-Sheet  (v2.2)

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
*(Ignore unless the user explicitly asks for them, because they rarely show in sprite silhouettes)*  

- **Bowman headsets** – any department.  
- **PDA / wallet cartridge** (omit name text unless user insists).  
- **Seclite flashlight / penlight** clipped to chest.  
- **Un-extended MOD-suit control unit**  
  *Tip ▸ If shift-click only says “MOD control unit on back” and does **not** list boots / gauntlets, the suit is UN-extended → safe to omit.*  
- **Plain pouches / satchels / duffelbags** without distinctive markings.  
- **Holobadge** (1-pixel chest square).  
- **Standard satchel / backpack** (unless sprite back-view supplied or user requests).  

---

## 2 · Always Render List — “tiny but iconic”  

*(Include even if the sprite shows only 1–2 pixels.)*

- **Cigars / cigarettes / cigarillos**  
- **Eyewear** of any kind – glasses, monocle, HUD shades, Sunscanners, etc.  
- **Rings** or **wristwatches** mentioned in text.  
- **Gloves** – use sprite colour; force bright-red only if text explicitly states red.

---

## 3 · Ask-the-User Items  

| Trigger text / situation | Clarifying question |
|--------------------------|---------------------|
| **Gas mask** listed but sprite shows muzzle uncovered | “Gas mask is lowered in the sprite – keep it off the face?” |
| **Bare torso / revealing outfit** | “Content filters prefer at least a sleeveless shirt; OK to add one?” |
| **Hardsuit mentioned but colour/department unclear** | “Which hardsuit variant? Sec = black-red, Cap = blue-gold, CE = white, Engineer = brown-orange, Med = lightblue-white, Blueshield = black-blue, or other?” |

*(ID badges default to the omit list; only ask if the user specifically says “show the ID text.”)*

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

### 4.3  Krav-Maga gloves
- “bright red combat gloves covering the entire hand”

---

### 4.4  Generic Combat Gloves  
- Copy the **exact sprite colour** (most likely black, grey).  
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

### 4.12  Insulated Gloves
- **Sprite cues**: vivid yellow, full-finger gloves (rubber texture).
- **Prompt snippet**  
  > “bright yellow insulated gloves covering the entire hand”
- **Pitfalls**: rendered as leather work gloves (brown) or fingerless style.

---

### 4.13  Health-Scanner HUD  *(monocle visor)*
- **Sprite cues**: small **light-blue visor** covering only **one** eye.
- **Prompt snippet**  
  > “single-eye light-blue health-scanner visor over the right eye”
- **Pitfalls**: model turns it into full sunglasses or a green security HUD.

---

### 4.14  Medical HUDSunglasses
- **Sprite cues**: chunky black frame; dark lenses with diagonal **blue** HUD glare (medical department colour).
- **Prompt snippet**  
  > “black medical HUD sunglasses – dark lenses displaying diagonal blue HUD glare”
- **Pitfalls**: glare rendered red (security) or plain black shades.

---

### 4.15  Standard Gas Mask  *(non-security)*
- **Sprite cues**: dark-green rubber mask covering entire face; round **bright-green glass lenses**.
- **Prompt snippet**  
  > “dark-green gas mask covering the full face, bright-green round eye lenses”
- **Pitfalls**: slim modern respirator; lenses coloured red or clear.

---

### 4.16  Breath Mask  *(medical respirator)*
- **Sprite cues**: **light-blue** breathing mask that covers mouth & nose only, leaving eyes exposed.
- **Prompt snippet**  
  > “light-blue medical breath mask over mouth and nose (eyes uncovered)”
- **Pitfalls**: drawn as full gas mask or oxygen helmet.

---

_Add more objects below this line as we discover new repeat issues._  
