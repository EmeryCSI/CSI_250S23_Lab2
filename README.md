<div align="center">  
    <img src="Images/logo.jpg" alt="Logo">
    <h2>Renton Technical College</h2>
    <h3>CSI-250</h3>
</div>
<br>

# Lab 2 Enumerable methods and Bootstrap

## Purpose - The goal of this assignment is to develop your understanding of:
- The methods available for filtering data that are part of the Enumerable class
- Bootstrap to create responsive and professional looking UI

# Instructions

## Task 1: Clone this repository to your local machine and open the included .Net 6 MVC project (10 pts)
 - You notice that you have been provided an Album model located in the Models folder
 - There is also an AlbumList class that is located in the Data folder

## Task 2: Register the AlbumList.CS with the Services Collection using dependency injection. (10 pts)

- Create in interface IAlbumList.CS that will provide access to the GetAlbums() method inside of AlbumList.CS
- Use the interface to register the AlbumList with the services container

## Task 3: Create an Album Controller (30 pts)

- Use dependency injection to provide access to the AlbumList. Remember that the controller should rely on the Interface and not the concrete class.
- Create Endpoints and Views for the following:
    - Index() Action should display all of all Albums in the List in the Index View in a Bootstrap Table
    - Details(int id) Action should take an Id and display the Details View with info about the album with a matching ID
        - If no Album Matches the ID return NotFound()
    - Create() Action should give the user a Bootstrap HTML Form to create a new Album on GET. On POST Add the Album to the List
    - The Edit(int id) is like a combination of Details and Create. 
        - It is similar to Details in that it will take in an id and send an album to the view as a model. 
        - It is similar to Create in that it will have a GET and POST. 
        - Data will come back from the form to update the information about the album. Try to create Edit based on your knowledge of Create and Details. 

## Task 5: When complete create a commit with the note "Submission for Lab 2" and push the changes to the repository

# Tips for success
- Commit early and often. As you complete each step create a new commit.
- Refer to the example code and the weekly powerpoint
- Office Hours are Mondays and Fridays from 11a-1pm, if you are struggling with any of the assignments please come by.


Feel free to message your instructor or the TA on Canvas if you have any questions.
