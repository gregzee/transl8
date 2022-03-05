# Tines 

### Summary

Tines is a low code/no code automation platform. The purpose of this project was to be able to quickly get some form of translation bot out on telegram quick. We noticed that there was news on there that was in Russian or Ukrainian coming in quicker than the 24/7 news cycle. We were able to build this out in Tines relatively faster than we would scripting in python.

You can check out the workflow build in tines [here](transl8bot.json)

Tines uses liquid syntax, please read up on it, and their [documentation](https://hub.tines.com/docs/quickstart).

Import the [story](transl8bot.json) and import into your Tines environment. 

Here is a swimlane of the workflow.
![image](https://user-images.githubusercontent.com/38545800/156892277-a2ec744c-ad01-493c-8e5f-eba7eba9da55.png)




## Add Credentials
1. [Add your google OAUth Credentials](https://github.com/gregzee/transl8/tree/main/translateapi#generating-the-oauth2-creds)
2. [Add your detectionlangue Credentils](https://github.com/gregzee/transl8/blob/main/detectionlanguage/README.md#for-tines)
3. [Add your Bot API Credentils](https://github.com/gregzee/transl8/blob/main/telegramapi/README.md#set-credentials-in-tines)

## Using Credentials
1. ```{{CREDENTIALS.<name>}}```
2. Read up on credentials here,  https://hub.tines.com/docs/credentials
  
