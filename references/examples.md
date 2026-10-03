# Worked prompts and repairs

These original teaching examples illustrate prompt structure. They are not official samples or verified Kling 4.0 results. Adjust duration and feature settings in the selected generator.

## Text-to-video: product action

```text
An amber perfume bottle with a black cap stands on a pale stone counter beside a window. A hand enters, lifts the bottle, pauses briefly, then sets it down in the same spot. Medium close-up with a slow push-in. Warm afternoon side light and soft shadows. One continuous shot. Sound: a gentle glass tap and quiet room ambience.
```

The bottle is the subject; lifting and setting down are sequential beats. The camera has one clear movement. A specific commercial product may need a product reference rather than a text approximation.

## Image-to-video: subtle portrait motion

```text
The person blinks, turns slightly toward the window, and gives a small relaxed smile. A light breeze moves a few strands of hair. The camera stays fixed. Keep the same clothing and background. Sound: quiet room ambience; no dialogue.
```

Assumes the starting image is a portrait near a window. If it is not, change the direction of the turn instead of inventing a different starting scene. Omit sound instructions if the selected mode does not support audio.

## Image-to-video: product camera move

```text
The camera makes a slow, shallow orbit around the bottle. The bottle stays upright and stationary on the plinth. Window reflections move gently across the glass as the viewpoint changes. Preserve the bottle shape and label from the input image. Sound: quiet studio ambience.
```

Camera motion and object motion are separate. Avoid combining this with a direction that spins the bottle unless both movements are intentional.

## Dialogue: two speakers

```text
Two friends stand beside a closed cafe on a quiet evening street. Hold a medium two-shot with both faces visible. The woman in the blue jacket looks at the door and says in English, disappointed: "We missed it." After a brief pause, the man in the grey sweater smiles and replies in English: "There's another place around the corner." Only one person speaks at a time. Sound: clear dialogue and faint street ambience.
```

Use the actual character or reference labels if available. Shorten the lines if speech must fit a short clip. A named voice or voice reference belongs in the interface's supported binding workflow, not in invented syntax.

## Multi-shot: intended 30-second ad plan

Use only if the selected mode supports the duration, or split it into individual clips. Time labels communicate intent; important visual milestones can use matching keyframes when supported.

```text
Create a calm morning product sequence in the same sunlit kitchen. Keep the commuter's tan jacket and the navy travel mug consistent across shots.
0–6 seconds: Medium-wide shot. The commuter approaches the counter and reaches for the mug. Slow camera push-in. Soft morning light.
6–13 seconds: Cut to a close-up of the hands. The commuter lifts the mug and closes its lid with one deliberate movement. Pause briefly so the action is readable.
13–22 seconds: Cut to a medium shot beside the doorway. The commuter places the mug into an open bag, picks up the bag, and turns toward the door.
22–30 seconds: Cut to a separate product insert of the same mug on the kitchen counter. A gentle camera orbit reveals its shape, ending with a steady front view.
Sound: quiet kitchen ambience, a lid click, soft fabric movement and restrained instrumental music. No dialogue. Use clean cuts between the stated shots.
```

The final shot is a separate product insert. If the user needs continuous chronological action, replace it with a close-up of the mug being placed in the bag rather than implying it returns to the counter.

## Reference-led: assign asset roles

```text
Use the attached portrait for the creator's appearance and the attached product photo for the navy mug's shape and color. Use the attached motion clip only for its slow camera push-in. Place the creator at a bright kitchen counter. The creator lifts the mug, turns it slightly toward the camera, and sets it down. Keep the mug design and the creator's clothing consistent. Sound: quiet kitchen ambience, no speech.
```

Replace “attached portrait,” “product photo,” and “motion clip” with the real attachment labels. Check that the inputs exist and that the selected mode accepts those asset types. If only an image is supplied, do not silently assume a motion clip exists.

## Targeted prompt repairs

| Observed problem | Small revision to try |
| --- | --- |
| Unclear action | Name the actor, verb, and object instead of “cinematic movement.” |
| Unwanted camera motion | Start with “Fixed camera”; remove competing camera moves. |
| Distorted product | Check the product reference; simplify handling or rotation. |
| Wrong event order | Separate beats and transitions; align keyframes if available. |
| Rushed speech | Shorten the line or allocate more time to the speaker. |
| Barely animated image | Add visible movement for a named subject. |
| Unexpected scene change | Resolve contradictions between the starting image and requested action. |
| Overloaded prompt | Remove repeated style words that do not change action, framing, light, or sound. |

Change one instruction at a time when diagnosing an output. These edits are hypotheses to compare, not guarantees of model behavior.
