# Map Testing

Hooray! You've just finished your map. It must be a great sense of accomplishment.
But before cheering up and call it a day, please test your map thoroughly before uploading to the Workshop to ensure the quality of the map and a fluid player experience.

Check out how to use maptest mode [here](/en/start/basic-operation.md#maptest).

## Flying Test

Tick all the boxes below:

- LevelInfo
- Cohesion and alignment
- Missing faces fixed
- Clipping and flickering fixed
- Object stacking and duplication fixed (especially keys and doors)
- Location of `GuardRail`(s)
- Coverage of `DeathBox`: Pay attention to sides or even ceiling under the circumstances of low-gravity, anti-gravity and super `JumpBox`(es).
- Arrangement of `LifeBall`(s): Are they accessible? Edge cases of _accidentally_ obtaining multiple lives in one section, or even life farming, are avoided?
- Tolerance regarding prop ball and box maneuvering, and gap handling

And some extras:

- Performance optimization: Limit the scale of decorations. Keep your map size under 1MB if possible.
- Style of decorations: Height of `Light`, location of `Pillar`
- Shortcut observation: Find out if there's any excessive shortcuts introduced by unexpected operations or routines, and determine whether to block them. (Especially cross-section keys ~~entering destination with 5 keys~~)
- In-between `DeathBox` check: Proper coverage? Accidental blockage of expected routes? Be aware: **DO NOT use `S_InvisibleRoad` or `DeathBox` to block routes or shortcuts!**
- Verification of precise mechanisms: If precision are required by any specific mechanisms (e.g. automatic map), put them on extensive tests to ensure them working properly.

## Test in Player Perspective

Don't use flying or skipping section functions for now, and walkthrough the whole map in player perspective.

Tick all the boxes below:

- Fully operational machinery. (Don't repeat the mistakes of _Ability Training 3_!)
- Difficulty control: Avoid wtf moments, e.g. <ruby>first-attempt pitfalls<rt>初見殺し</rt></ruby> or before-the-finish-line troll. Also, avoid super-duper-long sections.
- Logic check: Ensure a complete chain of reasoning. Provide adequate hints when necessary. Avoid counter-intuitive requirements (e.g. going across the bar of `M_TurnBoard2`, nonsense triggers). No more "room escape" clones.
- Player FOV check: Try out 4:3 resolutions, make sure all the necessary elements of puzzle solving are within player's field of view.
- Reach out to other map testers.
