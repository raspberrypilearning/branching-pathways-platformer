# Step Prerequisites

Steps that require another step to be completed first before they function, verified against the block scripts in each step file. A dependency is listed when the step's own blocks reference another sprite/mechanic (e.g. `touching (player v)?`), or the step text explicitly says so.

## Steps with prerequisites

| Step | Requires | Why |
|------|----------|-----|
| **4A / 4B / 4C – Move player** | Player (group 2) | Each opens with "Select the player sprite" — nothing to move until a player exists. |
| **5A – Jump/Fall (Keys)** | Movement (group 4) + Platforms (group 3) | Says "find your movement blocks"; jump uses `on ground` detection, so the player needs platforms to stand/land on. |
| **5B – Jump/Fall (Mouse)** | Mouse Move (4B specifically) + Platforms (group 3) | Says "find the mouse movement blocks you made earlier"; explicitly tells you to tune jump so the player can "land on the platforms above". |
| **7A – Place Collectables** | Player (group 2) | Scoring uses `if touching (player v)?` — needs a player to collect them. |
| **7B – Random Collectables** | Player (group 2) + Platforms (group 3) | Uses `touching (player v)?` to score and `touching (platform v)?` so collectables drop and land on platforms. |
| **7C – Add a Power Up** | Player movement (group 4); jump (group 5) only for the higher-jump variant | Works by changing `move speed` / `jump strength` in the existing movement script. |
| **8A – Get to Exit (Default)** | Exit sprite (group 6) + Player (group 2) | Selects the player sprite and wins on `touching (Exit v)?`. |
| **8B – Target Score** | Collectables (7A or 7B) | File explicitly says to add collectables first — nothing raises `Score` otherwise. (Player/platforms come transitively via the collectables.) |
| **8C – Take Key to Exit** | Exit sprite (group 6) + Player (group 2) + a Key | Wins only after the player collects the key and reaches the exit. (Key is added within this step.) |
| **9A / 9B / 9C – Hazards** | Player (group 2) | Harm the player via `touching (player v)?`. (9B/9C may optionally duplicate 9A — not required.) |
| **10C – New Level** | Platforms (group 3) + a win condition (any of group 8) | Switches level "when the player meets the win condition". |
| **10D – Animate your player** | Player (group 2) + Movement (group 4) | Costumes switch *while the player moves*. |
| **10E – Make Your Player Sprint** | Player movement (group 4) | Modifies the existing `move speed` inside the movement `forever` loop. |

## No prerequisites (do anytime)

- **Group 1 – Backdrop** (1A / 1B / 1C)
- **Group 2 – Player** (2A / 2B / 2C)
- **Group 3 – Platforms** (3A / 3B / 3C)
- **Group 6 – Exit sprite** (6A / 6B / 6C)
- **10A – Add Music** (just the Stage)
- **10B – Add Sound effects** (attaches sound to an existing sprite/Stage; most useful once jumping, collecting, winning or hazards exist, but not blocked)
