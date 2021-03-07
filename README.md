# Phonebook-solution-HACK-THE-BOX
Phonebook challenge password matching program

On the main page, we see a message from one of the site's admins - Reese. we also see the message that the username and password are suitable from the workstation.

After Googling, we will see that the * character can replace any characters. Trying to log in with a username Reese and password *.

We get to the phone book page. Now the task is to find the full Reese password.

We write a program that sends POST requests to the /login page with the data username=Reese and select password.

We take each character in turn from the ASCII table, add * to it and check it in the POST request. If we have a redirect to /, then the symbol is correct. Add the next one to it in turn with * at the end and continue the selection until the last character is } (from the task condition).

Enjoy!


