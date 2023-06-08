# AWS-Personalised-Chatbot
Amazon Lex is a service provided by Amazon Web Services (AWS) that enables the building of conversational interfaces, also known as chatbots or virtual assistants. It utilizes natural language understanding (NLU) to process and interpret user input, allowing the chatbots to understand and respond to user queries and commands.

Amazon Lex offers a set of tools and capabilities for creating highly interactive and intelligent chatbot applications. It leverages automatic speech recognition (ASR) for converting speech into text, and it can integrate with voice and text-based channels such as messaging platforms, mobile apps, and IoT devices

1. create an AWS account

2. Open Amazon Lex
 
3. create Intent

When designing a chatbot using Amazon Lex, intents are defined and configured to handle different types of user requests or actions. Each intent is associated with a set of sample utterances or phrases that users might use to express that particular intention.

![Image](https://user-images.githubusercontent.com/111515881/244296224-f6f0e94b-264f-4e65-b70e-4f64eaf76db4.png)


Intents help structure the conversation flow and enable the chatbot to understand and respond effectively to user queries or requests. They form a key component in building conversational interfaces and enable chatbots to provide meaningful and context-aware interactions.

There are 2 types of intents. choose 
- blank/empty intent for the creation of a new solution.

- built-in intents = designed to handle specific functionalities and can be used as a starting point for building your chatbot.


•	AMAZON.CancelIntent: Handles the user's request to cancel an ongoing operation or conversation.

•	AMAZON.HelpIntent: Handles the user's request for assistance or help.

•	AMAZON.StopIntent: Handles the user's request to stop or end the conversation.

•	AMAZON.NavigateHomeIntent: Handles the user's request to navigate to the home or main screen.

•	AMAZON.YesIntent: Handles the user's affirmative response.

•	AMAZON.NoIntent: Handles the user's negative response.

•	AMAZON.RepeatIntent: Handles the user's request to repeat the last response.

•	AMAZON.StartOverIntent: Handles the user's request to start the conversation over.

Slot types define the format, constraints, and possible values for a particular slot. Amazon Lex provides several built-in slot types, and you can also create custom slot types based on your specific requirements.
Here are some commonly used built-in slot types in Amazon Lex:

AMAZON.DATE: Used to extract dates or date ranges from user input.
Example: "Book a hotel on July 10th."

AMAZON.NUMBER: Used for extracting numerical values from user input.
Example: "I want to order 3 pizzas."

AMAZON.TIME: Used to extract time values or durations from user input.
Example: "Set an alarm for 7 AM."

AMAZON.US_CITY: Used for extracting U.S. city names from user input.
Example: "Find restaurants in Seattle."

AMAZON.EmailAddress: Used to extract email addresses from user input.
Example: "My email is john@example.com."

AMAZON.PhoneNumber: Used for extracting phone numbers from user input.
Example: "Contact me at 123-456-7890."

Give name and details about the INTENT.
![Image](https://user-images.githubusercontent.com/111515881/244300785-1d0a5c97-6c7a-4e4d-8a8f-65663e94c507.png)

SAMPLE UTTERANCES

Sample utterances are example phrases or sentences that users might say or type to interact with a chatbot. They help train the natural language understanding (NLU) capabilities of the chatbot by providing variations of how users can express their intentions or requests.

When defining intents in Amazon Lex, you associate them with a set of sample utterances. These utterances represent different ways users may express the same intent. By providing a diverse range of sample utterances, you increase the likelihood that the chatbot will accurately recognize and match user input to the correct intent.

Here are some examples of sample utterances for a hypothetical "Booking a hotel" intent:
![Image](https://user-images.githubusercontent.com/111515881/244311085-ddf2e73f-c5aa-4ba4-a71e-76d60c423bed.png)

SLOTS:
Slots allow the chatbot to gather and store user-provided values that are necessary for processing their request. When defining intents in Amazon Lex, you can specify the slots required for each intent and configure them with specific slot types, prompts, and validation rules.


![Image](https://user-images.githubusercontent.com/111515881/244311219-c063c1f6-8011-452b-bb68-619e53c5f585.png)




Each slot will appear like this:


![Image](https://user-images.githubusercontent.com/111515881/244311328-01774016-7e23-46f0-aa85-cd810c680d53.png)


In ADVANCED OPTIONS ….we can add the SUCCESS response and the FAILURE response for the user as a reply.
Additionally, we can add CONDITIONAL BRANCHING to validate the input as a IF-ELSE CONDITION.

CONFIRMATION

In the context of chatbot development, confirmation refers to the step in the conversation where the chatbot asks the user to verify or confirm a certain piece of information or an action before proceeding further. It helps ensure that the chatbot has understood the user's intent correctly and allows the user to review and validate the details before finalizing an action.



![Image](https://user-images.githubusercontent.com/111515881/244311430-80737d34-7fdf-4d74-94af-e14a8f1b4bb3.png)



FULFILLMENT

Fulfillment, in the context of chatbot development, refers to the process of carrying out the desired action or providing the appropriate response based on the user's request. It involves taking the information collected from the user, processing it, and generating a meaningful output or completing a specific task.
In Amazon Lex, fulfillment is typically implemented through integration with other services or systems, such as APIs, databases, or business logic. Once the user's intent and slot values are captured, the chatbot can use this information to fulfill the user's request.
Amazon Lex provides various mechanisms for implementing fulfillment logic, such as AWS Lambda functions. By integrating with Lambda or other services, you can write custom code to handle the business logic and interact with external systems as needed.
The fulfillment stage plays a crucial role in delivering a valuable and meaningful user experience. It enables the chatbot to take action on user requests, retrieve information from relevant sources, or execute specific operations to meet the user's needs effectively.



![Image](https://user-images.githubusercontent.com/111515881/244311532-86e113e5-f3e5-4119-ac87-0f0665a02f7d.png)



CLOSING RESPONSE


![Image](https://user-images.githubusercontent.com/111515881/244311597-3f4d0893-c71b-4e54-bebd-882d2cd4a023.png)



RESULTS:


![Image](https://user-images.githubusercontent.com/111515881/244312439-af53001b-c63e-4532-aff0-5524e6e1ed17.png)




![Image](https://user-images.githubusercontent.com/111515881/244312534-f98c3cb6-d1d1-4c07-81e8-61c556cf2d97.png)




![Image](https://user-images.githubusercontent.com/111515881/244312604-5aa146a4-e7e0-4ee9-b036-321169bd9236.png)




![Image](https://user-images.githubusercontent.com/111515881/244312665-4f0777ec-d8f1-4f8c-9826-cc5b803b13b6.png)




![Image](https://user-images.githubusercontent.com/111515881/244312735-a61282c4-29da-47c7-935b-87538a156c12.png)




![Image](https://user-images.githubusercontent.com/111515881/244312804-45921d5a-9806-4885-8814-54c079dde84f.png)




![Image](https://user-images.githubusercontent.com/111515881/244312884-73f1da7b-2ae1-4a3e-81c9-dea8e7af69d8.png)


