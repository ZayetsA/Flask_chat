Flask-SocketIO-Chat-application
===================
A simple chat application built with the Flask and SocketIO framework and MongoDB database.
After registration and authorization, the user can join the chat room, which he created himself, or in the room, to which he was invited by another user. The room creator has the ability to change his chat room: invite / remove users from it and change the name of the room. If the room is no longer needed, the room creator can delete it.
### ScreenShots
Sign Up:
![Sign Up](https://i.ibb.co/HYXFsqD/signup.png)
Login:
![Login](https://i.ibb.co/7gTnhYc/login.png)
Index page:
![index](https://i.ibb.co/DPBY9dN/index.png)
Room page:
![room](https://i.ibb.co/PCFyrGx/room.png)
Actions with rooms:
![create_room](https://i.ibb.co/gRg96XZ/create.png)
![edit_room](https://i.ibb.co/qN3XfpB/edit.png)
![delete_room](https://i.ibb.co/ggw4G6f/delete.png)
### Running the App

To get the app running:
 - Create a virtual environment:
 ```
 python3 -m venv env
 ```
 - Activate the virtual environment:
 ```
   source env/bin/activate
 ```
 On windows? Activate it with the below:
 ```
   env/Scripts/activate
 ```
 - Install the dependencies:
 ```
 pip install -r requirements.txt
 ```
 - Finally run the app:
 ```
  python app.py
 ```
 Congrats! The app should now be running on http://localhost:5000
 ### Notes
 User, room and message information is stored in the MongoDB database. I moved away from the task a little by choosing this base, because I really wanted to learn how to work with it a little, besides, its interface is convenient, and it exists at all. The key to the database is attached. Since the cluster is test, there is no point in hacking it, so hackers will not find anything there except a couple of test messages and simple users.
```
db_key: mongodb+srv://test_artem:1488@chatapp.jb5e0.mongodb.net/<dbname>?retryWrites=true&w=majority
```
