# IGN-Code-Foo-2018
Repo for IGN's Code Foo 2018 Application

[Link to Eli Dickerson's Introduction] (https://www.dropbox.com/s/z4qikkae1dgscqi/Pick%20Eli%20Dickerson%20for%20IGN%20Code%20Foo%202018.docx?dl=0)

[Link to Building the Eiffel Tower with Geomags] (https://www.dropbox.com/s/hbntnh412ie63kc/Building%20the%20Eiffel%20Tower%20With%20Geomags.docx?dl=0)

###### [The Chicken Crosses the Road] (https://github.com/EliasDickerson001/IGN-Code-Foo-2018/tree/master/The%20Chicken%20Crosses%20The%20Road)

For The Chicken Crosses the Road, I created an interface that allows the user to add potholes to the grid themself. There is a solutions button that will display all possible paths for Henny Penny the chicken based on the potholes the user added to the grid. The grid is built at run time in the code and will display all paths each time the solutions button is pressed. Potholes can be added to any cell in the grid except the starting point, which is hard-coded in to the grid.

I implemented my solution to this project by using a recursive depth first search algorithm that travels through every valid node in the grid by testing the conditions of each cell's neighbors. As the program travels through the grid, it marks cells in the current path as visited to avoid causing an infinite loop. If a cell's neighbor has been visited, or is a pothole, it is not a valid cell to travel through. Once the program makes it to a cell on the far right of the grid, we print the current path to the browser since it is a possible path that Henny can take to cross the road.

This same solution works with larger grids as well, but it is exponentially less efficient as the size of the grid increases.

###### [Front End Project] (https://github.com/EliasDickerson001/IGN-Code-Foo-2018/tree/master/Front%20End)

I chose to work on the front end project, and matched the provided design as close as I could. I added 2 additional features that were not explicitly shown within the example design: 
- When the user chooses to load more videos/articles in to the browser, I chose to implement a scroll bar for viewing the additional content instead of increasing the size of the page. This functionality allows the VIDEOS ARTICLES menu and LOAD MORE button to always stay in the user's view, so they do not have to scroll up or down unnecessarily to find these page elements.
- When the cursor hovers over a thumbnail image for either a video or article, a tooltip will display that reiterates the title of the content.
