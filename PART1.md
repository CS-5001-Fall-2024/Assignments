# Song Finder - Part 1 - Project 5
### Due Tuesday, December 3, 2024

This project requires the following concepts:

- Classes
- File I/O
- JSON Processing
- Software Development Techniques

### Overview

For this assignment, you will build a command line application to enable processing and searching of the [Million Song Dataset](http://millionsongdataset.com/lastfm/)

The data is comprised of a set of JSON files where each file contains metadata about a single song. The metadata includes the song title, artist, a list of tags (e.g., pop or alternative), and a list of similar songs. The full dataset is very large, but you will use the subset available here: [http://millionsongdataset.com/sites/default/files/lastfm/lastfm_subset.zip](http://millionsongdataset.com/sites/default/files/lastfm/lastfm_subset.zip)

If the link above doesn't work for you, you may need to copy/paste it into your URL bar and explicitly accept download from an insecure site (note the http rather than https). 

Your program will first load all of the songs into a data structure in memory. A portion of your grade will depend upon how you design your data structure for efficiency.

Once the data has been loaded into memory, you will present the user with a menu of options for searching and viewing the data. You will allow the user to select a command (e.g., search by artist); enter the information necessary (e.g., the artist name); and display the result. The program will allow the user to continue to search and view the data until they wish to exit the program.

### Design Requirements
The design of the data structure is up to you, but the following elements must be present in your design.

1. There must be a `Song` class that stores information about a single song. The properties of this class might include artist, title, and a data structure to store all tags associated with the song. You will instantiate a `Song` object for every JSON metadata file in the dataset.
2. There must be a `SongLibrary` class that uses one (or more!) data structures to store all of the `Song` objects. This class will provide methods to add new songs to the library and to search or access data in the library. It is likely that the methods of this class will map to the Functionality Requirements described below. Consider how to ensure that each method can be implemented efficiently!
3. Your main function will be in a file `song_finder.py`. The program will expect, at minimum, a command line parameter specifying the location of the top-level lastfm_subset directory, i.e., the program will be run as follows: python3 song_finder.py <directory_name>

### Functionality Requirements
1. **Search by artist:** If the user chooses to search by artist, you will ask the user for an artist (e.g., Phil Collins) and display all songs by that artist. The display must include, at minimum, the title of the song. 
2. **Search by tag:** If the user chooses to search by tag, you will ask the user for a tag (e.g., pop) and display all songs with that tag. The display must include, at minimum, the title and artist of the song.
3. **Most popular tags:** If the users chooses to view the most popular tags, you will display 10 tags that are most frequently used. In other words, you will  determine how many songs each tag is associated with; sort the tags based on that number; then display the 10 tags that map to the largest number of songs. The display must include the tag and number of songs that are tagged with that value.
4. **Show artists with more than `<n>` songs:** If the user chooses to show artists with more than `<n>` songs, you will ask the user to enter the value for `<n>`; retrieve all artists that have at least `<n>` songs; then display all artists and all songs by those artists. The display must include, at minimum, each artist name and the titles of each song by that artist.

### Testing Requirement
1. `SongTest`: you must include a module `SongTest` that appropriately tests
   your `Song` class. 
2. `SongLibraryTest`: you must include a module `SongLibraryTest` that appropriately tests
   your `SongLibrary` class. 
3. You may optionally provide additional test modules.

### Hints
1. It is strongly recommended that you implement methods in your `SongLibrary` that correspond the the Functionality Requirements. It is also strongly recommend that those methods do not print the result. Instead, return a data structure (e.g., a list) that contains the result (i.e., a list of `Song` objects where the artist is the artist specified by the search query). Have a separate function or other piece of code that will display the data in the result set. 
2. Though you may not copy large portions of your solution from the internet, it is expected that you will need to do some research and/or web searching as you develop your solution. It is also recommended that you discuss your design with your peers. 


## Assignment Submission

To earn credit for this assignment you must commit all of your changes to your GitHub repository prior to the deadline. It is strongly recommended that you commit your changes regularly. Do not wait until you complete all four parts of the assignment to upload your (partial) solution.

Step 1 - *Stage Changes*: Select the Source Control icon in the VSCode left menu. In the Changes section, click the + to *Stage All Changes*.

Step 2 - Commit Message: In the text box that says Message enter a meaningful message that describes the change you just completed.

Step 3 - *Commit & Push*: Select the down arrow in the blue box that says Commit. Choose *Commit & Push*.

Step 4 - Verify: Visit the repository on GitHub to confirm that your changes were uploaded successfully.