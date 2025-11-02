# Transparency Requirements for RPG Maker MZ Assets

## Quick Reference

| Asset Type | File Location | Background Requirement | Why? |
|------------|---------------|------------------------|------|
| **Concept Art** | Reference folder (not in game) | ✅ White background OK | NOT used in game - reference only |
| **Face Portraits** | `img/faces/` | ⚠️ Transparent recommended<br>(solid color also works) | Optional - RPG Maker supports both |
| **Walking Sprites** | `img/characters/` | ❌ MUST be transparent | Required - walks on various map tiles |
| **Battle Sprites** | `img/sv_actors/` | ❌ MUST be transparent | Required - appears over battle backgrounds |

## Detailed Requirements

### ✅ Concept Art - White Background OK
**File Type**: Reference only (NOT in game directories)
**Background**: White or any color
**Why**: This is for your reference when generating other assets. It never appears in the game.
**Example**: Character reference sheets showing front/side/back views

---

### ⚠️ Face Portraits - Transparent Recommended
**File Location**: `img/faces/`
**Background Options**:
- **Recommended**: Transparent PNG (most consistent)
- **Also Works**: Solid color or gradient background

**Why**: Face portraits appear in dialogue boxes and menus. RPG Maker can handle both transparent and non-transparent faces. However, transparent is recommended for consistency with other assets.

**How to Generate**:
- In AI prompt, specify: "PNG with transparent background"
- Alternative: "PNG with dark [color] background"

---

### ❌ Walking Sprites - MUST Be Transparent
**File Location**: `img/characters/`
**Background**: MUST be fully transparent PNG
**Why**: Characters walk over map tiles with different colors and patterns. If the sprite has a background, you'll see a colored box around the character.

**Critical**:
- Always specify in AI prompt: "PNG with TRANSPARENT background, NO white or colored background"
- After generation, verify in image editor that background is transparent (alpha channel)
- If AI generates with background, manually remove it using GIMP/Photoshop

**What Happens If Not Transparent**:
```
❌ With white background: [White box] around character on map
❌ With colored background: [Colored box] around character on map
✅ With transparent: Character blends perfectly into map
```

---

### ❌ Battle Sprites - MUST Be Transparent
**File Location**: `img/sv_actors/`
**Background**: MUST be fully transparent PNG
**Why**: Battle sprites appear over various battle backgrounds. Non-transparent backgrounds will show as boxes behind the character.

**Critical**:
- Always specify in AI prompt: "PNG with TRANSPARENT background"
- Verify transparency in image editor
- Character should blend into battle background seamlessly

---

## How to Verify Transparency

### In Image Editor (GIMP/Photoshop):
1. Open the PNG file
2. Look for checkerboard pattern in background (indicates transparency)
3. Check Layers panel - should show "Alpha" channel
4. Areas around character should be transparent, not white/colored

### In RPG Maker Playtest:
1. Start playtest (F12)
2. For walking sprites: Character should have NO box around it on map
3. For battle sprites: Start battle, character should blend into battleback
4. For faces: Face should appear cleanly in dialogue boxes

---

## Fixing Non-Transparent Assets

If AI generates assets with backgrounds instead of transparency:

### Using GIMP (Free):
1. Open the PNG file
2. Right-click layer → Add Alpha Channel
3. Use "Select by Color" tool
4. Click the background color
5. Press Delete
6. Export as PNG with transparency enabled

### Using Photoshop:
1. Open the PNG file
2. Use Magic Wand tool to select background
3. Press Delete
4. Save As → PNG with transparency

### Using Paint.NET (Free, Windows):
1. Open the PNG file
2. Use Magic Wand tool (tolerance ~30%)
3. Select background
4. Press Delete
5. Save (PNG format automatically saves transparency)

---

## AI Prompt Reminders

### For Face Portraits:
```
Technical requirements: PNG format with TRANSPARENT background...
```

### For Walking Sprites:
```
Technical requirements:
- PNG format with TRANSPARENT background
- NO white or colored background
- Character should be surrounded by transparency
```

### For Battle Sprites:
```
Technical requirements:
- PNG format with TRANSPARENT background
- Character appears over various battle backgrounds
- Ensure alpha channel transparency
```

---

## Summary

✅ **Concept Art**: White background is fine (reference only)
⚠️ **Faces**: Transparent recommended (solid color also works)
❌ **Walking Sprites**: MUST be transparent
❌ **Battle Sprites**: MUST be transparent

**When in doubt**: Use transparent PNG for all in-game assets!
