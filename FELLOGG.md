# Fellogg

En rad per fel. Skriv medan du minns hur du gjorde.

| Nr | Vad stod i loggen? | Lokalt eller på GitHub? | Hur tog du reda på orsaken? | Hur löste du det? |
|----|--------------------|-------------------------|-----------------------------|-------------------|
| 1  | Invalid workflow file                   |Github                        |Github action reported the error on the line 11 but was easy to define that the indentation was wrong on one line                           |I correct the indentation removing a extra space and save the change                   |
| 2  |os imported but not used                    |github and local                         |The running uv run check src tests reported an unused os import                             |I delete the import os and saved the changes                   |
| 3  |Tow file reformatted                   |Github and local                        |running uv run ruff formatting --check src tests hade 2 formattings problems                             |correct the formatting such as extra line and commit che change                   |
| 4  |Modulenotfound error                   |Github and local                        |pytest could not run the test because in baseline.py where a import numpy but it wasn't installed                              |I run uv add numpy then uv run pytest and all test succeeded revaling a falling calculation. I fix the calculation and commit also the updated pyproject and the uv.lock (removing it from .gitignore)|
| 5  |assertations                   |local                        |pytest show that the resault in the function moving_average differed from the expected averages  |I modified the denominator of the funcion to (window) instead of (window + 1) then committed and pushed the change|

