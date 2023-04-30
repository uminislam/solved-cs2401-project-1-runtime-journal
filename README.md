Download Link: https://assignmentchef.com/product/solved-cs2401-project-1-runtime-journal
<br>



As a runner I have, for years, kept a journal, in which I record the time and distance of every run. (I also record some other information, such as whom I was running with, and the weather, but we’re not going to worry about that here.) For this project I have designed a class, built on the MyTime class that you used in Lab 1, to hold the information about a single run. Your assignment is to development a running journal, that is, a container class for my runs.

Begin by copying MyTime.h, MyTime.cc, runtime.h, main.cc and runlog.txt into your working directory. You can get them from the Blackboard for this assignment or by copying them from the directory ~jdolan/cs2401/projects/project1 on prime.

Begin by writing the implementation for all the functions in the Runtime class. Please note that when we add, subtract, multiply and divide the runs we do these operations to both the time and the distance. Equality (==) means that both time and distance are the same. Also, doing equality of floating point numbers can be problematic, so it might be good to have the distance equal function call all distances that are within a tenth of a mile equal.

Now <u>you are to create a class</u> which has, as its primary private variable, an array capable of holding 200 of these runs. (Please declare the CAPACITY of 200 as a static const in your class.) You will also need a variable to keep track of how many of these spots are filled.

Your class will have:

<ul>

 <li>A default constructor</li>

 <li>A function that adds an additional run to the list – a run that is passed as a parameter</li>

 <li>A function that displays all the runs in the list to the screen</li>

 <li>A function that will allow the searching of a particular time, and display the first run that it finds that matches that time – this display should show distance and pace AND it should allow removal of this particular run in case it was recorded incorrectly.</li>

 <li>A function that will search for and display all the runs of a particular distance</li>

 <li>A function that will sort the array by time</li>

 <li>A function that will sort the array by distance</li>

 <li>A function that reports on the total time for all the runs recorded in the journal</li>

 <li>A function that reports on the total distance for all the runs recorded in the journal</li>

 <li>A function that reports on the average pace for all the runs in the journal</li>

</ul>

Also, all the data is saved to a back-up file that created when the program quits and then automatically reloaded (if the file is present) when the program restarts, thus saving the user from re-typing their data upon each entry. This data should be saved in the same format as I show in the runlog.txt file that I have given you.