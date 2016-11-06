# SaveGMailAsEML

Do you want to save your GMail messages to local computer without third-party softwares? If yes, then you have come to the right repository. Welcome!

Video Demonstration - 

The software programs in this repository talk ONLY to Google and your data is not shared with anyone. The source-code is open and can be easily modified. In order to use this application, there are few prerequisities:

# 1. Localhost

You need to have localhost server. Many localhost servers are available. I have used WAMP. The website is http://www.wampserver.com/en/.

Here is a link to Youtube video showing how to install - https://www.youtube.com/watch?v=RZTYqTGqtjI.

Before you download WAMP, ensure you have downloaded the prerequisite softwares.

Troubleshooting some common errors

1. Wamp Won't Turn Green & VCRUNTIME140.dll error -> http://stackoverflow.com/questions/34215395/wamp-wont-turn-green-vcruntime140-dll-error

2. Wamp Server not goes to green color -> http://stackoverflow.com/questions/17168624/wamp-server-not-goes-to-green-color

3. PHP Warning:  Unknown: POST Content-Length of X bytes exceeds the limit of 8388608 bytes in Unknown on line 0
                 
                 a. Open php.ini file.
                 b. Find post_max_size. Change limit from 8M to 2000M. If problem still occurs, change limit further.
                 
# 2. Google Client ID

Follow instructions given in Step 1 on this page (https://developers.google.com/gmail/api/quickstart/js) to get your google client id. You need to copy that id in backup.php file.

In "Where will you be calling the API from?", choose "Web browser (Javascript)".

# 3. How it works?

1. Download the SaveGMailAsEML folder and save it to www directory of WAMP.
2. Login using your GMail account.
3. After initialization, you will find your GMail labels under Labels.
4. Choose a GMail label and click on Start Back UP.
5. A folder will be created in SaveGMailAsEML folder with name of your GMail label. Subfolders will be created within that folder for pages and emails without attachments.
6. Status message appears on webpage when download is complete.

The downloaded emails are in .eml format. They can be viewed using Windows Live Mail or Windows Mail 10 or any other .eml viewer.

The time limit for receiving data from Google is 30 seconds (which is adjustable). If time exceeds 30 seconds, then the email is saved without attachment.

It is recommended to run the program while keeping the console window open. 

The code has been tested on Chrome Version 54.0.2840.71.

Known errors and solutions:

1. The access token is valid for 1 hour. If the program runs for more than 1 hour, an error will be shown in console window. When this happens refresh and run again. Use the "Continue from page" option and struture your query using label, dates, to, from, subject fields to start where you had left off.

2. Sometimes you may get resource exceeded or quota error. Wheb this happens, refresh and use the guide above to structure your query to start where you had left off.

3. Sometimes you mat get "Aw, Snap" error. Refresh and start again.
