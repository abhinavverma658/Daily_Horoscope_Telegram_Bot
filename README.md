# Daily_Horoscope_Telegram_Bot
This project centers on providing daily horoscope readings to users. Essential to this effort is seamlessly integrating an API with platforms like Zapier for automation and UChat for a smooth workflow.
## Tech stack used:
1.	***UChat*** – It is indeed a platform for designing bots, it's likely intended to help users create and manage chatbots for various purposes, such as customer support, information retrieval, or interaction automation. Many businesses and developers use chatbots to streamline communication and interactions with users. 
2.	***Zapier Platform*** – It is a popular automation tool that allows you to connect various web applications and automate workflows without needing to write code. It enables you to create "Zaps," which are automated workflows that trigger actions in one app based on events in another app.
3.	***Divine API*** - Divine API offers developers to integrate the features of Astrology API to their apps and give their users an enthralling experience to peep into the insights of their present, past and future.

## Entire process:
  ### 1.	Making Integration of Divine API with Zapier

1.	***Create a Zap***: To get started, you would have created a new Zap within your Zapier account.
2.	***Trigger Event***: For your trigger, you would have chosen an event that occurs in Divine API. This event could be something like "New Daily Horoscope Available," "Weekly Horoscope Update," or any other relevant event that you want to use as a trigger.
3.	***Connect to Divine API***: Zapier would have prompted you to connect to the Divine API by providing the necessary API key or authentication credentials. This would allow Zapier to access the data from Divine API.
4.	***Configure Trigger Data***: Depending on the chosen trigger event, you might need to configure the data that Zapier should retrieve from Divine API. This could include parameters like zodiac sign, date, or other relevant information.
5.	***Test Trigger***: After configuring the trigger, you would have tested it to ensure that Zapier can successfully retrieve the desired data from Divine API.
6.	***Set Up Action***: Once the trigger is configured and tested, you would proceed to set up an action. This is what Zapier will do when the trigger event occurs.
7.	***Choose Action App***: For the action, you would select an app that you want to connect with Divine API. This app could be an email service, a messaging platform, a spreadsheet tool, or any other app supported by Zapier.
8.	***Configure Action Data***: Depending on the chosen action app, you would configure how the data from Divine API should be used in the action. For example, if you're sending a daily horoscope to an email address, you'd specify the recipient and the content to include in the email.
9.	***Test Action***: After configuring the action, you would test it to ensure that Zapier can successfully perform the desired action using the data from Divine API.
![Screenshot 2023-08-09 112910 -1](https://github.com/abhinavverma658/Daily_Horoscope_Telegram_Bot/assets/73075510/72f5fc3f-4cd5-44aa-830d-6ee6bd2f4447)
Divine API Integration

## 2. Creating Telegram bot and accessing in UChat
 ### Creating a Telegram Bot:

1.	***Create a Telegram Account***: create a Telegram account. This is where your bot will be associated.

2.	***BotFather***: Open the Telegram app and search for the "BotFather" bot. This is the official Telegram bot that helps you create and manage other bots.

3.	***Start the Conversation***: Start a chat with the BotFather and send the /start command to initiate the conversation.

4.	***Create a New Bot***: To create a new bot, send the /newbot command. Follow the prompts to choose a name for your bot and a username that ends with "bot."

5.	***Receive Access Token***: Once your bot is created, the BotFather will provide you with an access token. This access token is essential for interacting with your bot's API.

### Accessing the Telegram Bot in UChat:

1.	***Register on UChat***: If you haven't already, register for an account on the UChat platform where you want to integrate the Telegram bot.
2.	***Access Token Integration***: In UChat, locate the section or settings where you can integrate external services or bots. Look for options related to chatbots or messaging integrations.
3.	***Enter Access Token***: Within the integration settings, you'll likely find a field to enter the Telegram bot access token. Paste the access token you received from the BotFather here.
4.	***Configure Integration***: Depending on the capabilities of the UChat platform, you might have additional settings to configure. This could include specifying which events should trigger interactions with the Telegram bot.
5.	***Testing***: Save the integration settings and test the integration. You might send test messages or perform actions that should trigger the Telegram bot to respond.
6.	***Monitor and Troubleshoot***: Once the integration is set up, monitor its behavior to ensure that messages are being properly sent to and received from the Telegram bot. If you encounter any issues, check your integration settings and access token.
7.	***Implement Use Cases***: Depending on your requirements, you can implement various use cases. 
![Screenshot 2023-08-09 114811-2](https://github.com/abhinavverma658/Daily_Horoscope_Telegram_Bot/assets/73075510/0ff168f2-d8d9-4b03-929d-dab34214597c)
Accessing telegram bot in Uchat

![Screenshot 2023-08-09 115346-3](https://github.com/abhinavverma658/Daily_Horoscope_Telegram_Bot/assets/73075510/cd73ebce-2a20-4793-adb2-85fd8a61c17a)
   Designing workflow and implementing use case
  	
## 3.	Automating horoscope between Divine API and UChat using Zapier
### Creating a Trigger in Zapier with UChat
1. ***Login to Zapier and UChat***:
   - Log in to your Zapier account and UChat account where you want to set up this automation.
2. ***Create a New Zap***:
   - Begin by creating a new Zap in Zapier. A Zap is a workflow that connects two or more apps.
3. ***Choose Trigger App (UChat)***:
   - For the trigger step, search and select UChat as the app to start the workflow.
4. ***Select Trigger Event (Button Press)***:
   - Choose the trigger event that corresponds to a user hitting a button in the Telegram bot within UChat.
5. ***Connect UChat Account***:
   - Connect your UChat account to Zapier. Follow the authentication process to link your UChat account.

### Creating an Action with Divine API
6. ***Choose Action App (Divine API)***:
   - For the action step, search and select Divine API or the relevant app you've integrated for horoscope data.
7. ***Select Action Event (Retrieve Horoscope)***:
   - Choose the action event that corresponds to collecting information about the day's horoscope from Divine API.
8. ***Configure Divine API Action***:
   - Set up the parameters needed to retrieve the horoscope information. This might include the zodiac sign, date, and any other relevant data.
     
### Returning Horoscope Information to UChat:
9. ***Create Another Action with UChat***:
   - Now, create another action step in your Zap to interact with UChat.
10. ***Select Action App (UChat)***:
    - Choose UChat as the app for this action.
11. ***Select Action Event (Send Message)***:
    - Choose the action event that corresponds to sending a message within UChat.
12. ***Configure UChat Message***:
    - In this step, you'll configure the content of the message that you want to send back to the user.
    - Use the horoscope information collected from the Divine API action and insert it into the message.
13. ***Map Data and Send Message***:
    - Map the horoscope information from the previous step into the message you're sending in UChat.
    - This could include using placeholders to dynamically insert the horoscope content.

### Testing and Activating the Zap:
14. ***Test the Zap***:
    - Test your Zap to make sure that all the steps are working correctly.
    - Simulate the trigger event, and see if the information flows seamlessly from the Telegram bot through Divine API to UChat.
15. ***Activate the Zap***:
    - Once you're satisfied with the testing, activate the Zap to make it live and ready to process real user interactions.
16. ***Monitor and Optimize***:
    - Keep an eye on the Zap's performance. Monitor how users are interacting with your Telegram bot and receiving horoscope information in UChat.
    - Adjust any settings or actions as needed to improve the user experience.
      
![Screenshot 2023-08-09 122003 -4](https://github.com/abhinavverma658/Daily_Horoscope_Telegram_Bot/assets/73075510/9479ea83-86e5-4063-b08a-1bfaa06f0a5d)
  Created Trigger Zap in UChat 
  
 ![Screenshot 2023-08-09 122226-5](https://github.com/abhinavverma658/Daily_Horoscope_Telegram_Bot/assets/73075510/6eaf4216-a1ca-42d1-89f0-988448d9bf1f)
Created 1st action of daily horoscope in Divine API

![Screenshot 2023-08-09 122603-6](https://github.com/abhinavverma658/Daily_Horoscope_Telegram_Bot/assets/73075510/48d5c94b-1cc8-4d05-a6ae-8447a8e638bd)
Created 2nd action to send message in Uchat(Telegram bot)

## 4.	Final Result
Get into telegram bot start with message /start, then it will show a message “Hi! Here’s the bot available for you”. There will be a button (Get Daily Horoscope) just down the message. Pressing that button will give horoscope of that day.

![Screenshot 2023-08-09 124053-7](https://github.com/abhinavverma658/Daily_Horoscope_Telegram_Bot/assets/73075510/b149dc58-77f6-4495-8aa3-bbb642b254e1)
Final result screenshot 1

![Screenshot 2023-08-09 124316-8](https://github.com/abhinavverma658/Daily_Horoscope_Telegram_Bot/assets/73075510/9165c9de-a076-4488-a683-20f26bbba645)
Final result screenshot 2

## Challenges I faced:
1.	As, there was no integration of Divine API with Zapier. This was my first challenge I faced.
2.	Understanding of how to make that integration happen.
3.	Understanding of how API works what are its method.
4.	After that my second challenge was to make action in that integration which retrieves information of horoscope of that day.
5.	Third challenge was to create telegram bot and to access in Uchat. 
6.	Now, my fourth challenge was to automate Uchat, and divine API using Zapier.
   
## How I overcame those challenges:

<p>In light of the absence of integration between the Divine API and Zapier, I embarked on a process of seeking guidance from official Zapier documentation regarding the integration of APIs. Additionally, I delved into various tutorials available on platforms like YouTube to glean insights into the intricacies of integrating APIs with Zapier. Through these endeavors, I aimed to gain a comprehensive understanding of the procedures and best practices involved in bridging the gap between the Divine API and the Zapier platform.</p><br>
<p>Subsequently, my next hurdle entailed creating an action within this integration. This action was designed to facilitate the retrieval of daily horoscope information. In order to achieve this, I embarked on a journey to develop a functional process that would seamlessly fetch and present the relevant horoscope data for the given day. This involved crafting a series of steps that would connect the integrated Divine API with the horoscope data source, ensuring the accurate extraction and presentation of the daily horoscope details. Through diligent experimentation and iterative refinement, I aimed to overcome this challenge and successfully enable users to access their daily horoscope information within the integrated framework.
The third significant obstacle I encountered involved the establishment of a Telegram bot and subsequently integrating it into the Uchat platform. This multi-faceted challenge required a series of strategic steps to accomplish.</p><br>
<p>Initially, I ventured into the creation of a Telegram bot by following Telegram's official documentation and guidelines. This involved registering a new bot, obtaining the necessary API credentials, and configuring its functionality to align with the envisioned objectives.
Once the Telegram bot was operational, the subsequent task was to seamlessly integrate it into the Uchat environment. This required a two-fold approach: first, establishing a communication channel between the Telegram bot and Uchat's infrastructure; second, ensuring that the interactions between the bot and Uchat users were smooth and intuitive.</p><br>
<p>To tackle the first aspect, I investigated Uchat's integration capabilities, exploring any available documentation or APIs that could facilitate the connection with the Telegram bot. Once the integration mechanism was deciphered, I proceeded to configure the necessary parameters and establish a reliable link between the two platforms.</p><br>
<p>In addressing the second aspect, I delved into the development of conversational flows that harmonized with Uchat's interface. This entailed scripting interactions, responses, and prompts that would enable users to seamlessly engage with the Telegram bot through the Uchat platform. My aim was to create a cohesive experience that allowed users to interact with the Telegram bot's features within the familiar Uchat environment.</p><br>
<p>By systematically navigating through the intricacies of creating the Telegram bot, integrating it into Uchat, and refining the user experience, I worked towards surmounting this challenge and bringing together the functionalities of both platforms to provide users with a unified and seamless interaction experience.</p><br>
<p>>The fourth challenge involved automating Uchat and the Divine API through Zapier. I explored Zapier's capabilities, defined triggers in Uchat, and created workflows that connected both platforms. These workflows utilized the Divine API to execute tasks based on user interactions in Uchat. Through testing and refinement, I aimed to seamlessly integrate Uchat and the Divine API, enhancing user engagement through streamlined automation.</p><br>

### How system works:

<p>Upon the user's interaction with the Telegram bot by clicking the "Get Daily Horoscope" button, a well-defined sequence of events is set into motion. This orchestrated process revolves around the objective of providing the user with their daily horoscope information.</p><br> 
<p>The initial action triggered by the button click is carefully designed to activate a Zap within the Zapier platform. This Zap, or automated workflow, serves as a bridge between the Telegram bot and the Divine API. Its purpose is to seamlessly initiate subsequent actions that culminate in the delivery of the requested horoscope information.</p><br>
<p>Once the Zap is triggered, it seamlessly transitions to the next step in the process: the action responsible for fetching the daily horoscope information. This action involves a series of interactions with the Divine API, utilizing the POST method. To gather the relevant horoscope data, the action provides necessary arguments such as the date, zodiac sign, API key, and timezone. These parameters facilitate the extraction of accurate and personalized horoscope insights for the given day.</p><br>
<p>Upon successful retrieval of the horoscope information from the Divine API, the workflow proceeds to the final action. This concluding action is tailored to send a message back to the user who initiated the request for their daily horoscope. The retrieved horoscope details are thoughtfully crafted into a user-friendly message format. This message is then dispatched through the Telegram bot to reach the user, providing them with the sought-after horoscope insights for the day.</p><br>
<p>Throughout this intricately designed process, each step is executed with precision and efficiency. The interaction flow from the user's initial button click to the eventual delivery of personalized horoscope information is carefully orchestrated. By integrating the Telegram bot, Zapier, and the Divine API, this system ensures that users receive a seamless and timely experience, with their horoscope needs fulfilled effortlessly within the messaging platform they are comfortable using.</p><br>

[FINAL IMPLEMENTATION](https://drive.google.com/file/d/1nHQy1SNs8dN8uuXP71uFKDgBvisFxT-C/view?usp=sharing)(Video Link)




   





