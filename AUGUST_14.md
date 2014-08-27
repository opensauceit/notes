#Notes
First meet-n-code was held at the [Camden Collective space]( http://camdencollective.co.uk/)
We decided to kickstart with building N.I.B aka Nodeschool in a box, a platform which allows people to run nodeschool and similar workshops in the browser without having to set up anything.

The aim was to create the fastest and most streamlined way for people to learn Node without the overhead of having to install it. Imagine you've never operated a console before, how can you learn back-end javascript quickly?

![notes](https://dl.dropbox.com/s/r6qw02nwu0w33fl/IMG_20140821_192643.jpg?dl=0)

#Architecture

Front-end has a list of courses available for the student to take. It holds the notes and instructions and an area where the student can write the code. The user's input is passed on to middleware through the API, which sanitise some of it and hands it to the backend. The backend executes the code in a docker container (spawned at execution time) and returns success or fail as the output to the middleware. 
