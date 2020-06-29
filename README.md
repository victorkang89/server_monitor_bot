# Server Monitor Bot for Linux based environment

<p align="center">
  <img src="docs/bot-working.gif" height=600 width=300 />
</p>

This is a tool I developed to keep an eye on my server when I might not have access to a PC.

I have the program runing on the server, and it is linked to a bot I have generated by the auth token.. Most commands available in a linux shell can be run through the bot, except for some commands like cd which cannot be run by the subprocess method.
run wit this bot. Just to be safe you can configure the list of commands that can be run from the bot. 

## How to use this?
1. Clone this github repo  
```git clone https://github.com/krishnanunnir/server_monitor_bot && cd server_monitor_bot```

2. Create a virtual environment  
``` mkdir .env && python3 -m venv .env/smb```

3. Activate the virtual environment  
```source .env/smb/bin/activate```

4. Now we need to install all requirements  
```cd bin && python run_once.py```

5. Generate a bot in telegram, add the token value of the bot and the user ids of the users permitted to use this bot in the properties.py file.

6. Configure other values in the properties.py for curr_dir, logs and permitted_commands.

7. We are now good to go and can start our server by running  
```python start.py```

## Future Additions
1. [X] Grabbing screenshots of the users device.
2. [ ] Scheduling messages for an interval
