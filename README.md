# SendLine
Sending message to chat application LINE 

Dowmload Line sticker from  http://cons-robotics.com/LINEAPI/sticker.pdf

Copy token from https://notify-bot.line.me/my/
Please note: Line account is compulsory to run this program

1. Access to the above link with your account
2. Press generate token
3. On the window you need to name your chat bot 
4. Choose the group or chat box that you like to send message
5. Add Line Notify into the group or chat box 


Open CMD
You may heck Python version before used with pip -V
1. Go to https://pypi.org/project/songline/
2. Install: pip install songline


from songline import Sendline

token = 'FM9m4KGs9rsVRzpTEZCGwdbQn5WcBOGE6CDElqSV3fF' #get from Line notify token

messenger = Sendline(token)

messenger.sendtext('Hi, how are you?') #send text
messenger.sticker(8,1) #send sticker
messenger.sendimage('https://post.greatist.com/wp-content/uploads/sites/3/2020/02/322868_1100-1100x628.jpg') #send picture

Please note: fine stickers code from https://notify-bot.line.me/doc/en/ or  http://cons-robotics.com/LINEAPI/sticker.pdf

Credit from Uncle Engineer

