# Bipartite Graph and Suggestion Algorithms in C 

[HASAN ALPER AYAZ] [12.12.2024]

-------------------------------------------------------------------

For the project to run, the file "interactions.txt" delivered with the source code must be located in the same directory as the project; the project must be compiled and executed in the directory where it resides.

gcc main.c -o a
./a

-------------------------------------------------------------------

In its submitted state, the project functions as an interactive menu when executed. The menu instructions describe its behavior. Non-numeric inputs break the program.

The maximum number of recommendations to be made is defined as MAX_RECOMMEND at location l10.

-------------------------------------------------------------------

To see all available recommendation algorithms for the user USER defined at location l7, instead of the interactive menu:

- Comment out the menu call at location l750.
- Uncomment the lines between l753 – l766 (inclusive of both ends).
- Compile and run the program as described above.

-------------------------------------------------------------------

Additionally, to run the function that starts from the source user and takes a random walk for STEPS number of steps (defined at location l12), and displays these steps together with the final node reached:

- Uncomment lines l769 and l770.
- Compile and run the program as described above.

-------------------------------------------------------------------

EXTRAS:

Within the source code file, some print commands are provided in comments that supply information about the methods used by the recommendation algorithms or help test the correctness of this information. To view these helper routines and learn more about them, the word "UNCOMMENT" should be searched in the source file. 
[All these helper codes are for debugging purposes and may produce outputs that are not user-friendly!!]

Information about the helper codes can be obtained from the source file or followed through the list below. 
[* marks relatively long output / ** marks very long output]

- [l288] UNCOMMENT 1:
Shows the ratings of the films recommended to the user.

- [l294] UNCOMMENT 2*:
Shows the ratings of all films present in the graph.

- [l320] UNCOMMENT 3:
Shows how many common films the user shares with the other user who has the highest number of common films.

- [l342] UNCOMMENT 4:
Shows how many points the other user (who shares the most films with the user) gave to the recommended movies.

- [l438] UNCOMMENT 5**:
Shows the weighted distance calculated for the currently processed user, the ratings they gave to the movies they watched, and the total weighted distance obtained if those movies were reached through this user.

- [l444] UNCOMMENT 6**:
Shows updates made on the Distances list together with movie IDs.

- [l467] UNCOMMENT 7*:
Shows the users visited while traversing the graph to find the shortest weighted distances.

- [l475] UNCOMMENT 8*:
Shows the weighted distance of all users to the source user.

- [l482] UNCOMMENT 9*:
Shows the weighted distance to all movies that the source user did not watch.

- [l494] UNCOMMENT 10:
Shows the weighted distance of the recommended movies to the user.

- [l539] UNCOMMENT 11:
Shows the user who has at least MIN_COMMON common movies (defined at l11) and has the most similar ratings to the current user, along with the average difference per movie between their ratings.

- [l553] UNCOMMENT 12:
Shows the ratings given to the recommended movies by the user with the most similar taste.

- [l752] UNCOMMENT 13 and [l768] UNCOMMENT 14:
Contain the options explained above related to program behavior.
(Using predefined output instead of a menu / Showing the random walk path)

-------------------------------------------------------------------