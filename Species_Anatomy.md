# SS13 Species & Anatomy Quick-Guide  (v1.1)

*(Put the one-liners into prompts when only a bare description is needed.
For nuanced prompts or troubleshooting, scroll to the two extended sections.)*

| Race | Visual one-liner |
|------|------------------|
| **Human** | Pink-to-brown skin, no extras |
| **Vulpkanin** | Orange/grey canine with upright ears & fluffy tail |
| **Tajaran** | Feline fur, slit pupils, long striped tail |
| **Skrell** | Smooth amphibian skin, head crests, no ears |
| **Unathi** | Scaled reptile, swept head fins/horns, thick tail |
| **Vox** | Avian - beak, feathers, digitigrade legs |
| **IPC** | Synthetic: metal/plastic limbs & glowing faceplate |
| **Diona** | Plant-humanoid, bark plating, glowing green eyes |
| **Plasmaman** | Glowing skeleton inside purple suit & helmet |
| **Slime-Person** | Semi-transparent gelatin body, droplet hands |
| **Nian (Lepidopteran)** | Fuzzy antennae & wings, compound eyes |
| **Kidan** | Chitin armour, mandible mouth, four compound eyes |
| **Drask** | Frost reptile, ice-blue scales, short wide tail |

---

## Ⅰ · Species-Detection Cues  
*(use when the sprite is tiny or obscured, e.g. action scenes)*

| Cue | What it means | Fixes |
|-----|---------------|-------|
| **Tail present & fluffy (2-3 px width)** | Likely **Vulpkanin**; check for upright triangular ears. | Helps pick Vulp in crowded action shots. |
| **Tail present & long, striped** | **Tajaran**; also look for muzzle shape. |
| **Head fin / crest silhouette** | **Unathi** (or Skrell if smooth). |
| **Bright beak pixel** | **Vox** – be sure not to flatten into human nose. |
| **Hair fringe covering visor** | Anthro *has hair length* → keep bangs in illustration (prevents short-hair mismatch). |
| **No ears + smooth blue-green skin** | **Skrell** |
| **Glowing faceplate + joint seams** | **IPC** |
| **Purple hazmat suit, glowing ribs** | **Plasmaman** |

> **Prompt hint:** when you detect one of these cues, front-load it in the prompt
> (`"orange Vulpkanin with fluffy tail"`), so the model locks the species early.

---

## Ⅱ · Species Common Traits & Frequent Mistakes

| Race | Key anatomy / colour notes | Typical generator error | Prompt patch |
|------|---------------------------|-------------------------|--------------|
| **Vulpkanin** | Fur two-tone muzzle & tail tip; separate *hair* can cover visor. | White muzzle rendered as skull mask; hair ignored → short fur. | “orange canine fur with **white muzzle**, long magenta bangs over visor, fluffy white-tipped tail.” |
| **Tajaran** | Striped feline tail, ear tufts, whisker dots. | Tail omitted; stripe pattern lost. | “long striped feline tail clearly visible.” |
| **Skrell** | Smooth skin, three-lobed head crest, slim neck. | Gives human ears or scaly texture. | “no external ears, smooth teal skin, head crest.” |
| **Unathi** | Hard scales, swept horns, thick tail, tall digitigrade legs. | Head fins flattened; tail missing. | “green scaled Unathi, swept-back head fins, thick reptile tail behind legs.” |
| **Vox** | Bird beak, feather ruff, digitigrade legs. | Beak flattened to human nose. | “avian Vox with sharp grey beak and neck feathers.” |
| **IPC** | Joint seams, glowing ‘face’ panel, no flesh. | Adds human skin patches or ears. | “white polymer IPC, glowing cyan faceplate, mechanical joints.” |
| **Diona** | Bark plates, leaves/vines hair, bioluminescent eyes. | Full humanoid skin. | “wood-bark plating and leaf hair.” |
| **Plasmaman** | Transparent suit, glowing bones; always helmeted. | Shows bare skull or removes suit. | “purple pressurised suit encasing glowing skeleton.” |
| **Nian** | Furry chest, antennae, colourful wings. | Wings dropped; antennae turned to hair. | “large midnight-blue wings unfurled, fluffy antennae.” |
| **Kidan** | Chitin segments, four eyes, mandibles. | Drawn as human with helmet. | “dark red chitin armour body, four glowing yellow eyes.” |
| **Drask** | Frosty scales, breath vapour, squat tail. | Rendered as generic lizard. | “ice-blue scales with frost vapour exhale.” |

---

### How to use these tables

1. **Identify** the race quickly with Section Ⅰ cues.  
2. **Copy** the one-liner description into the prompt.  
3. **Append** any Section Ⅱ prompt patches if that race is prone to an error you’ve seen.

*Doing this should fix:*
- Anthro fur-vs-hair confusion  
- Hair-length misreads over HUDs  
- Species ID fails in busy action scenes  
- Missing tails, beaks, crests, etc.
