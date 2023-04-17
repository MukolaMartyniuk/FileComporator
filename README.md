# FileComporator
A program for comparing text for plagiarism
A program for checking text for plagiarism. Documents in .doc and .txt formats are checked. For the program to work, you must have React, Java, Spring, MySQL.
1. Installation of the necessary means.
1.1. Install MySQL Community Server 8.0.27 database server (https://downloads.mysql.com/archives/installer/). Only the server can be installed. It is important to remember the username and password.
1.2. Install the latest version of the IntelliJ IDEA (Ultimate Edition) development environment (https://www.jetbrains.com/idea/download/#section=windows).
1.3. Install Node.js 17.3.0 (https://nodejs.org/uk/download/releases/).
1.4. Install the mail server maildev. To do this, enter the command npm install -g maildev in the command line.
1.5. Install Java JDK 17.0.2 (https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html).

2. Launch the application.
2.1. Start the MySQL Community Server database server.
2.2. Starting the server part of the application.
2.2.1. Open the filecomparator folder in IntelliJ IDEA.
2.2.2. Go to "File -> Project Structure.. -> Project", select the previously installed JDK 17 version.
2.2.3. Go to application.yml, find spring -> datasource-> username/password. Enter the username and password you specified when installing MySQL Community Server. A good tone would be to encrypt the password, for this Jasypt is used with the algorithm PBEWithMD5AndDES and with the keyword Salah.
2.2.4. Start the application server by clicking on "Run".
2.3. Starting the mail server.
2.3.1. To start the mail server, enter maildev in the command line and go to the page in the browser (http://0.0.0.0:1080/).
2.4. Launching the client part.
2.4.1. Open the filecomparator-front folder in IntelliJ IDEA.
2.4.2. Open the Terminal tab in IntelliJ IDEA.
2.4.3. Enter npm install and press "Enter".
2.4.4. Enter npm start and press "Enter".
2.4.5. After that, a web browser will open with the application.
