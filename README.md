## CS150 Assignment 5

Hotel Occupancy Summarizer

**Points**: 35

**Goals:**

1. Continue working with external data files

2. Write C++ code that uses nested loops

You have just been hired by the Swynn Hotel in Las Vegas to help them
determine their occupancy rate. The manager at Swynn would like you to
print out a report that shows for each floor, the number of rooms on the
floor, the number of occupied rooms, and the number of unoccupied rooms.
The report must also list the total number of rooms, the total number of
occupied rooms, and the total number of unoccupied rooms. Finally, the
report must display the percentage of occupied rooms and the percentage
of unoccupied rooms.

The data that has been provided for you is in a text file named
"hotel.txt" and includes a series of lines of data. The first line
contains the number of floors in the hotel. This is followed by a line
for each floor in the hotel containing the number of rooms, then a
series of zeros or ones indicating if each room is occupied (one) or
unoccupied (zero).

For example, if a hotel has two floors, floor 1 has 5 rooms, 3 of which
are occupied, and floor 2 has 3 rooms, none of which are occupied, then
the file could look like:

<pre>
2
5 0 0 1 1 1
3 0 0 0
</pre>

The hotel manager also wants your program to account for the fact that
there is no 13<sup>th</sup> floor at the Swynn. Most hotels do not have a 13<sup>th</sup>
floor as the number 13 is considered unlucky. Triskaidekaphobia is the
fear of the number 13! Instead of a 13<sup>th</sup> floor, the Swynn goes
straight from the 12<sup>th</sup> floor to the 14<sup>th</sup> floor.

**Notes:**

1.  Read the hotel data from a file called "hotel.txt".

2.  Minimally, a data file must consist of one line containing the
    number zero indicating that there are no floors in this hotel.

3.  There is no input from the user in this program. All of the data
    will be read from the input file.

4.  Make sure there are no magic constants, including inside the setw as
    the columns of information are each 13. The only magic constant that
    is allowed is 0 to initialize counters.

5.  Constants must be all in caps and constants must be declared before
    variables.

For the following input file:

<pre>
14
3 0 1 1
6 0 0 0 1 1 1
2 1 1
7 0 1 0 0 1 1 1
4 0 0 0 1
8 0 0 0 1 1 0 1 0
3 0 0 0
1 0
8 0 0 1 1 0 0 1 1
2 0 1
5 1 0 1 0 1
4 1 1 1 0
3 1 1 1
6 1 1 1 1 1 1
</pre>

Your program must produce the following output exactly:

<pre>
              *** Hotel Occupancy ***

        Floor        Rooms     Occupied   Unoccupied
----------------------------------------------------
            1            3            2            1
            2            6            3            3
            3            2            2            0
            4            7            4            3
            5            4            1            3
            6            8            3            5
            7            3            0            3
            8            1            0            1
            9            8            4            4
           10            2            1            1
           11            5            3            2
           12            4            3            1
           14            3            3            0
           15            6            6            0
----------------------------------------------------
        Total           62           35           27

Percentage of occupied rooms: 56.45%
Percentage of unoccupied rooms: 43.55%
</pre>

**If there are no floors in the hotel, produce the following output exactly:**
<pre>
              *** Hotel Occupancy ***

        Floor        Rooms     Occupied   Unoccupied
----------------------------------------------------
----------------------------------------------------
        Total            0            0            0

Percentage of occupied rooms: 0.00%
Percentage of unoccupied rooms: 0.00%
</pre>
**To complete this assignment, you must submit the following:**

1.  **An electronic Solution of your program on GitHub**

    a.  You are to click on the Assign05 GitHub Assignment Link on
        Moodle to accept this assignment as we've done in lab. Once
        accepted, code up a complete solution to the above assignment
        specification. Your complete solution is to be pushed to GitHub
        no later than the date and time specified above for your
        specific section. I will only grade your solution from the
        proper location on GitHub.

    b.  Pay attention to the example output above. Your program's output
        must look **exactly** like the example output! The spacing and
        newlines in your output must match exactly.

    c.  Make sure that your program compiles and runs correctly with no
        errors and no warnings. If you get any errors, double check that
        you typed everything correctly. Be aware that C++ is
        case-sensitive.

2.  **An electronic copy of your program is to be placed on Moodle**

    a.  See Lab01 for producing a pdf of your complete program. Once you
        have produced the pdf of your program and named the pdf your
        **punetid**, drop the pdf in the Assign05 folder on Moodle.

    b.  The pdf must be in the drop folder on Moodle by the time and day
        specified above. Anything submitted after that will be
        considered late.

**IMPORTANT:** This is not a last minute assignment. There is a reason
you have 12 days to complete this assignment. If you start this
assignment the weekend before it's due, there is a high likelihood that
you will not finish. Remember also, the tutors are not going to write
your code. They will help with a specific issue in your program.

> **Good luck! And remember, if you have any problems, come and see
> straight away. **
