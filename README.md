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


# 3. How it works?

1. Download the SaveGMailAsEML folder and save it to www directory of WAMP.
2. Login using your GMail account.
3. After initialization, you will find your GMail labels under Labels.
4. Choose a GMail label and click on Start Back UP.
5. A folder will be created in SaveGMailAsEML folder with name of your GMail label. Subfolders will be created within that folder for pages and emails without attachments.
6. Status message appears on webpage when download is complete.

The downloaded emails are in .eml format. They can be viewed using Windows Live Mail or Windows Mail 10 or any other .eml viewer.

The code has been tested on Chrome Version 54.0.2840.71.
