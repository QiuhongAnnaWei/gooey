# Gooey

## Introduction
Gooey is a graphic design tool that helps streamline and enhance the process of selecting colors and fonts for designers. Powered by a machine learning palette recommendation algorithm, it aims both to make the execution of stylesheet making smoother and to support inventive exploration in the visual space for anyone. Our website meshes intellgient self-developed heuristics and user-specific soft clustering algorithm with an aesthetically appealing and intuitive user interface in the hope that we can make the design process more efficient, enjoyable, and imaginative.
<br/>

## Links
[Deployed App](https://powerful-forest-21960.herokuapp.com/)  
[More detailed README](https://powerful-forest-21960.herokuapp.com/about)  
[Figma Mocks](https://www.figma.com/file/5qDBB51FS1zYHBRXRJjSVm/Gooey?node-id=0%3A1)  

## Set Up

### To Develop:

In the `backend` directory, you will need to create your venv.

**For Macs:** <br/>
`python3 -m venv venv`<br/>
`. venv/bin/activate`<br/> 
or `source venv/bin/activate`<br/> 
`pip install flask python-dotenv firebase_admin`

NEW： Run `gunicorn run:app` in the root directory to run the app on port 8000.
You'll need to go into `frontend/src/constants.js` and comment in the 8000 variable to see
changes in the front end.

**For Windows:** <br/>
`py -m venv venv`<br/>
`source venv/Scripts/activate`<br/>
`pip install flask python-dotenv firebase_admin`

In the future, if you need to add more modules, you will need to activate your <tt>venv</tt> and <tt>pip install</tt> them.

Once finished, you should just be able to run
`flask run`
and see that the Flask app is running on port 5000.

To end the server, use CNTRL+C. 

To exit your venv, type
`deactivate`

NEW (untested sorry Minna) for windows： Run `flask run` in the root directory to run the app on port 5000.
You'll need to go into `frontend/src/constants.js` and comment in the 5000 variable to see
changes in the front end.


If you want to install all dependences, go to the root directory and go: `pip install -r requirements.txt`
<br/>
<br/>

### To Test:

Step 1) In the `backend` directory, activate the virtual environment and run Flask server 

For Mac: `. venv/bin/activate` , then
`flask run`

For Windows:
`py -m venv venv` , then
`flask run`

Step 2) Make sure that nose2 is installed (`pip install nose2`). In another terminal, go to the `backend` directory,
activate the virtual environment (like above) and run all tests using nose2.

For Mac: `. venv/bin/activate` , then
`nose2 -v`

For Windows:
`py -m venv venv` , then
`nose2 -v`

 
 IN SUMMARY: you will need two terminals on the virtual environment in which one runs the flask server
 and the other runs the tests via nose2. 

