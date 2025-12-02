# Build a Language Translation Bot using Amazon Lex
In this project, we'll be building a language translation bot using Amazon Lex.
If you want to translate a word or sentence into another language, all you have to do is type it into the chatbot - and it will output the translation.

### Video Tutorial
<img width="1920" height="1080" alt="Language  Translation Bot" src="https://github.com/user-attachments/assets/510df793-ac51-4bd2-b699-22bf51f634c0" />
Video Link: 

### In this video, we'll be going through the following steps.

1. Creating an empty chatbot
2. Specifying intents and slots
3. Specify Fulfilment
4. Create an IAM role
5. Create a Lambda function
6. Test the Lambda function
7. Test the chatbot

### Services Used 🛠
* Amazon Lex: Build the chatbot and define conversation flow.
* AWS Lambda: Get the book recommendation using a third party API.
* AWS IAM: Ensures secure access by managing user permissions.
* Amazon Translate: Used for translation of the sentence according to the input language specified.

### Estimated Time & Cost ⚙️
* This project is estimated to take about 1-2 Hours
* Cost: Free (When using the AWS Free Tier)

### Project Architecture:
<img width="1630" height="711" alt="translator_bot_arch" src="https://github.com/user-attachments/assets/af219e6b-0850-4582-b8d1-f4228d608be9" />

### Final Result:
<img width="345" height="681" alt="final_product" src="https://github.com/user-attachments/assets/1322ef79-4978-4aa0-95c1-c6b50c3f816e" />

```sh
Sample Utterances:

I want to translate
Can you help me translate
Translate for me
I want to translate in {language}
Translate in {language}
Can you translate in {language} for me

Language Slot Type:
French
Japanese
Chinese
Spanish
German
Norwegian

Lambda Role:
TranslateFullAccess
AWSLambdaBasicExecutionRole
```

### Lambda Test Event:

```JSON
{
  "sessionState": {
    "intent": {
      "name": "TranslateIntent",
      "slots": {
        "text": {
          "value": {
            "interpretedValue": "Hello",
            "originalValue": "Hello"
          }
        },
        "language": {
          "value": {
            "interpretedValue": "French",
            "originalValue": "French"
          }
        }
      }
    }
  }
}
```

Follow us:
* Join the channel: https://www.youtube.com/channel/UCwhERUcuzUCwr8x8mQ8zrcw/join
* YouTube: https://www.youtube.com/@TechWithYeshwanth/videos
* Follow our GitHub here: https://github.com/yeshwanthlm
* Follow our blog here: https://dev.to/yeshwanthlm/
* Follow us on Instagram: https://www.instagram.com/techwithyeshwanth/
* Follow us on LinkedIn: https://www.linkedin.com/in/yeshwanth-l-m/
