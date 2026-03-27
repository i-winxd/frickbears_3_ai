# Withered Foxy

- Shows up after `round((900 / (AI + 10)) * random_range(0.75, 1.25))` seconds from being reset. (90 seconds on AI 0 (technically); 30 seconds on AI 20 on average, linearly interpolated in between, and some random noise is added)
- Will wait until Endo or Dreadbear are not at the window. 
- If he is in your window for a total of 18 seconds at AI 0, 8 seconds at AI 20 (linearly interpolated if inbetween), **with your flashlight off,** he jumpscares you. This is how long you can ignore him without flashing.
- Flashlight must be held for longer at higher AI levels