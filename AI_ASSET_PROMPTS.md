# AI Character Asset Generation Guide
## Complete Step-by-Step Prompts for RPG Maker MZ Characters

This guide provides detailed, copy-paste-ready prompts for generating complete character assets for the "Pharmageddon" RPG.

---

## **⚠️ TRANSPARENCY REQUIREMENTS - READ THIS FIRST**

Different asset types have different background requirements:

| Asset Type | Background Requirement | Reason |
|------------|----------------------|--------|
| **Concept Art** | White background OK | Reference only, NOT used in game |
| **Face Portraits** | Transparent OR solid color (transparent recommended) | Optional - both work in RPG Maker |
| **Walking Sprites** | MUST be transparent | Required - characters walk on various map backgrounds |
| **Battle Sprites** | MUST be transparent | Required - appear over battle backgrounds |

**TL;DR**: Use **TRANSPARENT PNG backgrounds** for all in-game assets (faces, walking sprites, battle sprites). Only concept art can have a white background because it's reference only.

---

## **Character Asset Generation Order**

Generate assets in this recommended order:
1. **Concept Art** (optional reference - white background OK)
2. **Face Portraits** (easiest - transparent recommended)
3. **Walking Sprite** (medium difficulty - MUST be transparent)
4. **Battle Sprite** (most complex - MUST be transparent)

---

## **STEP 1: Concept Art (Optional Reference)**

### Purpose
Create reference art to maintain consistency across all other assets.

**IMPORTANT**: This is REFERENCE ONLY and NOT used in the game. White background is fine here.

### AI Prompt Template
```
Create a character reference sheet for an RPG character. Full-body front view, side view, and back view on white background. Character design: [DESCRIBE CHARACTER - see examples below]. Include color swatches showing exact colors used. Anime/JRPG art style. High detail. 1920x1080 pixels or larger.
```

### Example Prompts

**Cyberpunk Medic Character**:
```
Create a character reference sheet for an RPG character. Full-body front view, side view, and back view on white background. Character design: Female cyberpunk medic in her late 20s, short white hair with cyan highlights, augmented reality visor over left eye, medical cross symbol on jacket, utility belt with syringes and medical equipment, tactical boots, color palette of white, cyan, and dark gray. Include color swatches showing exact colors used. Anime/JRPG art style. High detail. 1920x1080 pixels.
```

**Street Samurai Character**:
```
Create a character reference sheet for an RPG character. Full-body front view, side view, and back view on white background. Character design: Male street samurai with cybernetic arm, slicked-back black hair, armored jacket with neon red accents, katana on back, tech-enhanced sunglasses, combat pants with knee guards, color palette of black, red, and chrome silver. Include color swatches showing exact colors used. Anime/JRPG art style. High detail. 1920x1080 pixels.
```

### Post-Generation Instructions
1. Save this file as `concept-CharacterName.png` in a reference folder (NOT in game directories)
2. **This file is NOT used in-game** - it's only for your reference when generating other assets
3. Use this as visual reference for all subsequent asset generation
4. Note the exact colors used for consistency

---

## **STEP 2: Face Portraits** (576×288 pixels, 8 faces)

### Technical Specifications
- **Exact Dimensions**: 576 width × 288 height pixels
- **Grid Layout**: 4 columns × 2 rows = 8 face positions
- **Individual Face Size**: 144 × 144 pixels each
- **File Format**: PNG
- **Background**: OPTIONAL - can be transparent OR have solid color/gradient background
  - **Recommended**: Transparent PNG for consistency with other assets
  - **Also works**: Solid color or gradient background (dark colors work best)
- **Content**: 8 different facial expressions

### Grid Layout Reference
```
[Face 0: Neutral] [Face 1: Happy]     [Face 2: Sad]      [Face 3: Angry]
[Face 4: Surprised][Face 5: Worried]  [Face 6: Determined][Face 7: Shocked]
```

### AI Prompt Template - FULL VERSION
```
Create an RPG character portrait sprite sheet with EXACT dimensions 576 pixels wide by 288 pixels tall. The sheet must contain exactly 8 character face portraits arranged in a perfect 4x2 grid (4 columns, 2 rows). Each individual portrait must be exactly 144x144 pixels with NO gaps or padding between portraits.

Character Description: [INSERT CHARACTER DETAILS]

The 8 portraits must show these exact expressions in this exact order:
- Top row, left to right: Neutral expression, Happy/smiling, Sad/downcast, Angry/fierce
- Bottom row, left to right: Surprised/shocked, Worried/concerned, Determined/serious, Very shocked/gasping

Art style: Anime/JRPG character portrait style, shoulder-up or bust shot, consistent character design across all 8 faces, only facial expression changes between portraits.

Background options: CHOOSE ONE:
- Option A (recommended): Transparent PNG background
- Option B: Dark solid color or subtle gradient background (if using this, specify the color)

Technical requirements: PNG format, each face exactly 144x144 pixels, total canvas exactly 576x288 pixels, no borders or gaps between portraits, pixel-perfect grid alignment.
```

