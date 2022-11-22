Gets Max Square from a .txt file.

This is a rewrite of 42's final proyect, originally written in C I have rewritten it in Python.

AIM OF PROJECT:

The aim of this project is to find the biggest square on a map, avoiding obstacles.
The map is made up of "empty" characters, lines and "obstacle" characters.
The aim of the program is to replace "empty" characters by "full" characters in order to represent the biggest square possible. A valid square size starts at 1x1.
If more than one valid square is available, it will display the one closest to the top and then most to the left.

USAGE:

You can run the program in the terminal using your interpreter of choice and the .txt files you want to check.
It will take any number of .txt files as arguments, check if they contain a valid map (valid maps will be defined later) and set of instructions.

VALID INSTRUCTIONS:

Valid instructions are defined as:

It will be the first line in the .txt file, which contains:

Number of rows in map followed by the 'empty' character, then the 'obstacle' character and finally the 'full' character.

Example of valid instruction line:

14.ox

14 = Number of rows
'.'= Empty character
'o'= Obstacle character
'x'= Full character

VALID MAPS:

Valid maps are defined as:

All rows in map must have the same length
The characters on the map can only be those introduced in the first line
The amount of rows will be equal to the 'number of rows' defined in the first line of the .txt
It must contain at least 2 lines, first one with Map information and second with at least a single valid character.



Example of valid map: 

8.ox -> 8 = rows in Map. '.' = 'empty' characters. 'o' = 'obstacle' character. 'x' = 'full' character.
o....o....
..........
...o...o..
....o..o..
...o......
.....o....
..........
o.o......o

Output: 

The biggest square for map "name of file" is 3, located at 1, 0 coordinates: 
Empty = .       Full = x         Obstacle = o
o....o....
xxx.......
xxxo...o..
xxx.o..o..
...o......
.....o....
..........
o.o......o

INVALID MAPS:

If the programn encounters an invalid map, it will print an error message explaining the error and move on to the next file if provided at time of execution.

Example of Invalid Map:

5.ox
.....
.....
...o.
..o..
eeeee

Output: 

Characters in map not equal to characters in information line. "Name of file" is an invalid map.

RANDOM MAP GENERATOR:

You can use the example files provided or use the mapgen.pl script to create new maps. The script requires 3 arguments, number of lines, lenght of lines and density of obstacles. It'd print out the map,
so it's best save the result to a new .txt file.


Cheers!

KNOWN ISSUES:

Needs to check instruction lines for repeated characters.
Needs to check if instruction line has all the needed information.
Needs to strip new lines at the end of file

3.+ 