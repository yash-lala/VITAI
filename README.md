# VITAI
The perfect nutritionist + Personal assistant
See code ![here]([url](https://www.icloud.com/shortcuts/fccfedfb2e444df2bf48581ae321cfd8))

VITAI has been designed intentionally to exist in the background without a traditioanl UI element.
It seemlessly does it work in the background without interrupting your workflow and nudges you to live a healthy lifestyle by tailored meals, meditaions and workout plans.

Inspiration 
US obesity rates have tripled over the last 60 years, As of 2023, 43% of Americans are obese -this number is up 13% from the year 2000. 1 in 6 adults, or,  approximately 50 million people in the US are experiencing mental health issues and 55% of them do not receive any mental health treatment. ( Source: mhanational). 
These stats were appalling, and,  understandably, are going to increase exponentially. 
Several studies have found that Depression and Anxiety can both be associated with overeating, poor food choices, a more sedentary lifestyle and very little physical activity. 
Recognizing that health & wellness is a 1.2 trillion TAM in the US alone, a question arose, why are obesity rates and mental health issues at an all time high? 
Lack of awareness, lack of resources, lack of access, lack of understanding of what a healthy lifestyle could look like, lack of instructions on how to change a lifestyle into a healthier one was a significant contributor! 


What it does 
The app guides the user to a healthier lifestyle by providing personalized meal and workout plans synced directly to the users daily schedule
	The key features include:
Food Purchase Tracking: Grocery and restaurant transactions are synced to the app and the nutrition profile of the food item gets stored. 
Integration With Health App: Using the health app on ios, users’ comprehensive health profile indicating health objectives get extracted and is considered as an input to be fed into our proprietary AI Algorithm.
Health Assistant: The algorithm takes nutritional content and health objectives of the user’s as the input and suggests personalized workout routines, with exercise types, frequency, and intensity tailored to each user's body, fitness level, and goals. The algorithm also analyzes food logs, and generates meal plans along with an ingredient list and macronutrient insights.
Consolidated View: The workout routine and consolidated advice for the users are stored on the Notes app on the device
Integrated Calendar and Reminders: Diet and workout plans are automatically synced to the users’ calendar and reminder app on their devices. 


The end result is a holistic healthy living assistant that learns user habits and preferences to deliver the perfect customized plan to help them reach their wellness goals. The app simplifies nutrition and fitness so users can live their healthiest lives. 


How we built it - We leveraged OpenAI's API and Apple's Shortcuts ecosystem to create a seamless workflow that works on "fuzzy json" principles - truly making our app dynamic and personalized to each user. The prompts fed to gpt4, give it the freedom to choose the type of events that should be recommended, it does this by simply reading the users note on what they like - if there are any accommodations that we should be aware of - it then generates a json which we consume through the API creating its suggestions into calendar events that the user can effortlessly follow. All of the user's data stays with them. Health has never been so accessible and so secure. 


Challenges we ran into 
Our Challenges were two fold 1. Technological , 2. Identifying the right business model 
We faced  problems initially in interfacing our GPT-4 model with a device, in this case an iphone. We tried setting up an intermediate google cloud function store to act as a data intermediary between the streamlit app and our backend running on Google Collab’s servers. The implementation proved to be clunky with fairly high latency. 
In full hackathon spirit,as a team consisting of 4 aspiring product managers and no developer, we decided to pivot and use the more intuitive Shortcuts app that comes installed by default on iOS and MacOS. 
A component of our project involves reading a user’s restaurant order via tap at checkout, when users pay using Apple Pay. Emulating a NFC tag proved to be more difficult than we anticipated. We decided to settle on using an android phone as a makeshift NFC tag.Programming the android powered NFC tag to work on the standard that the iphone’s background NFC reader worked with was time consuming. Our scramble to find an Android device was dramatic enough to make a two seasons long Netflix series. Apple’s dominance here has never been more visible.
On the business side of things - converging on a pricing model was challenging. We ran financial projects for various monetization strategies such as subscription models, pay as you go pricing, one-time fees, etc. 
With our application having several tangential applications, deciding to prioritize one use case over the other required a lot of market research, collective brainstorming, and at the end of the day - some hopefully correct intuitive gut decisions


Accomplishments that we're proud of 
Identifying a problem, ideating a solution, performing market and financial analysis,building a pitch deck, a sample MVP - all in a day and a half, a feat we didn’t know we’re capable of! 
Taking a step back and looking at the bigger picture everytime we ran into technical difficulties, to figure out a simpler solution
Keeping the UX smooth, seamless- keeping in mind the customers gain throughout 
Presenting a solution we’d be want to working towards beyond one  weekend

What we learned
This project opened our eyes to the endless opportunities that interfacing with OpenAI’s APIs provide. We learned a lot about nuances of prompt engineering, marveled at the performance differences between GPT3.5 and GPT-4, got lost in discussion about just how beyond our imaginations a potential GPT-5 would be and everything else in between. 
We were exposed to  the inner workings of several multi-billion dollar industries like Wellness, Healthcare and Nutrition. We researched a great deal about “consumer willingness to pay” and debated on what it took to make a “sticky” application. The collective process of building a working prototype, brainstorming GTM strategies, creating financial projects and tying up several loose ends in between provided far more learning than any crash course or youtube tutorial could provide.
While we did have our differences in thought, as every competent team does, we collectively fantasized over the enormous opportunity generative AI posed for our futures, and the world! Marc Andreessen was indeed right. Software is eating the world!

What's next for VITAI - We will exapnd it capabilites to "seeing" and "sensing" with camera and 3rd party app integrations where it can do what in does best - in a multimodal form. 

Built With
ChatGPT, Shortcuts (Health, Calendar, Notes) 
 

