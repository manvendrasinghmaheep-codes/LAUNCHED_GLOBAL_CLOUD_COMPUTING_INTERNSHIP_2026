# MAJOR PROJECT: RECEPTION—THE RISE OF INTELLIGENT HOSPITALITY

The major project represents the culmination of my cloud computing internship, where I moved beyond automation into the domain of intelligent user interaction. After building a strong foundation with serverless architectures, this project challenged me to design a system that not only processes data but also communicates, understands, and responds like a real-world assistant. It marked my transition from building backend workflows to creating user-centric, interactive cloud solutions.

In the modern hospitality industry, efficiency is no longer defined solely by infrastructure but by the quality of user experience. Customers expect instant responses, seamless booking, and personalized interactions. This project addresses these expectations by introducing an AI-powered hotel booking chatbot capable of handling reservations, guiding users through available options, and delivering a smooth conversational experience. The system is designed to simulate a real hotel receptionist—available 24/7, responsive, and accurate.

Built using AWS LEX, the chatbot leverages natural language understanding to interpret user inputs and respond intelligently. By integrating structured intents, dynamic slots, and a well-defined conversational flow, the bot transforms simple text inputs into meaningful booking actions. Whether a user wants to book a room, check availability, or understand pricing, the system handles it efficiently.

This project was not just about creating a chatbot—it was about understanding how machines can bridge the gap between human intent and system execution. From designing conversational logic to testing real-time interactions, every step contributed to building a system that feels natural and intuitive. It reflects my ability to combine cloud technology with user experience design, creating solutions that are both functional and engaging.

Ultimately, this project stands as a testament to my growth—from learning cloud basics to building intelligent systems. It showcases my readiness to take on real-world challenges and design solutions that align with modern industry standards.

---

# PROBLEM STATEMENT: THE CHAOS OF MANUAL RESERVATIONS

Traditional hotel booking systems often rely on manual processes or static interfaces that lack real-time interaction and personalization. Customers frequently face delays, confusion in room selection, and lack of clarity regarding pricing and availability. These inefficiencies not only impact user experience but also increase operational workload for hotel management. In an era where instant communication is expected, there is a clear need for an intelligent, automated solution that can handle user queries, guide decisions, and streamline the booking process seamlessly.

I have been given a task to -

## Create a Chatbot using Amazon Lex Tool.

### Intent of the chatbot: Book Hotel

* #### 1) All the information must be conveyed to the user after booking the room and
#### must be informed to the user the price of the hotel room and the day of stay.
* #### 2) Using this chatbot user must be aware of the types of Available rooms
#### (Classic, Duplex, etc)-Choose your own Category as well.
* #### 3) All events must be in flow for the fulfillment of the intent.

Keeping the given constraints in mind I started my work on creation of this chatbot.
---

# BOT OVERVIEW: LEX—THE SOUL OF AUTOMATED BOOKING

The hotel booking chatbot developed in this project is an intelligent conversational system designed to automate and simplify the reservation process. Built using AWS LEX, the bot is capable of understanding natural language inputs and guiding users through a structured booking journey.

The system is powered by a well-defined intent model supported by over 20+ diverse utterances, enabling it to handle various user inputs such as booking requests, location-based queries, and date-specific reservations. It utilizes key slots including room type, check-in date, and number of nights to capture essential booking details accurately. These inputs are processed in a structured flow, ensuring that all necessary information is collected before confirming the reservation.

Beyond booking, the bot is designed to provide general information such as available room categories (Classic, Deluxe, Duplex, Suite) and guide users in making informed decisions. The conversational design ensures clarity, engagement, and efficiency, making the interaction feel natural and intuitive. This project demonstrates how conversational AI can transform traditional booking systems into dynamic, user-friendly experiences.

---

## TOOL USED: THE ARSENAL OF CLOUD DOMINANCE

Amazon Lex is a fully managed conversational AI service by AWS that enables developers to build chatbots using voice and text. It provides advanced natural language understanding (NLU) capabilities, allowing the system to interpret user intent and extract relevant data. Lex simplifies the creation of conversational interfaces by managing speech recognition, intent matching, and dialogue flow. In this project, it served as the core platform for designing and deploying the hotel booking chatbot.

---

# INTENT DESIGN: THE BLUEPRINT OF HUMAN DESIRE

Intent design forms the backbone of the chatbot, defining how user inputs are interpreted and processed. In this project, a primary booking intent was created to handle hotel reservations. This intent was carefully structured to capture user goals and guide them through the booking process step by step.

