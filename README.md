## Project 1 Essay

### tic tac toe

After spending much of project week struggling with game logic it became clear that I would not be able to meet many of the requirements for the submission deadline. I consulted with the instructors and my peers and came up with a new plan which allowed me to build a working game with legible code, but I fell short of API and Authorization specifications.

With the resubmission, API integration for authentication went smoothly since a previous class lesson had detailed the jQuery $.ajax() method for providing a user the ability to sign-up, sign-in, change their password and sign-out, all requirements for the project. The method takes a configuration object containing all the instructions jQuery requires to fulfill the request. In our case, those instructions included the API url, the type of CRUD action (POST, PATCH, DELETE) and the data entered by the user into the form.

For game-play API integration, the configuration object instructions for POST and GET are similar to those used for authentication, but they require the addition of Authorization headers so that the signed-in user's token can be used to save and retrieve all of their game statistics. The PATCH request also requires authorization along with additional information to log moves and game stats. Referring to the [Game Documentation](https://git.generalassemb.ly/ga-wdi-boston/game-project-api/blob/master/docs/game.md), I passed an object to the Ajax request containing data the API expects to receive.

While the game project is still a work in progress, I've included a GET request and fixed the modals to close upon submit success. I'll rewrite the documentation to include wireframes and user storie and continue to make improvements on the user experience.
