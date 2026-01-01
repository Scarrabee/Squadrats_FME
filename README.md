# Squadrats_FME
FME workspace for Processing Squadrats KML Files: Generating Yards and übersquares
OR: FME version of this phyton script with the addition of übers: [https://github.com/matthew-conner/Squadrat-Extension/blob/main/README.md](https://github.com/matthew-conner/Squadrat-Extension/blob/main/README.md)

**Version 0.5 - 01/01/2026**
- It aint pretty but it works!
- über part is still wip

**How it works:**
1. The process starts by importing the Squadrats KML file. You can download the KML file from the Squadrats map: [Squadrats](https://squadrats.com/map)
2. FME reads the KML features (squares) and analyzes their spatial relationships.
3. The workspace checks each square to determine if all four neighboring squares (North, East, South, West) are also visited. This spatial analysis is essential for identifying "yards". "Yards" are defined as contiguous regions where each square has all four neighbors visited.
4. The workspace also looks for "Ubersquares" or squares of squares. For example an übersquadrat of 5x5 contains the full grid of 25 squadrats, 5 in ea. direction.
5. You get a KML export of the result

**Requirements**
- FME licence. Created in FME


**Credits**
-Based on data from [Squadrats](https://squadrats.com/map) - A game about exploring the world, one square at a time.
-[[https://github.com/matthew-conner/Squadrat-Extension/blob/main/README.md](https://github.com/matthew-conner/Squadrat-Extension/blob/main/README.md)](https://github.com/matthew-conner/Squadrat-Extension/blob/main/README.md#squadrats-local-yard-finder)
