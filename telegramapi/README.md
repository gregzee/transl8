# Telegram for Transl7

### Summary

We will discuss what we needed to do for the Transl8 bot on Telegram. The API on Telegram is super rich, and there are things that we probably missed. So we will just keep it to the purpose of this bot. If there is anything that you think we can improve upon please let us know.


## Botfather

You must always reach out to the Botfather on telegram.

1. Start up telegram, and send a message to botfather https://t.me/botfather
2. You will be greeted with a list of commands.

![image](https://user-images.githubusercontent.com/38545800/156890408-bea8f6c4-d0bd-4f7e-8d94-21bbd62f74db.png)

3. Select new bot and go through the botfathers workflow.
4. Take note of the token the bot gave you <###>:<###>
5. Set your webhook to your Telegram bot
- If you are usine tines.io, your webhook action will provide you all the details.

**From Tines**

![image](https://user-images.githubusercontent.com/38545800/156890918-a503c93d-bc43-41ec-8601-b3359e7d3bbf.png)
![image](https://user-images.githubusercontent.com/38545800/156891691-8cf426ec-8049-46a2-bc91-3d12f8c2216b.png)
![image](https://user-images.githubusercontent.com/38545800/156891716-32997949-54b5-479e-a5f0-d86aafe7f483.png)


*Curl Example:*
```
curl https://api.telegram.org/bot<token>/setWebhook \
    -F "url=webhook" \
```

6. Assuming all went well we can move forward
7. Use botfather for anything else, like building commands or building a profile.

## Next Steps

If you have completed Google Translate API, The detectionlanguage API and now this, we can move forward and use Tines to glue everything together.