### Example Prompts

**Cyberpunk Medic Portrait Sheet** (with transparent background - recommended):
```
Create an RPG character portrait sprite sheet with EXACT dimensions 576 pixels wide by 288 pixels tall. The sheet must contain exactly 8 character face portraits arranged in a perfect 4x2 grid (4 columns, 2 rows). Each individual portrait must be exactly 144x144 pixels with NO gaps or padding between portraits.

Character Description: Female cyberpunk medic, late 20s, short white hair with cyan highlights, augmented reality visor over left eye (glowing cyan), medical cross earring, white high-collar jacket with cyan trim, pale skin, cybernetic facial tattoo on right cheek, sharp intelligent eyes.

The 8 portraits must show these exact expressions in this exact order:
- Top row, left to right: Neutral professional expression, Happy confident smile, Sad concerned look, Angry fierce glare
- Bottom row, left to right: Surprised wide eyes, Worried anxious expression, Determined serious focused look, Very shocked gasping

Art style: Anime/JRPG character portrait style, shoulder-up view showing head and upper shoulders, consistent character design across all 8 faces, only facial expression changes between portraits.

Technical requirements: PNG format with TRANSPARENT background, each face exactly 144x144 pixels, total canvas exactly 576x288 pixels, no borders or gaps between portraits, pixel-perfect grid alignment.
```

**Alternative version with dark background** (also acceptable):
```
[Same as above, but change the last line to:]
Technical requirements: PNG format with dark gray gradient background, each face exactly 144x144 pixels, total canvas exactly 576x288 pixels, no borders or gaps between portraits, pixel-perfect grid alignment.
```

**Street Samurai Portrait Sheet** (with transparent background - recommended):
```
Create an RPG character portrait sprite sheet with EXACT dimensions 576 pixels wide by 288 pixels tall. The sheet must contain exactly 8 character face portraits arranged in a perfect 4x2 grid (4 columns, 2 rows). Each individual portrait must be exactly 144x144 pixels with NO gaps or padding between portraits.

Character Description: Male street samurai, mid-30s, slicked-back black hair with red streak, tech-enhanced red sunglasses, cybernetic jaw implant (chrome), scar across left eyebrow, stubble beard, black armored collar with red LED strips, tan skin, sharp angular features.

The 8 portraits must show these exact expressions in this exact order:
- Top row, left to right: Neutral stoic expression, Happy slight smirk, Sad regretful frown, Angry intense scowl
- Bottom row, left to right: Surprised raised eyebrow, Worried tense look, Determined battle-ready focus, Very shocked eyes wide

Art style: Anime/JRPG character portrait style, shoulder-up view showing head and upper shoulders, consistent character design across all 8 faces, only facial expression changes between portraits.

Technical requirements: PNG format with TRANSPARENT background, each face exactly 144x144 pixels, total canvas exactly 576x288 pixels, no borders or gaps between portraits, pixel-perfect grid alignment.
```

