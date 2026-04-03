# Technical Roadmap (Baby Steps)

I’m going to lay this out in **phases** so you can work in 45-minute chunks.

---

## Phase 1 — Movement and World (you already started)

**Goal:** Walking around a world that feels like a place.

Tasks:

1. Player movement (done)
2. Camera follow
3. Tilemap for terrain
4. Collisions (trees, rocks)
5. Multiple terrain types (grass, forest, water, mountain)
6. Map boundaries
7. Simple day/night lighting
8. Footstep sounds
9. Wind / ambient sound

45-minute tasks examples:

* Add camera smoothing
* Add new terrain tile
* Add tree collision
* Add ambient forest sound
* Add day/night color shift
* Add map transition to second area

---

## Phase 2 — The Dryad Companion

**Goal:** She exists and follows you.

Tasks:

1. Dryad sprite
2. Follow player behavior
3. Idle animations
4. Occasionally walk ahead / behind
5. Simple speech bubble
6. Trigger dialogue when pressing key
7. Region-based dialogue (forest, river, hill)

45-minute tasks:

* Dryad follow script
* Idle animation
* Speech bubble UI
* Dialogue JSON file
* Region trigger zones
* Random idle dialogue
* Make her look at player when talking

---

## Phase 3 — Campfire System (Very Important)

**Goal:** Core gameplay loop exists.

Tasks:

1. Press key → place campfire
2. Campfire sprite + light
3. Sit animation
4. Campfire menu:

   * Talk
   * Sleep
   * Eat (later)
5. Longer dialogue at camp
6. Save game at camp
7. Fade to night when sleeping

45-minute tasks:

* Campfire object
* Light shader
* Sit animation
* Campfire menu UI
* Dialogue mode at camp
* Save system
* Sleep fade transition

Once this phase is done, **you have the core loop**:

> Walk → Camp → Talk → Sleep → Continue

That’s huge.

---

## Phase 4 — Memory System

This is what will make the Dryad feel alive.

You do NOT need AI memory magic. Just a simple system like:

```
memories = [
  "First camp",
  "Crossed the river",
  "Cold night",
  "Old ruins",
  "You picked many berries",
]
```

Then occasionally she references memories.

Tasks:

1. Memory list
2. Add memory when events happen
3. Campfire dialogue references memories
4. Dream triggers from memories

45-minute tasks:

* Memory JSON file
* Add memory when entering region
* Dialogue referencing memory
* Memory UI journal
* Random memory reflection at camp

---

## Phase 5 — Dreams / Faerie

**Goal:** First dream sequence.

Tasks:

1. Sleep → dream map loads
2. Dream movement (slower floaty movement)
3. Dryad leads, player follows
4. Strange dream environment
5. Wake up at camp
6. Unlock memory or map marker

45-minute tasks:

* Dream scene
* Dream movement physics
* Dryad path in dream
* Fade transition
* Dream dialogue
* Wake up transition
* Unlock memory after dream