By mapping user queries to a specific intent, the system ensures that each interaction leads toward a meaningful outcome. The intent is supported by multiple utterances and slots, enabling it to handle variations in user language while maintaining accuracy. Proper intent design ensured that the chatbot remained focused, efficient, and capable of delivering consistent responses.

---

# UTTERANCES: THE VOICE OF 23 COMMANDS

Utterances represent the various ways in which users can express their intent. In this project, over 20 carefully crafted utterances were designed to cover a wide range of booking scenarios, including direct requests, location-based queries, and date-specific inputs.

These utterances play a crucial role in making the chatbot flexible and user-friendly. By supporting multiple variations of similar queries, the system can understand natural language inputs more effectively. This ensures that users do not need to follow a strict format while interacting with the bot. Instead, they can communicate naturally, enhancing the overall experience and engagement.

---

# SLOTS: THE PRECISION OF DATA CAPTURE

Slots are used to capture specific pieces of information required to complete a task. In this project, slots such as room type, check-in date, and number of nights were used to gather essential booking details.

These slots ensure that the chatbot collects accurate and structured data, which is necessary for processing reservations. By prompting users for missing information, the system maintains a smooth conversational flow while ensuring completeness and correctness of data.

---

# CONVERSATION FLOW: THE RHYTHM OF SEAMLESS DIALOGUE

The conversation flow of the chatbot is designed to mimic a real hotel receptionist, guiding users step by step through the booking process. The interaction begins with a welcome message, followed by prompts to collect necessary details such as room type, check-in date, and duration of stay.

Each response is carefully structured to maintain clarity and engagement, ensuring that users feel guided rather than instructed. The system also includes confirmation prompts, allowing users to verify their booking before finalizing it. This not only improves accuracy but also enhances user trust.

The flow is dynamic and adaptive, responding to user inputs in real time while maintaining a logical sequence. This ensures that the interaction remains smooth, efficient, and user-friendly, reflecting the standards of modern hospitality systems.

---

# IMPLEMENTATION: DEPLOYMENT OF MY BOT

## CREATE YOUR BOT

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/MAJOR_PROJECT/MAJJOR_SCREENSHOT/LEX%20Dashboard.png" width="800"/>
</p>

<p align="center"><em>Figure 1: AWS LEX Dashboard showing its prices, creation guide and create a bot section from where we will start building out bot.</em></p>

---

#### * FOLLOW THESE STEPS -

* Step 1: Open AWS Lex Console.

* Step 2: Click on create bot.

* Step 3: Out of 3 options given now -

- BASIC BOT
- EXAMPLE BOT
- GEN AI BOT

* Choose basic bot. Our bot is a custom booking bot.

* Step 4: IAM ROLE -

Q. Create a role with basic amazon lex permissions.

* CHOOSE ON CREATE A ROLE.

AWS will automatically provide permissions. We can avoid manual IAM setup like minor project.

---

* Step 5: Bot error logs-

* Select enable.

Might help in error debugging.

* Step 6: COMPILANCE ( COPPA )

* Select: NO .

OUR BOT IS FOR THE PURPOSE OF HOTEL BOOKING NOT FOR CHILDREN .

* Step 7: Session timeout -

* Choose 8-10 minutes.
Users delay booking sometimes.

* Step 8: DISABLE SPEECH TO SPEECH INFERENCE.

WHY -

It helps in avoiding extra configurations and billings.

* Step 9: NOW CREATE YOUR BOT.

---

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/MAJOR_PROJECT/MAJJOR_SCREENSHOT/LEX%20CHATBOT.png" width="800"/>
</p>

<p align="center"><em>Figure 2: AWS LEX Dashboard now looks like this with you bot name, status and other section of the dashboard.</em></p>

---

## INTENT 

#### * FOLLOW THESE STEPS -

Step 1: Intent name -

THIS IS INTERNAL NAME FOR THE SYSTEM.

* Give your bot a suitable name.

* Step 2: Display name -

This is the name which would be shown on the UI.

Give this a meaningful name and proceed to next section.

Step 3: INTENT UTTERANCE GENERATION DESCRIPTION.

* This is the optional AI helper generational field which helps in generating utterances.

* Give this field a necessary and required prompt for which lex later on might suggest some utterances.

* Step 4: Context section:

* LEAVE IT EMPTY.

Our bot has only one intent which is to book hotel. Hence, we don't require multi-conversational context section which helps in creating advanced bots.

##### * NOW WE MOVE ON TO NEXT SECTION.
---
## UTTERANCES 

