# Description
For this Project I used PHP, MySQL, Ajax, and Jquery. 
<br>
Team member names: Mauricio Macias, Maria Diaz. 
<br>

# Short introduction and explanation of each team member's contributions <br>
Mauricio Macias: Separated css elements to their own css stylesheet and created references to that file within the code. Wrote the index.html interface and color randomization code. Correctly stored username and color into the database. Added color stylesheet changes with div in client.js. This changed the rectangle portion of the message bubble to match the randomized color. <br>

Maria Diaz: Imported the Ajax chat source code to the school server. Changed username, db, and password to match correct server location. Added username and color columns to database. Changed border-color in css to a css variable and added access to change the variable in div in client.js. This changed the triangle portion of the message bubble to match the randomized color. Created the readme.txt file. <br>
			
Both parties contributed to trouble shooting, planning, and testing of the database. <br>

# Wireframe

![](img/name.png)
<br>
<br> user enters username before entering the chat room and randomly is selected a color for their chat bubble.
<br>
![](img/chat.png)
<br>
<br> Group chat with participants identified by name and color. 
<br>
# Database Design
<br>
CREATE TABLE `chatlog` ( <br>
  `id` int(11) NOT NULL, <br>
  `message` text NOT NULL, <br>
  `sent_by` varchar(50) NOT NULL, <br>
  `date_created` int(11) NOT NULL, <br>
  `username` varchar(50) NOT NULL, <br>
  `color` varchar(10) NOT NULL <br>
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4; <br>
