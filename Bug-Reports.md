# Bug Reports – Advanced Parkour System

---

## BUG-01: Player Can Fall Outside the Playable Area Without Respawn

### Environment
- Engine: Unity 2023.2.20f1
- Platform: PC
- Build: Playable Demo

### Severity
High

### Priority
High

### Description
During gameplay, the player can jump from elevated rooftops and fall outside the intended playable area.  
Once outside the level boundaries, the character remains alive and can continue moving indefinitely, with no respawn, death, or recovery mechanism available.

### Steps to Reproduce
1. Start the demo and spawn on a rooftop
2. Move the character toward the edge of the building
3. Perform a jump toward the outer boundary of the level
4. Miss the intended landing and fall outside the map

### Expected Result
- The player should be respawned at a safe checkpoint  
OR  
- The player should be reset after falling outside the playable area

### Actual Result
- The player falls outside the level boundaries
- No respawn or recovery logic is triggered
- Gameplay enters an unintended state

### Impact
- Breaks intended gameplay flow
- Allows unintended exploration
- Reduces overall polish and player experience

### Evidence
- 🎥 Video (Full reproduction): [
ParkourSystem-BUG-01-PlayerFallsOutsidePlayableArea](https://www.youtube.com/watch?v=k_vOo7-qRrU)
- 🖼️ Visual preview (GIF): available in the `Evidence` folder