#### * FIRSTLY, MAKE SURE THAT YOU SLOTS ARE IN THIS ORDER - 

* Room Type -> Check in Date -> Nights of stay.

REASON -

* ##### THIS IS NOT AN ERROR. We just want our bot to behave like real booking bot having natural priority to firstly determine room type and decide the initial costs later then allows customers to select their check in date and nights of stay to stay relevant to real life scenario.

* NOW KEEPING THIS PRIORITY ORDER IN MIND WE PROCEED TO ADD UTTERANCES WHICH ARE TEXT HELPS TO DETERMINE INTENT AND ALLOW BOT TO INTERACT WITH THE USER USING REQUESTS, SEARCHES AND DATA SPECIFIC QUERIES.

* You can create your utterances based on your choice or communication preferences or use my utterances. You can also add some on mine too.

---

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/MAJOR_PROJECT/MAJJOR_SCREENSHOT/LEX%20Utterances%201.png" width="800"/>
</p>

<p align="center"><em>Figure 3: Boooking requests related utterances that triggers out chatbot main intent and the conversation proceeds from here.</em></p>

---

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/MAJOR_PROJECT/MAJJOR_SCREENSHOT/LEX%20Utterances%202.png" width="800"/>
</p>

<p align="center"><em>Figure 4: Check in date and total night stay relevant utterances which deals with date and duration of stay for the user.</em></p>

---

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/MAJOR_PROJECT/MAJJOR_SCREENSHOT/LEX%20Utterances%203.png" width="800"/>
</p>

<p align="center"><em>Figure 5: Room type related utterances which gets more detailed information from the user and now after completing all basic required fields the user can proceed to confirm and book the chosen room. I have chosen in total 23 diverse utterances to handle natural language of the user.</em></p>

---


##### NOW WE MOVE ON TO NEXT SECTION.

---

## SLOTS

* DON'T FORGET LOGICAL PRIORITY ORDER FOR HOTEL BOOKING.

-> Select add slot.

 ##### SLOT 1:

* Step 1: On the left panel, click on Slot types.

* Step 2: Click create slot and this is your room type slot.

* Step 3: Add optional description.

* Step 4: In the values section add the different types of rooms of hotel based on costs.

* Step 5: Click save.

---

* Step 6: Go back to your intent.

* Step 7: Now, in slot section you should see your newly created slot then select it.

* Step 8: Add a relevant prompt.

* Step 9: Select slot required on and save it.

---

 ##### SLOT 2:

* Step 1: Go to slots and choose add a slot.

* Step 2: This is your check in date slot.

* Step 3: In slot type choose amazon.date .

* Step 4: Provide a relevant prompt.

---

 ##### SLOT 3:

* Step 1: Go to slots and choose add a slot.

* Step 2: This is your night stay slot.

* Step 3: In slot type choose amazon.number .

* Step 4: Provide a relevant prompt.

---

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/MAJOR_PROJECT/MAJJOR_SCREENSHOT/LEX%20Slots.png" width="800"/>
</p>

<p align="center"><em>Figure 6: You can check that my chatbot has priority order in descending oder from top as confirming the room first is more relevant than asking stay period or date of check in.</em></p>

---


## CONFIRMATION PROMPT 

THIS IS A NECESSARY FIELD OF OUR PROJECT.

-> THIS IS IN DIRECTION OF OUR INTENT.

* User will be informed that his/her room is booked and now they can proceed further.

* It has two parts confirmation and decline.

* -> As the name suggests, confirmation is used before booking and decline is used if user opts for exit.

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/MAJOR_PROJECT/MAJJOR_SCREENSHOT/LEX%20Confirmation.png" width="800"/>
</p>

<p align="center"><em>Figure 7: This part can make our bot looks highly skilled and trained to deal with both professionalism and user friendly nature.</em></p>

---

* Provide suitable relevant prompt and proceed to next section.

---

## INITIAL RESPONSE

-> THIS IS ALSO RELEVANT FOR OUR PROJECT. 

* -> THIS FIELD GETS TRIGGERED WHEN INTENT IS DISPLAYED BY THE USER IN CONVERSATION.

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/MAJOR_PROJECT/MAJJOR_SCREENSHOT/LEX%20Initial%20Response.png" width="800"/>
</p>

<p align="center"><em>Figure 8: Warm and friendly start to the conversation in the direction of out intent. Provide a knowledgeable start.</em></p>

---

* -> Provide necessary warm and friendly initial input and then proceed to next section.

