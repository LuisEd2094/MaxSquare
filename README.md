Gets Max Square from a .txt file.

This is a rewrite of 42's final proyect, originally written in C I have rewritten it in Python.

it will take any number of .txt files as arguments, check if they contain a valid map and set of instructions. If it's a valid map it will print the original map replacing the 'empty' characters in it
with the 'full' characters, displaying the Max Square possible. 

You can run the program in the terminal using your compiler of choice and the .txt files you want to check.

You can use the example files provided or use the mapgen.pl script to create new maps. The script requires 3 arguments, number of lines, lenght of lines and density of obstacles. It'd print out the map,
so it's best save the result to a new .txt file.

If the programn encounters an invalid map, it will print an error message explaining the error and move on to the next file if provided at time of execution.

Valid files are defined as:

All lines must have the same length
The characters on the map can only be those introduced in the first line
The amount of lines will be equal to the 'lines' defined in the first line of the .txt

Example of valid map: 

11.ox -> 11 = Lines in Map. '.' = 'empty' characters. 'o' = 'obstacle' character. 'x' = 'full' character.
o....o....
..........
...o...o..
....o..o..
...o......
.....o....
..........
o.o......o

Output: 

The biggest square for map example.txt is 3, located at 1, 0 coordinates: 
o....o....
xxx.......
xxxo...o..
xxx.o..o..
...o......
.....o....
..........
o.o......o

Example of Invalid Map:

5.ox
.....
.....
...o.
..o..
eeeee

Output: 

Characters in map not equal to characters in information line. "Name of file" is an invalid map.

Cheers!