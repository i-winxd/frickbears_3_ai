# Funtime Freddy

- Which side he is on is panned.
- There are voicelines when he appears in either hallway. They are **different** if the bonnie puppet is missing or not. Once he is in a hallway, he won't move until attacking.
- After Funtime Freddy announces an attack, the game, every frame does this:
    - If the correct door is closed and the other one isn't, this plays a sound and resets Funtime Freddy. He will not appear in the hallway anymore until he does again.
    - If both doors are closed, nothing happens, which means his state won't change. You must open the door the attack isn't happening on to reset him.
    - If the correct door isn't closed, a jumpscare occurs.
