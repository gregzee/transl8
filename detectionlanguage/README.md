# detectlanguage.com

## Getting Started

I used this over the Google translate engine. I am not familiar with how the billing/quota works, and from my quick research, it seems that the Google Translate & Detection character limit seems to both count towards the character count. If that is the case, I wanted to split this and find another API.

We are using https://detectlanguage.com/ for Transl8, and after various tests it seemed great, very user friendly. 

1. Sign up
2. Generate an API Key
3. Documentation on the website is really straight forward when trying to detect a language
4. https://detectlanguage.com/documentation#single-detection

## For Tines

1. Copy API Key
2. Go to Credentials & Create New
3. Use "TEXT" credential
4. Store & Save

*Example:*

![image](https://user-images.githubusercontent.com/38545800/156892893-21a4465a-5c1a-4695-9fed-3e7e89c8e64d.png)



## How is it used?

Transl8 is only looking for Ukrainian and or Russian. We detectlanguage.com to determine that mostly, and if there is anything else but those languages, we kindly let the user know that other languages are not supported. This whole project is for what is happening in Ukraine today.



