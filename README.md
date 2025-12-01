# Updated: April 2025
# Before running the examples

1. Execute "npm i"

2. First, make sure you have a cloud.mongodb.com account and can access 
   the “Atlas” section.

3. In "Atlas" add a new database user by selecting under the “Security” title, 
   “Database Access.”.  There is a “+ ADD NEW DATABASE USER” option on 
   that page. Select "Password" authentication method. Make sure you 
   copy the user name and password as you will need it for the connection 
   string (uri) to connect from Node.js.

4. In "Atlas", under "Security", select "Network Access", "Add IP Address",
   and select the option that allows access from anywhere "ALLOW ACCESS FROM ANYWHERE".

5. In the code distribution, update the file credentialsDontPost/.env in the MongoDBCode 
   folder with the mongo connection string. This string can be found in MongoDB Atlas
   by selecting "Database", "Clusters", "Connect", "View full instructions" 
   under "Connection Configuration" select "Drivers" and select from the right
   pane under "Connection Instructions", Node.js under "Select driver". Follow
   steps #2 and #3. In step #3. under "Add your connection string into your 
   application code." you will find the connection string you need. Remember 
   to replace &lt;password&gt; in the string with the password associated 
   with the username that you created. The following is an example of how 
   the string might look like assuming terps and ABCD as username and 
   password, respectively.
   
   MONGO_CONNECTION_STRING = `mongodb+srv://terps:ABCD@cluster0.mmvm8.mongodb.net/?retryWrites=true&w=majority&appName=Cluster0`

5. To see databases, select “Clusters” under the “Database” title 
   and then click on the “Browse Collections” buttons.

6. You can create a database by selecting the “+Create Database” button.  
   For the examples below, you don’t need to create a database as a 
   database called “CMSC335DB” and a collection called “moviesCollection” 
   will be created when you run the example node .\insertMovies.js.  
   ** Run this example, before you run any other example **

7. After running the examples, you can drop (remove) the CMSC335DB 
   database by selecting the trash bin icon you see when you hover 
   over CMSC335DB.

8. The following examples illustrate CRUD operations.  They are recipes 
   that you can use for your project(s). The examples are: insertMovies.js,
   listAllMovies.js, lookUpMovies.js, listAllMoviesCursor.js, updateMovie.js, 
   updateMany.js, deleteMovie.js, deleteMany.js, clearCollection.js, 
   listDatabases.js, listCollections.js, 

