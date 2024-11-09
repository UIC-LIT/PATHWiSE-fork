1. Install an Apache and MySQL server. XAMPP is a good option that comes as a bundle and compatible with all major OS: https://www.apachefriends.org/download.html
2. (Optional) Create a virtual host and put all the files from this repository at the root of this new virtual host. Example URL: pathwi.se or path.wise
3. Create a Database named "pathwise_prototype" with a username of 'root' and password ''. Copy of these details can be found at validate/index.php line no 32-35
4. Install the Open AI based Emotion and Comment Type classification system from here: https://github.com/UIC-LIT/misty-emot/ Update the origins value in the src/server/main.py file with the virtual host URL from Step 2. You may use "*" as value too for the staging/dev environemnt
5. Update the SERVER_URL variable at the begining of the following files: assets/main.js and assets/main-working.js of this repositry. The value should match the server URL you get from Step 4.
6. Update the misty_IP variable in assets/robot-play.js file with the appropriate robot IP
