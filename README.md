# Weekend Challenge 2
### Technologies Implemented
* JavaScript/jQuery
* Node.js
* Express.js

### Front-end
#### Display
* Two values using input fields;
* Four command buttons to select the desired mathematical operation (e.g. addition, subtraction, multiplication, and division) to use on the two input values, and;
* A clear button that resets the input fields

#### Action/Logic
##### Client-side
The client submits a Ajax POST which places the:
* Two input values, and;
* The value of the selected mathematical operator into an object defined by the mathematical that is selected;
* The object is then sent to the server for calculation

##### Server-side
The server--configured on port 7500--receives POST requests:
* On URL-specific routes depending on the mathematical operator selected on the front-end;
* After converting the object inputs into numeric values, performs the requested/required mathematical operation, then;
* Performs a ```res.send``` of the result back to the client

Once the Server receives the request, it will compute the numbers in one of four different ways:

addition,
subtraction
multiplication
division
Once the result of the mathematical operation is determined, it should be sent back down to the Client where it will be displayed on the Front End.

HARD MODE

Create a calculator-like Front End!

Convert the input fields for the two values to buttons. This experience would allow the user to

click on a numerical button
click on a mathematical operator
click on a numerical button
click on an equal button that sends all of the information to the server
Remember, you will need to modify your Client logic to accommodate this new interface.

PRO MODE

Create a delay from when the Client receives the response from the Server, and when the calculation is actually displayed on the Front End:

The delay should be 3 seconds.
During that delay, show a message that says computing until the 3 second delay has finished, then remove the computing message while showing the calculation.
Submitting this Assignment
Create a README.md explaining what your application does
Submit via the assignment app

## Front-end/Client Functionality & Server Logic
IMPORTANT: The logic for the calculation needs to be implemented on the Server.