---

## FULFILLMENT

-> AWS LEX has fallback messages for this section.

It has two parts - confirmation and decline.

##### Similar to confirmation section we proceed by providing necessary inputs to stay close to our real life simulation of hotel booking.

###### Now, we  move on to next section.

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/MAJOR_PROJECT/MAJJOR_SCREENSHOT/LEX%20Fullfillment.png" width="800"/>
</p>

<p align="center"><em>Figure 9: Provide a professional response like a real receptionist.</em></p>


---

## CLOSING RESPONSE

-> After the end of the conversation out bot provides closing response to thank the user who chose it to book room using our lex chat bot.

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/MAJOR_PROJECT/MAJJOR_SCREENSHOT/LEX%20Closing%20Response.png" width="800"/>
</p>

<p align="center"><em>Figure 10: Provide a inviting and courteous ending message to the user.</em></p>

---

### -> Provide a nice ending to the conversation with the user.

---

# TESTING: THE TRIAL OF LOGIC

The chatbot was thoroughly tested using multiple scenarios to ensure accuracy, reliability, and smooth interaction. Different user inputs were provided to evaluate how well the system handles variations in language and incomplete information.

Testing also involved verifying slot extraction, intent recognition, and confirmation flows. By analyzing responses and refining configurations, the chatbot was optimized to deliver consistent and accurate results. This phase ensured that the system performs effectively under real-world conditions.

---

## CONVERSATION MODEL -

* Utterances -> Intent detection

* Intent -> Slots Collection

* Slots -> Confirmation

* Confirmation -> Fullfillment

* Fullfillment -> Closing response

---

#### PAY ATTENTION TO RIGHT SIDE OF THE IMAGES -

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/MAJOR_PROJECT/MAJJOR_SCREENSHOT/CHATBOT%20TEST1.png" width="800"/>
</p>

<p align="center"><em>Figure 11: The user initiated the conversation by showing the intent that he wants to book a hotel room. After which our bot started slots collection starting from room type.</em></p>

---

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/MAJOR_PROJECT/MAJJOR_SCREENSHOT/CHATBOT%20TEST2.png" width="800"/>
</p>

<p align="center"><em>Figure 12: After that our bot proceeds to enquire about check in date and total nights of stay.</em></p>

---

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/MAJOR_PROJECT/MAJJOR_SCREENSHOT/CHATBOT%20TEST3.png" width="800"/>
</p>

<p align="center"><em>Figure 13: Now after collecting all the required data the bot moves towards the last stage of confirmation..</em></p>

---

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/MAJOR_PROJECT/MAJJOR_SCREENSHOT/CHATBOT%20TEST4.png" width="800"/>
</p>

<p align="center"><em>Figure 14: To which the user given consent and thus our bot provided fullfillment and nice closing response.</em></p>

---

### CONVERSATION FINAL WORK FLOW

* User → Book a room

* Bot → Welcome message

* Bot → What type of room would you like?

* User → Classic

* Bot → What day would you like to check in?

* User → 25 March

* Bot → How many nights will you stay?

* User → 2

* Bot → Please confirm your booking

* User → Yes

* Bot → Booking confirmed
* Bot → Closing response

---

# CONCLUSION: THE LEGACY OF A CLOUD ARCHITECT

The completion of this major project marks a defining moment in my cloud computing journey. It represents not just the development of a chatbot, but the evolution of my understanding of how intelligent systems are designed, built, and refined. From handling simple cloud resources to creating an interactive, user-focused application, this project reflects my growth as a developer and problem solver.

Throughout this journey, I encountered multiple challenges—from designing conversation flows to handling logical errors and refining user interactions. However, each challenge strengthened my ability to think critically, adapt quickly, and persist through difficulties. I learned that building real-world systems requires more than technical knowledge—it demands patience, creativity, and a deep understanding of user needs.

This project has instilled in me a strong sense of confidence and direction. It has proven that I can take an idea, design its architecture, implement it using cloud technologies, and deliver a functional solution. More importantly, it has reinforced my commitment to continuous learning and improvement.

As I move forward, I carry with me not only the skills gained but also the mindset developed through this experience. I am driven by passion, disciplined in execution, and committed to achieving excellence in the field of cloud computing. This project is not the end of my journey—it is the beginning of a path where I aim to build scalable, intelligent, and impactful cloud solutions.

The legacy of this project lies not just in its implementation, but in the determination behind it—a determination that will continue to drive me toward becoming a skilled cloud architect.

---


