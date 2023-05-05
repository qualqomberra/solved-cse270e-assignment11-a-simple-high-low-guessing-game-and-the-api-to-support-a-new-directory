Download Link: https://assignmentchef.com/product/solved-cse270e-assignment11-a-simple-high-low-guessing-game-and-the-api-to-support-a-new-directory
<br>
Create a new directory called Assignment-11

Create a simple high/low guessing game and the API to support it.

Modify the random Number app so that it uses the express static middleware and also uses the bodyparser.json middleware.

Create the following API code in app.js

Get Random Number between range

/api/v1/random/:min/:max

{“result”:”YOUR RANDOM NUMBER”} or if errror

status=404

{“result”:”msg”}

Get Random Number between 0 and Max

/api/v1/random/:max

{“random”:”YOUR RANDOM NUMBER”} or if error

status=404

{“result”:”msg”}

Set Game Max in server. The server will let the user play high low and this call sets the maximum range for the game. /api/v1/game method: post

{“max”:”number”}

{“result”: “OK” } if error

status=404 result=”Error”

Test Number against number in Server /api/v1/game/:number

method: get jsonOut

{“result”: “HIGH” or “LOW”, or “MATCH”} if bad input status=404 result=”ERROR”

Create an index.html to play the game

Use very simple html. My html file is at the end of these instructions.

Create game.js that uses jquery to make calls to the API

Make sure your package.json has all the required modules

Run this server on port 3011 Make sure all your code is in git