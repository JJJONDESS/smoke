# Melt9 AR Menu - simple pizza + realistic steam (v32)

Based on the clean v23. No dome, no glass box, no cylinder,
no base, no logo plate - just the pizza, appearing when the
camera sees the target photo, with realistic steam rising
from it, like the Dosa / Naan video.

Steam (dishes/steam.png, 4 planes in index.html, search "STEAM"):
- thin white wisps, not a solid grey blob
- very low opacity (max 0.26-0.30), pizza stays visible
- 4 wisps, different speeds (3.4-4.2 seconds) and different
  start delays (0 / 0.9 / 1.8 / 2.7 seconds), so the steam
  never moves in one big block
- each wisp fades in as it leaves the pizza and fades out
  at the top, then starts again
- steam rises straight up on screen, it does NOT spin
  with the pizza

Kept from v23: fixed AR label (dish name + price, only on
targetFound), Add to cart + Photo in AR, 1-second flash,
auto-spin that pauses while you touch the pizza, soft
shadow under the pizza, self-hosted libs/ engine.
iOS (Quick Look) + Android (MindAR camera scan).

To change the steam: in index.html, search "STEAM".
Stronger = raise "to: 0.30" in the fade lines (try 0.40).
Thinner = smaller width (try 0.22). Faster = smaller dur.
