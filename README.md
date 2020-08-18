# IART

## Compile and Run
Since the project was built in Python, the only requirement for running with the command line is having python3 installed in the OS - it is already built in Linux (or run in IDEs with Python extensions).

Compiling is not needed with Python, to run the application one must type: python3 main.py <<file_path>>

## How to use
The program is very simple and straight forward:
</br>
======================================== </br>
=========== Photo Slideshow ============</br>
</br>
|         1. Create Slideshow          |</br>
|         2. Quit                      |</br>
</br>
|   > Select 1</br>
</br>
|------------- Algorithms -------------|</br>
|        1. Hill Climbing              |</br>
|        2. Tabu Search                |</br>
|        3. Simulated Annealing        |</br>
|        4. Genetic Algorithm          |</br>
|        5. Quit                       |</br>
</br>
|   > Select  _
</br>

> Each algorithm requires fields that must be specified by the user. The fields and their default values and intervals are defined.</br>
   The option of saving the evolution of the algorithm's processing in a csv file is provided.</br>

For example, in Hill Climbing:</br>
|   > Define maximum number of iterations (over 100 ; 'default' for 1000; -1 for no limit): _</br>
|   > Limit number of initial state slides (None for no limit): _</br>
|   > Do you wish to save the development in csv format (y/n): _</br>
</br>

> Every algorithm during its processing prints the current state in a way the user can understand.</br>

For example, in Hill Climbing: </br>
------------------------------- </br>
Function name :  add_horizontal </br>
Node Score :  34 </br>
Number of photos: 150 </br>
Number of slides: 101 </br>
------------------------------- </br>
</br>

> Prints of different steps are also shown: </br>

get_initial_state (/home/meias/Work/GitHub/IART/DataStructure/Slideshow.py:208):</br>
    0.007 seconds </br>
// this referres to how much time was spent on developing an initial state</br>

hillClimb (/home/meias/Work/GitHub/IART/SearchTree/Node.py:67):</br>
    0.508 seconds </br>
// this referres to how much time was spent on the algorithm's processing </br>

> When a solution is determined, the following prints appear, describing the number of slides in the solution, the total score and the output file's name: <algorithm>_solved.txt </br>

--------------- Finished --------------- </br>
Solution: 101 slides </br>
Score: 35 </br>
--------- Creating output file --------- </br>
|   Output file: hillclimbing_solved.txt </br>



Note:
 - A few of the inputs don't have validation: for example, when the user inserts a string instead of an integer. </br>
 - There is a folder of test files called 'input' inside the Parser module.
