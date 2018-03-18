# diagrams-braille

Functions for rendering diagrams to Braille.

```
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣠⠴⠚⠉⠉⠉⠉⠉⠓⠦⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣠⠞⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠳⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢰⠃⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠘⡆⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⣀⣠⠤⠤⠤⠤⢤⣀⣏⣠⠤⠤⠤⠤⢤⣀⣀⣀⡤⠤⠤⠤⠤⣄⣹⣀⡤⠤⠤⠤⠤⣄⣀⠀⠀⠀⠀
⠀⢀⡴⠚⠁⠀⠀⠀⠀⠀⣠⠞⣟⠦⡀⠀⠀⠀⣠⠖⠉⠲⣄⠀⠀⠀⢀⡴⣻⠳⣄⠀⠀⠀⠀⠀⠈⠓⢦⡀⠀
⢠⠞⠀⠀⠀⠀⠀⠀⢀⡞⠁⠀⢹⡀⠙⣆⠀⡼⠁⠀⠀⠀⠈⢧⠀⣰⠋⢠⡏⠀⠈⢳⡀⠀⠀⠀⠀⠀⠀⠳⡄
⡟⠀⠀⠀⠀⠀⠀⠀⡼⠀⠀⠀⠀⠹⣄⠘⣾⠁⠀⠀⠀⠀⠀⠈⣷⠃⣠⠏⠀⠀⠀⠀⢧⠀⠀⠀⠀⠀⠀⠀⢳
⡇⠀⠀⠀⠀⠀⠀⣠⡷⠒⠋⠉⠉⠉⠛⣳⣿⣒⡋⠉⠉⠉⠙⣒⣿⣞⠛⠉⠉⠉⠙⠒⢾⣄⠀⠀⠀⠀⠀⠀⢸
⡇⠀⠀⠀⠀⣠⠞⠁⢧⠀⠀⠀⠀⢠⠞⢁⣿⠉⢯⡉⠉⢉⡝⠉⣿⡈⠳⡄⠀⠀⠀⠀⣼⠈⠳⣄⠀⠀⠀⠀⢸
⠹⡄⠀⠀⣰⠃⠀⠀⠘⣆⠀⠀⢠⠏⢀⡼⠈⢧⠀⢹⣀⡏⠀⡼⠁⢧⡀⠹⡄⠀⠀⣰⠃⠀⠀⠘⣆⠀⠀⢠⠏
⠀⠘⢦⡀⣇⣀⣤⠤⠤⢬⣧⣄⣟⣠⣾⠤⠤⠬⣷⣄⣿⣠⣾⠥⠤⠤⣷⣄⣻⣀⣼⡥⠤⠤⢤⣀⣸⢀⡴⠋⠀
⠀⠀⣠⠟⡟⠦⠤⣤⣤⡤⣤⠟⡟⢷⡤⢤⣤⡤⢤⠾⣿⠷⡤⢤⣤⣤⢤⡾⢻⠻⣦⢤⣤⣤⠤⠴⢻⠻⣄⠀⠀
⢀⡞⠁⠀⢳⠀⠀⠀⢀⡼⠁⠀⢹⡀⠙⣆⠀⡴⠋⢠⠿⡄⠙⢦⠀⣰⠋⢀⡏⠀⠈⢧⡀⠀⠀⠀⡾⠀⠈⢳⡀
⡞⠀⠀⠀⠈⢣⡀⠀⡼⠁⠀⠀⠀⠳⡄⠸⣾⠁⣠⠏⠀⠹⣄⠈⣷⠇⢠⠞⠀⠀⠀⠀⢧⠀⢀⡜⠁⠀⠀⠀⢳
⡇⠀⠀⠀⠀⠀⠙⠦⣇⡀⠀⠀⠀⠀⠈⣲⣿⡞⠓⠋⠉⠙⠚⢳⣽⣖⠁⠀⠀⠀⠀⢀⣸⠴⠋⠀⠀⠀⠀⠀⢸
⡇⠀⠀⠀⠀⠀⠀⠀⣇⠉⠙⠓⠒⢛⡽⢉⣷⠉⠉⠓⠒⠚⠉⠉⣾⡙⢫⡛⠒⠚⠋⠉⣸⠀⠀⠀⠀⠀⠀⠀⢸
⠹⡄⠀⠀⠀⠀⠀⠀⠸⣄⠀⠀⢠⠏⠀⡼⠙⣆⠀⠀⠀⠀⠀⣰⠋⢧⠀⠹⡄⠀⠀⣠⠇⠀⠀⠀⠀⠀⠀⢠⠏
⠀⠙⢦⡀⠀⠀⠀⠀⠀⠘⢦⡀⡞⣠⠞⠁⠀⠈⠣⣀⠀⣠⠜⠁⠀⠈⠳⣄⢳⢀⡴⠃⠀⠀⠀⠀⠀⢀⡴⠋⠀
⠀⠀⠀⠙⠲⠤⣤⣀⣀⣠⡤⠽⡟⠧⣤⣀⣀⣀⡤⠼⠛⠧⢤⣀⣀⣀⣤⠼⢻⠯⢤⣄⣀⣀⣠⠤⠖⠋⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢻⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⡏⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢳⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⡞⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠙⠦⣄⠀⠀⠀⠀⠀⠀⢀⣠⠴⠋⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠉⠓⠒⠒⠒⠚⠉⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
```

This package provides a backend for Diagrams to render tactile Braille graphics.
Additionally, a small frontend command-line program called brldia is
provided which allows to create diagrams from a number of primitive
functions and optional arguments.  It basically exports a minimal
version of diagrams-lib to the command-line. See ``brldia --help`` for details.


