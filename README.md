# Python_Voice_Chatbot [![Maintenance](https://img.shields.io/badge/Maintained%3F-no-red.svg)](https://bitbucket.org/lbesson/ansi-colors) [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/) [![GitHub license](https://img.shields.io/github/license/wsdt/Python_Voice_Chatbot.svg)](https://github.com/wsdt/Python_Voice_Chatbot/blob/master/LICENSE) [![Generic badge](https://img.shields.io/badge/Docker-Compatible-blue.svg)](https://www.docker.com/) [![Donate](https://img.shields.io/badge/Donate-Pay%20me%20a%20coffee-3cf)](https://github.com/wsdt/Global/wiki/Donation) [![saythanks](https://img.shields.io/badge/say-thanks-ff69b4.svg)](https://saythanks.io/to/kevin.riedl.privat%40gmail.com)

Easy to use *modular* chatbot to talk to, get information from etc. (depends on enabled modules) and the best of all **keeping your data private/locally**. Therefore, the assistant can operate offline except by the use of some modules (e.g. weather module, etc.). Would love to see some reactions (issues, pull-requests, etc.). Please note, that this project is young and has not all featured functionalities.
This application uses the Chatterbot framework.  

## How to get started
To get your home assistant running you just have to take 1-2 steps (depends on whether you started the assistant before).
1. Execute *setup.py* once, if you newly downloaded this assistant
1. Execute *main.py*

Above steps will work assuming that you have all python libraries installed. Considering this I recommend using Docker, for that I have provided a [Dockerfile](https://github.com/wsdt/Python_Voice_Chatbot/blob/master/Dockerfile).

### Docker-Ready
To start the bot without any complications I made a [Dockerfile](https://github.com/wsdt/Python_Voice_Chatbot/blob/master/Dockerfile) for you guys. You will find this project also on [Dockerhub (hub.docker.com/r/wsdt/python_voice_chatbot)](https://hub.docker.com/r/wsdt/python_voice_chatbot). Therefore you have two options to build the docker image: 
1. Build docker image
   - Build the dockerfile yourself/locally. 
     ``` docker build -t wsdt/python_voice_chatbot . ```
       **OR**
   - You can also download the pre-compiled image from Dockerhub. Just pull the existing docker image (gets built every time a   contributor pushes on Github).
     ``` docker pull wsdt/python_voice_chatbot ```
1. Start a new container out of the newly created/built image: 
``` docker run wsdt/python_voice_chatbot ```
1. Verify that the container is running by: 
``` docker ps -a ```

For more detailed information I recommend you to look through the [Docker-documentation](https://docs.docker.com/). 

## Contribution [![Open Source Love svg2](https://badges.frapsoft.com/os/v2/open-source.svg?v=103)](https://github.com/ellerbrock/open-source-badges/) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)

This project is licensed under GNU V3, so contributions/pull-requests are welcome. All contributors get listed here.  

**Contributors** 
- Kevin Riedl ([WSDT](https://github.com/wsdt))

### How to contribute
To create new modules or changing/extending the application core, please take a look into following files, which are well commented (Better documentation follows):
1. ./starterkit/abstr_answer.py --> How to create a new module
1. ./setup.py --> How to install this assistant

Project not maintained due to other projects, which tried to do the same. 

### How to add an issue
1. **Add a good title to your issue.** Please use a concise and precise title. 
  * *BAD*: "ServiceMgr"
  * *GOOD*: "Redesign/Improve ServiceMgr"
2. **Add a good description to your issue.** Your description doesn't need to be concise, but should be clear/understandable and provide enough information for other contributors to solve the issue. For that I provided an issue template. 

## Python_Chatbot
You might have seen that I published also a quite similar repository called Python_Telegram_Chatbot [https://github.com/wsdt/Python_Telegram_Chatbot]. The Python_Chatbot repository is only a simple chatbot for your Telegram app, which can conversate with you and has some additional features like some information about your Instagram account, random quotes/pics/questions etc. 

In contrast to that **this** repository provides are more modular interface and does not communicate via Telegram, but via voice with you. 
