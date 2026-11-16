# MG6

1. The entire for loop will complete fully inside that single Update method before it finishes. Therefore, a heavy loop will block the main thread and cause the game to lag rather than spreading across mulitple frames.
2. The player can accidentally fall back down through the platform if their upward jump speed slows down before fully clearing the top edge. This happens because the collision logic turns back on prematurely based on position or input rather than waiting until the player is safely above the platform.
