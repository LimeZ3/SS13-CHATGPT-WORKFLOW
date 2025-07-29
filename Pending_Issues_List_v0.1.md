# SS13 Illustration – Pending Issues List  (v0.4)

Below are all open hiccups we’ve logged so far.  
We’ll tick them off or rewrite as we implement fixes.

---

### Rendering & Style

- **Style preset ignored**  
  *Non-default keywords like “Slick Anime” or “Line Art” sometimes render as Bold-Comic.*

- **Prompt-length trade-offs**  
  *>180 words dilute detail; <60 drops essentials.*

- **Reference docs lazy-load**  
  *Cheat-sheets aren’t always opened unless Step-0 “open” calls fire.*

---

### Gear & Prop Fidelity FIX SUBMITTED

- **HUD-type glasses errors**  
  *Security HUD shades render plain black or wrong-colour glare; Sunscanners gain random text.*

- **ID badge problems**  
  *Text garbled / badge becomes a flat card; “no-text cartridge” rule occasionally skipped.*

- **Weapon / sidearm missing**  
  *Disabler, baton, etc., listed but absent in final art.*

- **Satchel / backpack visibility**  (low-priority cosmetic)

- **Holobadge omission**  
  *1-pixel chest badge dropped — acceptable per omit-list.*

- **Gas-mask presence check**  
  *Shift-click lists mask but sprite shows it lowered; omit if not on face.*

- **Utility-gear token waste**  
  Headset, PDA, seclite, unextended MOD unit, generic security belt → **Low-Visibility Omit List**  
  *Exception: gloves & “tiny but iconic” items stay.*

- **Tiny but iconic items**  
  Cigars, eyewear, wristwatches, rings → **always include** even if 1-pixel.

---

### Colour & Material Accuracy FIX SUBMITTED

- **Combat-glove colour drift**  
  *Bright-red Krav gloves appear black — OR dark gloves forced red.*

- **Glove-colour fidelity rule**  
  *Copy sprite hue; only force red if text explicitly says so.*

- **Sleeve-stripe colour drift**  
  *Extra white band added to red arm stripes.*

- **Blood-stained items render clean**

- **Background department palette**  
  *Security corridor rendered teal; departmental colours off.*

---

### Species & Anatomy - FIX SUBMITTED

- **Anthro fur vs. hair confusion**  
  *White Vulp/Taj muzzle read as skull mask; need separate fur-colour vs. hair-colour.*

- **Hair-length misread on anthros**  
  *Fringe covering visor becomes short slick hair.*

- **Species detection in action scenes**  
  *Anthro tails/ears missed → Vulp/Taj flagged as human.*

- **Species anatomy omissions**  
  *Tails absent; Unathi crests simplified; Vox beak flattened.*

---

### Armour & Clothing FIX SUBMITTED

- **Armor vs. cloak layering**  
  *Cloak hides security armor or swaps red cross (Medical) onto Sec plate.*

- **Hardsuit type & palette recognition**  
  *Black-blue vs. black-red vs. blue-gold suits blended.*

- **Partial-nudity safeguard**  
  *Bare-chest sprites risk filter strike — prompt to add sleeveless shirt.*

---

### Scene Composition

- **Accurate head-count in crowded screens**  
  *Scene with four combatants produced three.*

- **Sprite angle coverage gaps**  
  *Missing rear view loses backpacks, tails, coat tails.*

---

### To-Do: Cheat-Sheet Expansion

- Add: security beret, disabler sidearm, red/grey combat gloves, etc.

---
