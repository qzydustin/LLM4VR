# LLM4VR - VR Scene Dataset

This folder contains VR scene datasets organized by resolution, difficulty, scene, and lighting conditions.

## Folder Structure

```
LLM4VR/
├── original/              # Original resolution images
│   ├── easy/              # Easy difficulty scenes
│   │   ├── scene_1/
│   │   │   ├── light_on/     # 5 images: different viewing angles
│   │   │   ├── light_off/    # 5 images: different viewing angles  
│   │   │   └── flash_light/  # 5 images: different viewing angles
│   │   ├── scene_2/       # Same structure as scene_1
│   │   └── scene_3/       # Same structure as scene_1
│   ├── medium/            # Medium difficulty (same structure)
│   └── hard/              # Hard difficulty (same structure)
│
└── 512x512/               # 512×512 resolution compressed images
    ├── easy/              # Same structure as original
    ├── medium/
    └── hard/
```

## File Naming Convention

Format: `scene_{difficulty}_{scene_number}_{lighting_state}_{view_angle}.png`

**Lighting States:**
- `light_on` - Normal lighting
- `light_off` - No lighting
- `flash_light` - Flash lighting

**View Angles:**
- `front` - Front view (0°)
- `right_30` - Right 30° view
- `right_60` - Right 60° view  
- `left_30` - Left 30° view
- `left_60` - Left 60° view

**Examples:**
- `scene_easy_1_light_on_front.png`
- `scene_medium_2_light_off_right_30.png`
- `scene_hard_3_flash_light_left_60.png` 