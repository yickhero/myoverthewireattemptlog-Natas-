# myoverthewireattemptlog-Natas-
This is my attempt log on over the wire Natas levels

Level 0:
- I saw a mostly blank webpage in it and I assume the password is in the source
- I went to the source and look at different files and found the password
- password: scfWG6qNEIdzqVyfRwEGXyNUfFZkZeQ7

Level 0 --> Level 1:
- So right clicking has been blocked, but i usually press F12 to go to inspector
- Therefore it didn't affect me, and I found the password in the source files
- password: vsDOxoXyq3wckCP1ZmTZ71ngIA606odB

Level 1 --> Level 2:
- So I found nothing in the HTML file
- but I found a path which wasn't there in the last level, which was the files/pixel.png
- I thought the png file was the password but it wasn't
- so I added a /files after the URL and there was a file there that contains the password
- password: K30JrSRHzjxq3paUQuwozY4MNvmNFyhI

Level 2 --> Level 3:
- So there is nothing in the inspector but one comment "!-- No more information leaks!! Not even Google will find it this time... -->"
- So I assumed is something with bots and crawls
- so I searched up what file is for bots and crawls in websites and i found robots.txt
- which i put it behind the URL and it led me to the password
- password: JDrPnuZAKyl6MkiqQGFIddrqpvgOASth

Level 3 --> Level 4:
- So I found out that I have to pretend that I am coming from natas5 to get the password
- Therefore I need to change the header that was sent to the server
- I downloaded burpsuite and use the browser to intercept the request
- then use the repeater to repeate the request and change the line from 
Referer: http://natas4.natas.labs.overthewire.org/ --> Referer: http://natas5.natas.labs.overthewire.org/
- It gave me the password afterwards
- password: e4z2Noy3oqwPJUWzJH0dseN67Cn1sy2M

Level 4 --> Level 5:
- So I used burp suite to intercept again
- I used the repeater to changed the loggedin variable from 0 to 1
- and i got the password
- password: 7mhjtShJAcld2NYbKHEadnhEwRn2P8VT

Level 5 --> Level 6:
- So there is a textbox where you need to put in the secret
- I looked at the source code and the password is in includes/secret.inc
- so I put that in the URL and got the secret
- password: B1szg95UcTnrzwnF3i3TzYHlyYh8iBV0