### Post-Generation Checklist
- [ ] Image is exactly 576×288 pixels (check in image editor)
- [ ] 8 faces are clearly visible
- [ ] Each face is 144×144 pixels (verify by dividing canvas into 4×2 grid)
- [ ] No gaps or padding between faces
- [ ] All 8 faces show the same character with different expressions
- [ ] Character design is consistent (hair, clothing, features don't change)
- [ ] File is PNG format
- [ ] Background is either transparent OR solid color (both acceptable, transparent recommended)

### Saving
- **Filename**: `CharacterName.png` (e.g., `CyberMedic.png`)
- **Location**: `C:\Projects\rpg-maker\img\faces\`
- **Git**: Will be tracked by Git LFS automatically

---

## **STEP 3: Walking Sprite Sheet** (576×384 pixels, 8 characters)

### Technical Specifications
- **Exact Dimensions**: 576 width × 384 height pixels
- **Grid Layout**: 4 columns × 2 rows = 8 character positions
- **Individual Character Block**: 144 × 192 pixels each
- **Frame Layout per Character**: 3 columns × 4 rows
  - **Individual Frame**: 48 × 48 pixels
  - Row 1: Down-facing (3 frames)
  - Row 2: Left-facing (3 frames)
  - Row 3: Right-facing (3 frames)
  - Row 4: Up-facing (3 frames)
- **File Format**: PNG
- **Background**: MUST BE TRANSPARENT (required for walking sprites)

### Walking Animation Frame Details
Each character has 12 frames total (3 frames × 4 directions):
- **Frame 1**: Left foot forward
- **Frame 2**: Standing position (both feet together)
- **Frame 3**: Right foot forward

### Grid Layout Reference
```
[Char 0]  [Char 1]  [Char 2]  [Char 3]
[Char 4]  [Char 5]  [Char 6]  [Char 7]

Each character block (144×192px) contains:
[Down-L] [Down-C] [Down-R]
[Left-L] [Left-C] [Left-R]
[Right-L][Right-C][Right-R]
[Up-L]   [Up-C]   [Up-R]
(Each cell = 48×48px)
```

### AI Prompt Template - FULL VERSION
```
Create a top-down RPG character walking sprite sheet with EXACT dimensions 576 pixels wide by 384 pixels tall. The sheet contains 8 character positions arranged in a 4x2 grid (4 columns, 2 rows). Each character occupies exactly 144x192 pixels.

CRITICAL: Each character must show 4-directional walking animation in a 3x4 grid of 48x48 pixel frames:
- Row 1 (3 frames): Walking DOWN/SOUTH - left foot forward, standing center, right foot forward
- Row 2 (3 frames): Walking LEFT/WEST - left foot forward, standing center, right foot forward
- Row 3 (3 frames): Walking RIGHT/EAST - left foot forward, standing center, right foot forward
- Row 4 (3 frames): Walking UP/NORTH - left foot forward, standing center, right foot forward

Character designs for all 8 positions: [DESCRIBE EACH CHARACTER OR "repeated character" FOR SINGLE CHARACTER]

Art style: Top-down pixel art RPG style, similar to classic JRPG sprites, clean pixel art with clear outlines, character should be proportioned to fit within 48x48 pixel frame comfortably (typically 32-40 pixels tall).

Technical requirements:
- PNG format with TRANSPARENT background (NO white or colored background)
- Total canvas exactly 576x288 pixels
- Each character block exactly 144x192 pixels
- Each individual frame exactly 48x48 pixels
- No gaps or padding between frames
- Pixel-perfect grid alignment
- Characters should face the correct direction (down, left, right, up)
- Walking animation should show clear left/center/right stepping motion
```

### Example Prompts

**Option A: Single Character Repeated (Recommended for Beginners)**
```
Create a top-down RPG character walking sprite sheet with EXACT dimensions 576 pixels wide by 384 pixels tall. The sheet contains 8 character positions arranged in a 4x2 grid (4 columns, 2 rows). Each character occupies exactly 144x192 pixels.

CRITICAL: Each character must show 4-directional walking animation in a 3x4 grid of 48x48 pixel frames:
- Row 1 (3 frames): Walking DOWN/SOUTH - left foot forward, standing center, right foot forward
- Row 2 (3 frames): Walking LEFT/WEST - left foot forward, standing center, right foot forward
- Row 3 (3 frames): Walking RIGHT/EAST - left foot forward, standing center, right foot forward
- Row 4 (3 frames): Walking UP/NORTH - left foot forward, standing center, right foot forward

Character design: Female cyberpunk medic wearing white jacket with cyan highlights, short white hair with cyan tips, medical cross on back of jacket, utility belt, dark pants, tactical boots. Character should be about 36-40 pixels tall in the sprite. ALL 8 CHARACTER POSITIONS SHOULD SHOW THE SAME CHARACTER (repeated 8 times for potential future variants or team members).

Art style: Top-down pixel art RPG style, clean pixel art with black outlines, vibrant colors (white, cyan, dark gray), character proportioned to fit comfortably in 48x48 pixel frame.

Technical requirements:
- PNG format with TRANSPARENT background (NO white or colored background)
- Total canvas exactly 576x384 pixels
- Each character block exactly 144x192 pixels
- Each individual frame exactly 48x48 pixels
- No gaps or padding between frames
- Pixel-perfect grid alignment
- Characters should face the correct direction (down, left, right, up)
- Walking animation should show clear left/center/right stepping motion
```

**Option B: Single Large Character ($ Prefix Format)**

If you want just ONE character on the sheet (uses less space, cleaner):

```
Create a top-down RPG character walking sprite with EXACT dimensions 144 pixels wide by 192 pixels tall. This is a single character sprite showing 4-directional walking animation.

The sprite must be organized in a 3x4 grid of 48x48 pixel frames:
- Row 1 (3 frames): Walking DOWN/SOUTH - left foot forward, standing center, right foot forward
- Row 2 (3 frames): Walking LEFT/WEST - left foot forward, standing center, right foot forward
- Row 3 (3 frames): Walking RIGHT/EAST - left foot forward, standing center, right foot forward
- Row 4 (3 frames): Walking UP/NORTH - left foot forward, standing center, right foot forward

Character design: Female cyberpunk medic wearing white jacket with cyan highlights, short white hair with cyan tips, medical cross on back of jacket, utility belt, dark pants, tactical boots. Character should be about 36-40 pixels tall in the sprite.

Art style: Top-down pixel art RPG style, clean pixel art with black outlines, vibrant colors (white, cyan, dark gray), character proportioned to fit comfortably in 48x48 pixel frame.

Technical requirements:
- PNG format with TRANSPARENT background
- Total canvas exactly 144x192 pixels
- Each individual frame exactly 48x48 pixels
- No gaps or padding between frames
- Pixel-perfect grid alignment (3 columns, 4 rows)
- Characters should face correct directions
- Clear walking animation with stepping motion
```

**Save this with `$` prefix**: `$CyberMedic.png` (the `$` tells RPG Maker it's a single character file)

### Post-Generation Checklist
- [ ] Image dimensions are exactly correct (576×384 for sheet, 144×192 for single)
- [ ] Transparent background (NO white/colored background visible)
- [ ] All frames are exactly 48×48 pixels
- [ ] Character faces DOWN in row 1, LEFT in row 2, RIGHT in row 3, UP in row 4
- [ ] Walking animation shows clear stepping motion (left foot, center, right foot)
- [ ] Character is appropriately sized (not too large for 48×48 frame)
- [ ] Pixel art is clean with clear outlines
- [ ] No gaps or padding between frames
- [ ] File is PNG format

### Common AI Generation Issues & Fixes
1. **AI adds white/colored background**: Use image editor to remove background, set to transparent
2. **Dimensions are wrong**: Crop/resize canvas to exact pixels WITHOUT scaling content
3. **Character too large**: Regenerate with "character should be 32-40 pixels tall" in prompt
4. **Frames not aligned**: Use image editor grid overlay to verify 48×48 pixel alignment
5. **Wrong number of frames**: Regenerate emphasizing "3 columns × 4 rows" per character

### Saving
- **Filename**:
  - Standard sheet: `CharacterName.png` (e.g., `CyberMedic.png`)
  - Single character: `$CharacterName.png` (e.g., `$CyberMedic.png`) - note the `$` prefix!
- **Location**: `C:\Projects\rpg-maker\img\characters\`
- **Git**: Will be tracked by Git LFS automatically

---

## **STEP 4: Side-View Battle Sprite** (576×384 pixels, 18 motions)

### Technical Specifications
- **Exact Dimensions**: 576 width × 384 height pixels
- **Grid Layout**: 9 columns × 6 rows = 54 frames
- **Individual Frame**: 64 × 64 pixels
- **File Format**: PNG
- **Background**: MUST BE TRANSPARENT (required for battle sprites)
- **Frames per Motion**: 3 animation frames (horizontal)
- **Total Motions**: 18 different battle actions

### Motion Layout Reference
```
Column:     1        2        3        4        5        6        7        8        9
Row 1:  [Walk 1][Walk 2][Walk 3][Wait 1][Wait 2][Wait 3][Chant1][Chant2][Chant3]
Row 2:  [Guard1][Guard2][Guard3][Dmg 1][Dmg 2][Dmg 3][Evade1][Evade2][Evade3]
Row 3:  [Thrst1][Thrst2][Thrst3][Swing1][Swing2][Swing3][Msle 1][Msle 2][Msle 3]
Row 4:  [Skill1][Skill2][Skill3][Spell1][Spell2][Spell3][Item 1][Item 2][Item 3]
Row 5:  [Escap1][Escap2][Escap3][Victr1][Victr2][Victr3][Dying1][Dying2][Dying3]
Row 6:  [Abnor1][Abnor2][Abnor3][Sleep1][Sleep2][Sleep3][Dead 1][Dead 2][Dead 3]

Each cell = 64×64 pixels
```

### Detailed Motion Descriptions

**Row 1: Basic Motions**
- **Walk** (frames 1-3): Side-view walking motion, left to right
- **Wait** (frames 4-6): Idle battle stance, breathing/slight movement
- **Chant** (frames 7-9): Preparing to cast, hands gathering energy, glowing effect

**Row 2: Defensive Motions**
- **Guard** (frames 10-12): Defensive stance, shield up or arms crossed
- **Damage** (frames 13-15): Getting hit, recoiling backward, pain expression
- **Evade** (frames 16-18): Jumping/dodging backward or to side

**Row 3: Physical Attacks**
- **Thrust** (frames 19-21): Stabbing attack with spear/sword, forward lunge
- **Swing** (frames 22-24): Slashing attack, wide arc motion
- **Missile** (frames 25-27): Shooting/throwing projectile, arm extended

**Row 4: Skills & Items**
- **Skill** (frames 28-30): Using special ability, dynamic pose
- **Spell** (frames 31-33): Casting magic, hands raised, magical effect
- **Item** (frames 34-36): Using item, reaching into bag/pocket

**Row 5: Battle End Motions**
- **Escape** (frames 37-39): Running away, turning and fleeing
- **Victory** (frames 40-42): Celebratory pose, weapon raised or peace sign
- **Dying** (frames 43-45): Collapsing to knees, falling animation

**Row 6: Status Motions**
- **Abnormal** (frames 46-48): Afflicted by status (poison, confusion), swaying
- **Sleep** (frames 49-51): Sleeping stance, ZZZ effect, eyes closed
- **Dead** (frames 52-54): Defeated, lying on ground

### AI Prompt Template - FULL VERSION
```
Create a side-view RPG battle character sprite sheet with EXACT dimensions 576 pixels wide by 384 pixels tall. The sheet must be organized in a perfect 9x6 grid (9 columns, 6 rows) with each frame exactly 64x64 pixels. This creates 54 total frames showing 18 different battle motions with 3 animation frames each.

Character design: [DESCRIBE CHARACTER IN SIDE-VIEW BATTLE POSE]

The sprite sheet must show these 18 battle motions in this EXACT order:

ROW 1 (frames 1-9):
- Columns 1-3: WALK - side-view walking motion (left foot, center, right foot)
- Columns 4-6: WAIT - idle battle stance, breathing animation
- Columns 7-9: CHANT - preparing to cast, gathering energy, slight glow

ROW 2 (frames 10-18):
- Columns 1-3: GUARD - defensive stance, blocking with shield/arms
- Columns 4-6: DAMAGE - getting hit, recoiling back, pain expression
- Columns 7-9: EVADE - dodging/jumping to the side or backward

ROW 3 (frames 19-27):
- Columns 1-3: THRUST - stabbing attack forward with weapon (spear/sword lunge)
- Columns 4-6: SWING - slashing attack in wide arc motion
- Columns 7-9: MISSILE - shooting/throwing projectile, arm extended forward

ROW 4 (frames 28-36):
- Columns 1-3: SKILL - using special ability, dynamic action pose
- Columns 4-6: SPELL - casting magic, hands raised, mystical gesture
- Columns 7-9: ITEM - using item, reaching for pocket/bag

ROW 5 (frames 37-45):
- Columns 1-3: ESCAPE - running away, turning to flee
- Columns 4-6: VICTORY - celebratory pose, weapon raised triumphantly
- Columns 7-9: DYING - collapsing to knees, falling down animation

ROW 6 (frames 46-54):
- Columns 1-3: ABNORMAL - afflicted by status effect, swaying/staggering
- Columns 4-6: SLEEP - sleeping stance, eyes closed, peaceful
- Columns 7-9: DEAD - defeated, lying on ground motionless

Art style: Anime/JRPG side-view battle sprite style, character should be 48-56 pixels tall, dynamic poses, clear action silhouettes, character faces RIGHT (toward enemy).

Technical requirements:
- PNG format with TRANSPARENT background
- Total canvas exactly 576x384 pixels
- Perfect 9x6 grid layout
- Each frame exactly 64x64 pixels
- No gaps or padding between frames
- Pixel-perfect alignment
- Character consistently sized across all frames
- Smooth 3-frame animations for each motion
- Character should face RIGHT in all poses (attacking toward the right side)
```

### Example Prompts

**Cyberpunk Medic Battle Sprite**:
```
Create a side-view RPG battle character sprite sheet with EXACT dimensions 576 pixels wide by 384 pixels tall. The sheet must be organized in a perfect 9x6 grid (9 columns, 6 rows) with each frame exactly 64x64 pixels. This creates 54 total frames showing 18 different battle motions with 3 animation frames each.

Character design: Female cyberpunk medic in side-view battle stance. White armored jacket with cyan LED strips, short white hair with cyan highlights, cybernetic visor over left eye (glowing cyan), medical cross symbol on shoulder, utility belt with syringes, tactical boots. Holding high-tech medical gun/scanner device. Character about 50 pixels tall, facing RIGHT.

The sprite sheet must show these 18 battle motions in this EXACT order:

ROW 1 (frames 1-9):
- Columns 1-3: WALK - side-view walking motion, steady pace
- Columns 4-6: WAIT - idle battle stance, breathing, scanner device ready
- Columns 7-9: CHANT - preparing ability, device glowing cyan

ROW 2 (frames 10-18):
- Columns 1-3: GUARD - defensive stance, medical shield projecting
- Columns 4-6: DAMAGE - getting hit, recoiling back, cyan sparks
- Columns 7-9: EVADE - quick dodge backward, agile motion

ROW 3 (frames 19-27):
- Columns 1-3: THRUST - forward lunge with syringe weapon
- Columns 4-6: SWING - wide arc attack with medical scanner beam
- Columns 7-9: MISSILE - shooting healing dart/projectile from medical gun

ROW 4 (frames 28-36):
- Columns 1-3: SKILL - deploying medical drone/gadget with hand gesture
- Columns 4-6: SPELL - casting healing ability, cyan energy from hands
- Columns 7-9: ITEM - pulling syringe from belt, administering

ROW 5 (frames 37-45):
- Columns 1-3: ESCAPE - turning and running away
- Columns 4-6: VICTORY - triumphant pose, holding medical scanner up
- Columns 7-9: DYING - collapsing to knees, dropping weapon

ROW 6 (frames 46-54):
- Columns 1-3: ABNORMAL - staggering, glitching visor effect
- Columns 4-6: SLEEP - sleeping stance, visor dimmed
- Columns 7-9: DEAD - lying on ground, defeated

Art style: Anime/JRPG side-view battle sprite, pixel art or high-detail sprite art, character 48-54 pixels tall, dynamic battle poses, clear action silhouettes, character consistently faces RIGHT, cyan glow effects on visor and tech.

Technical requirements:
- PNG format with TRANSPARENT background
- Total canvas exactly 576x384 pixels
- Perfect 9x6 grid layout
- Each frame exactly 64x64 pixels
- No gaps or padding between frames
- Pixel-perfect alignment
- Character consistently sized and positioned across all frames
- Smooth 3-frame animations for each motion
```

**Street Samurai Battle Sprite**:
```
Create a side-view RPG battle character sprite sheet with EXACT dimensions 576 pixels wide by 384 pixels tall. The sheet must be organized in a perfect 9x6 grid (9 columns, 6 rows) with each frame exactly 64x64 pixels. This creates 54 total frames showing 18 different battle motions with 3 animation frames each.

Character design: Male street samurai in side-view battle stance. Black armored jacket with red neon trim, cybernetic right arm (chrome with red LEDs), slicked-back black hair with red streak, katana sword, tech sunglasses, combat pants. Character about 52 pixels tall, facing RIGHT, ready for combat.

The sprite sheet must show these 18 battle motions in this EXACT order:

ROW 1 (frames 1-9):
- Columns 1-3: WALK - side-view walking, confident stride, hand on katana hilt
- Columns 4-6: WAIT - idle battle stance, katana ready, breathing
- Columns 7-9: CHANT - preparing technique, cybernetic arm glowing red

ROW 2 (frames 10-18):
- Columns 1-3: GUARD - defensive stance, katana blocking horizontally
- Columns 4-6: DAMAGE - getting hit, recoiling, red sparks from cyber arm
- Columns 7-9: EVADE - quick sidestep dodge, blade trailing

ROW 3 (frames 19-27):
- Columns 1-3: THRUST - quick forward stab with katana
- Columns 4-6: SWING - powerful slash in wide arc, blade motion blur
- Columns 7-9: MISSILE - throwing shuriken/blade from cyber arm

ROW 4 (frames 28-36):
- Columns 1-3: SKILL - special cyber-slash technique, red energy trail
- Columns 4-6: SPELL - activating cybernetic ability, red circuit patterns
- Columns 7-9: ITEM - grabbing item from belt with free hand

ROW 5 (frames 37-45):
- Columns 1-3: ESCAPE - tactical retreat, turning to run
- Columns 4-6: VICTORY - katana raised overhead triumphantly, slight smirk
- Columns 7-9: DYING - falling to one knee, dropping sword

ROW 6 (frames 46-54):
- Columns 1-3: ABNORMAL - staggering, cyber arm glitching/sparking
- Columns 4-6: SLEEP - kneeling/sleeping, sword lowered
- Columns 7-9: DEAD - collapsed on ground, katana fallen beside

Art style: Anime/JRPG side-view battle sprite, pixel art or detailed sprite art, character 48-54 pixels tall, dynamic samurai combat poses, motion blur on fast attacks, character faces RIGHT, red glow on cybernetic arm.

Technical requirements:
- PNG format with TRANSPARENT background
- Total canvas exactly 576x384 pixels
- Perfect 9x6 grid layout
- Each frame exactly 64x64 pixels
- No gaps or padding between frames
- Pixel-perfect alignment
- Character consistently sized across all frames
- Smooth 3-frame animations
- Katana should be clearly visible in combat poses
```

### Post-Generation Checklist
- [ ] Image is exactly 576×384 pixels
- [ ] Transparent background (no white/color showing)
- [ ] 9 columns × 6 rows = 54 frames visible
- [ ] Each frame is exactly 64×64 pixels
- [ ] Character faces RIGHT in all poses
- [ ] Character is consistently sized across all frames (48-56 pixels tall)
- [ ] All 18 motions are present and distinguishable
- [ ] Animations show clear motion between 3 frames
- [ ] Weapon/equipment is visible and consistent
- [ ] File is PNG format

### Common AI Generation Issues & Fixes

1. **Wrong dimensions**:
   - Fix: Crop/resize canvas to exactly 576×384 WITHOUT scaling
   - Verify: Check image properties, should be 576×384

2. **Character inconsistent size across frames**:
   - Fix: Manually adjust or regenerate with "character must be same height in all frames"

3. **Wrong number of frames/wrong grid**:
   - Fix: Regenerate emphasizing "9 columns × 6 rows, 64×64 pixels each frame"

4. **Character faces LEFT instead of RIGHT**:
   - Fix: Flip entire image horizontally in image editor

5. **Motions in wrong order**:
   - Fix: Use image editor to cut and rearrange 64×64 pixel cells to correct order
   - Reference the motion layout chart above

6. **Background not transparent**:
   - Fix: Use image editor (GIMP, Photoshop) to remove background and save with alpha channel

7. **Frames have gaps/padding**:
   - Fix: Crop and realign to perfect 64×64 grid

### Saving
- **Filename**: `CharacterName.png` (e.g., `CyberMedic.png` or `StreetSamurai.png`)
- **Location**: `C:\Projects\rpg-maker\img\sv_actors\`
- **Git**: Will be tracked by Git LFS automatically

---

## **POST-GENERATION: Setting Up in RPG Maker MZ**

Once you have all 3 image files generated and saved:

1. **Open RPG Maker MZ**
2. **Go to Database** (F9 or Tools > Database)
3. **Select "Actors" tab**
4. **Create new actor or edit existing**
5. **Set the following fields**:

### Face Settings
- **Face**: Click the face graphic box
- **Select your face file**: `CharacterName.png` from the list
- **Face Index**: Select which face (0-7) - usually 0 for first face

### Character Sprite Settings
- **Character**: Click the character sprite box
- **Select your walking sprite**: `CharacterName.png` or `$CharacterName.png`
- **Character Index**:
  - If using standard sheet (576×384): Select 0-7 for position
  - If using $ prefix single (144×192): Always use 0

### Battle Sprite Settings
- **[SV] Battler**: Click the side-view battler box
- **Select your battle sprite**: `CharacterName.png` from sv_actors folder

### Text Fields
- **Name**: Character's display name (e.g., "Dr. Sarah Chen")
- **Nickname**: Subtitle/class (e.g., "Cyber Medic")
- **Profile**: Character backstory (e.g., "Former ER doctor turned street medic in Neo Tokyo's underground...")

6. **Click OK** to save

---

## **VERIFICATION: Testing Your Character Assets**

### In RPG Maker Playtest:
1. Press **F12** or **Game > Playtest**
2. Check that character appears on map with correct walking sprite
3. Open **Menu** (X or Escape) - verify face portrait appears
4. Check **Status** screen - verify face, name, nickname, profile
5. **Start a battle** (create test battle in database):
   - Verify side-view battle sprite appears
   - Watch character perform attack - verify animations work
   - Cast spell - verify spell animation plays
   - Get hit - verify damage animation plays

### What to Look For:
- ✅ Walking sprite shows correct character walking in 4 directions
- ✅ Face portrait displays correctly in dialogue/menus
- ✅ Battle sprite shows character in side-view with all animations
- ✅ Character is properly sized (not too large or too small)
- ✅ Transparent backgrounds show correctly (no white boxes)
- ✅ Animations are smooth

---

## **TROUBLESHOOTING COMMON ISSUES**

### Character shows as blank/missing sprite
**Cause**: File not found or wrong filename
**Fix**:
- Verify file is in correct directory (`img/characters/`, `img/faces/`, or `img/sv_actors/`)
- Check filename exactly matches what's set in Database
- Ensure file extension is `.png` (lowercase)

### White box around character
**Cause**: Background not transparent
**Fix**:
- Open PNG in image editor (GIMP, Photoshop, Paint.NET)
- Remove background layer
- Export with transparency/alpha channel enabled

### Wrong character shows from sheet
**Cause**: Wrong character index selected
**Fix**:
- In Database > Actors, change "Character Index" or "Face Index" (0-7)
- Index 0 = top-left, index 7 = bottom-right

### Battle sprite animations don't play correctly
**Cause**: Frames in wrong order or wrong grid size
**Fix**:
- Verify sprite sheet is exactly 576×384 pixels
- Verify 9×6 grid with 64×64 pixel frames
- Check motions are in correct order per layout chart above

### Character too large/too small on map
**Cause**: Character sprite is not properly sized for 48×48 pixel frames
**Fix**:
- Regenerate walking sprite with "character 32-40 pixels tall" in prompt
- Or manually resize character in image editor while keeping canvas size

---

## **QUICK REFERENCE: File Locations & Naming**

| Asset Type | File Location | Filename Format | Example |
|------------|---------------|-----------------|---------|
| **Face Portrait** | `img/faces/` | `CharacterName.png` | `CyberMedic.png` |
| **Walking Sprite (sheet)** | `img/characters/` | `CharacterName.png` | `CyberMedic.png` |
| **Walking Sprite (single)** | `img/characters/` | `$CharacterName.png` | `$CyberMedic.png` |
| **Battle Sprite** | `img/sv_actors/` | `CharacterName.png` | `CyberMedic.png` |

---

## **WORKFLOW SUMMARY**

For each new character:

1. ✅ Generate **Concept Art** (optional reference)
2. ✅ Generate **Face Portrait Sheet** (576×288px) → save to `img/faces/`
3. ✅ Generate **Walking Sprite Sheet** (576×384px or 144×192px) → save to `img/characters/`
4. ✅ Generate **Battle Sprite Sheet** (576×384px) → save to `img/sv_actors/`
5. ✅ Verify dimensions and transparency in image editor
6. ✅ Set up in RPG Maker Database > Actors
7. ✅ Playtest to verify all assets display correctly

---

## **AI GENERATION TIPS**

### Best Practices:
1. **Be specific about dimensions** - AI often adds padding; emphasize "EXACT dimensions"
2. **Request transparent background** explicitly for sprites
3. **Mention pixel art style** for walking sprites
4. **Describe character consistently** across all prompts (copy/paste description)
5. **Specify character facing direction** (DOWN for walking row 1, RIGHT for battle sprites)
6. **Test with one character first** before generating full party

### Recommended AI Tools:
- **Midjourney**: Best for high-quality concept art and portraits
- **DALL-E 3**: Good for precise dimensions and grid layouts
- **Stable Diffusion** (with ControlNet): Best for pixel art and exact sprite dimensions
- **Aseprite AI plugins**: Specialized for pixel art sprites

### Post-Processing Tools:
- **GIMP** (free): Remove backgrounds, crop to exact dimensions, add transparency
- **Aseprite** (paid): Pixel art editing, grid alignment, animation preview
- **Photoshop**: Professional editing, precise cropping
- **Paint.NET** (free, Windows): Simple edits, transparency support

---

## **EXAMPLE: Complete Character Prompt Set**

Here's a complete set of prompts for one character:

**Character Concept**: "Nova" - Cyberpunk Hacker

### 1. Concept Art
```
Create a character reference sheet for an RPG character. Full-body front view, side view, and back view on white background. Character design: Female cyberpunk hacker "Nova", age 22, purple mohawk with neon pink highlights, augmented reality goggles on forehead, black leather jacket with circuit board patterns, fingerless gloves with hacking tools, ripped jeans with holographic patches, combat boots with LED soles. Color palette: black, purple, neon pink, cyan. Include color swatches. Anime/JRPG art style. 1920x1080 pixels.
```

### 2. Face Portrait Sheet
```
Create an RPG character portrait sprite sheet with EXACT dimensions 576 pixels wide by 288 pixels tall. The sheet must contain exactly 8 character face portraits arranged in a perfect 4x2 grid (4 columns, 2 rows). Each individual portrait must be exactly 144x144 pixels with NO gaps or padding.

Character: Female cyberpunk hacker "Nova", age 22, purple mohawk with neon pink highlights, augmented reality goggles on forehead (glowing cyan lenses), black jacket with circuit patterns, piercing green eyes, mischievous expression, pale skin.

The 8 portraits show: Neutral smirk, Happy grin, Sad frown, Angry scowl, Surprised wide eyes, Worried anxious, Determined focused, Very shocked gasping.

Art style: Anime/JRPG portrait, shoulder-up view, consistent character across all 8 faces.

Technical: PNG with TRANSPARENT background, each face 144x144px, total 576x288px, no gaps, pixel-perfect grid.
```
Save as: `Nova.png` in `img/faces/`

### 3. Walking Sprite (Single Character)
```
Create a top-down RPG character walking sprite with EXACT dimensions 144 pixels wide by 192 pixels tall. 3x4 grid of 48x48 pixel frames.

Row 1: Walking DOWN - left foot, center, right foot
Row 2: Walking LEFT - left foot, center, right foot
Row 3: Walking RIGHT - left foot, center, right foot
Row 4: Walking UP - left foot, center, right foot

Character: Female hacker "Nova" with purple mohawk, AR goggles on head, black jacket, jeans, boots. Character 36 pixels tall.

Art style: Top-down pixel art, clean outlines, vibrant purple/pink/black colors.

Technical: PNG, TRANSPARENT background, 144x192px total, 48x48px frames, 3x4 grid, no gaps.
```
Save as: `$Nova.png` in `img/characters/`

### 4. Battle Sprite
```
Create a side-view RPG battle sprite sheet with EXACT dimensions 576 pixels wide by 384 pixels tall. 9x6 grid, 64x64 pixel frames, 54 total frames.

Character: Female hacker "Nova" in side-view, purple mohawk, AR goggles glowing cyan, black jacket with circuits, holding holographic tablet/hacking device, 50 pixels tall, facing RIGHT.

18 battle motions in exact order:
Row 1: Walk, Wait (typing on tablet), Chant (tablet glowing)
Row 2: Guard (digital shield), Damage (recoil), Evade (quick dodge)
Row 3: Thrust (forward hack beam), Swing (wide hologram slash), Missile (shooting data packet)
Row 4: Skill (deploying drone), Spell (casting code matrix), Item (pulling device)
Row 5: Escape (running), Victory (fist pump), Dying (collapsing)
Row 6: Abnormal (glitching), Sleep (sitting), Dead (lying down)

Art style: Anime JRPG side-view sprite, dynamic poses, cyan/purple glow effects.

Technical: PNG, TRANSPARENT background, 576x384px, 9x6 grid, 64x64px frames, faces RIGHT.
```
Save as: `Nova.png` in `img/sv_actors/`

---

**You now have complete, copy-paste-ready prompts for generating all character assets!**

Good luck with your "Pharmageddon" character creation! 🎮
