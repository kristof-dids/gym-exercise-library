# Instructional image system

The active exercise artwork lives in `images/studio/`. Every exercise has a deterministic slug-based filename, allowing the interface to resolve its new image directly while retaining the original photo as an automatic fallback during production.

## Art direction

- Realistic commercial fitness photography on a seamless white studio background
- Use the same fit adult male presentation throughout the library: short dark hair, charcoal-gray fitted shirt, black shorts, and black training shoes
- High-key, soft lighting with only a subtle floor shadow
- Full body and equipment remain inside the frame
- Dynamic exercises show two clearly separated start and finish positions from the same camera angle, plus an orange-red arrow that follows the actual joint or travel path
- Static holds show one technically correct position; use a force or alignment indicator only when it explains the exercise, never a false movement phase
- The changed joint angle must be visibly different between phases while non-moving joints, the torso and equipment geometry remain consistent
- Equipment counts must be exact and identical between phases; never duplicate, merge or omit dumbbells, handles, plates or cables
- Carries must visibly show a stride and the anti-lean posture; calf walks must visibly keep the heels elevated
- A compact gray anatomical figure sits in unused upper-right space, with primary muscles in vivid orange-red and secondary muscles in a lighter orange-red
- Use front, back, or paired front/back anatomy views according to which view communicates the targets most clearly
- No embedded names, labels, numbers, borders, logos, or watermarks; the interface supplies the text
- Portrait `4:5` canvas, delivered to the site as `680 × 850` WebP

## Prompt template

```text
Use case: scientific-educational
Asset type: portrait exercise-library thumbnail, 4:5 aspect ratio
Primary request: create a clean instructional [EXERCISE] demonstration image matching the established studio exercise-panel visual language.
Scene/backdrop: seamless pure white studio background with a subtle floor shadow
Subject: one fit adult athlete in a charcoal gray fitted T-shirt, black athletic shorts, and black training shoes; show [POSES AND CORRECT FORM]
Style/medium: polished realistic commercial fitness photography, crisp isolated edges, medically neutral and instructional
Composition/framing: [ONE OR TWO] full-body poses, fully visible, with ample white space; [ORANGE-RED ARROW DIRECTION WHEN NEEDED]
Muscle indicator: compact neutral-gray [FRONT/BACK/PAIRED] anatomical figure in unused upper-right space; highlight [PRIMARY MUSCLES] vivid orange-red and [SECONDARY MUSCLES] lighter orange-red
Lighting/mood: high-key soft studio lighting, clean and approachable
Color palette: white, charcoal, black, with one orange-red accent where motion needs explanation
Constraints: anatomically plausible; correct technique; equipment physically coherent; no text, labels, numbers, anatomy diagram, border, logo, or watermark
Avoid: gym background, extra people, distorted hands, extra limbs, duplicate body parts
```

Always use the current source photo as a movement/equipment reference, but do not preserve its gym background or wardrobe. Check every generated asset for exercise accuracy, correct equipment geometry, complete framing, and a readable muscle indicator before placing it in `images/studio/`.

The earlier proof-of-concept variants remain in `images/instructional/` for comparison and rollback.
