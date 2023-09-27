# Robot Creative Workshop

The Robot Creative Workshop is a very interesting DIY feature open to all MyShell users. You can combine interesting bots in several ways, and we strongly encourage everyone to create their own lively and interesting entertainment bots and enjoy the experience!

You can create your own robot in just five minutes!

1. Use definitions to specify the robot's personality and mission;
2. The amazing fast voice cloning gives the robot a pleasant voice;
3. The external knowledge base makes the robot have incredibly powerful professional knowledge;
4. And the upcoming Internet and API access capabilities, multimodal models will bring deeper and more powerful capabilities to the robot.

## Definition

The robot definition is the most critical parameter setting (Prompt) for the robot. It allows you to define the robot's role, function, and even conversation style. MyShell supports everyone to generate a complete and comprehensive Prompt for the robot through the simplest role definition method.

### Auto-Prompt (strongly recommended)

Auto-Prompt is an innovative Prompt generation tool launched by MyShell. You can have a knowledgeable, character, and speaking style similar to the defined role by simply defining the bot's simple identity. There are currently two main ways to define:

_**Through role definition**_

For some well-known character roles, you can directly enter the character name, and then MyShell will automatically supplement the character's background knowledge, personality traits, and conversation style, and display the complete Prompt as the robot's parameter setting.

Some specific examples and dialogue effects are as follows:

**Input**: "Rick Sanchez"

**Dialogue effect**: Realistically imitate Rick Sanchez's "arrogant" and "sarcastic" speaking style and have his background story (as shown in the figure below)

<figure><img src="../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

**Input**: "SpongeBob SquarePants"

**Dialogue effect**: Realistically imitate SpongeBob SquarePants' innocent and cute speaking style and incorporate SpongeBob SquarePants' character experience (as shown in the figure below)

<figure><img src="../../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

Please note that network access may be required during the expansion of the Prompt. For characters after 2021, the waiting time may be longer. If you encounter a failure, please try again in two minutes or ask directly in our official [Discord](https://discord.com/invite/XQ7Tx8qEwg) community!

_**Through description definition**_

You can also complete a richer characterization of the robot through more specific descriptions. MyShell will further expand it through a large number of excellent Prompt practices and a huge knowledge base. You can easily deploy a learning, entertainment, or tool robot that perfectly reflects your ideas.

Some specific scenarios and effects are as follows:

**Scenario**: Create an exclusive robot with specific skills

**Input**: "Kira, an experienced English teacher who can help me improve my English"

**Dialogue effect**: As an exclusive English teacher, Kira will actively inquire about her situation and arrange follow-up learning plans.

<figure><img src="../../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

**Scenario**: Role-playing game

**Input:** "RPG Game, act as an astronaut landing on an unknown planet."

**Response:** The bot has already imagined an exciting RPG game plot with just one sentence, leading players on an adventure!

<figure><img src="../../.gitbook/assets/image (1) (1).png" alt=""><figcaption></figcaption></figure>

**Scene:** Tool Bot

**Input:** "A top Twitter influencer who can help others with tweets writeups"

**Response:** The bot will help generate more attractive copy based on the topic provided by the user!

<figure><img src="../../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

The above lists some common use cases. Feel free to explore more possibilities and create your own custom bot! Additionally, a good bot is born through continuous debugging. When you define a bot through automated prompts, its complete prompt will be displayed for further modification. If the desired effect is not achieved after debugging, come and learn advanced knowledge.

### Prompt (Advanced)

For users with more complex needs, we also provide a more detailed usage of prompts and some application techniques, including rich examples. First, please understand the advanced concepts of prompts:

* The essence of a prompt is to trigger an AI language model to play a fill-in-the-blank game with you. The system prompt provides initial instructions to the model, defining its role, personality, instructions to follow, and background information when interacting with you.
* Place clear instructions (such as requiring the language model to play a certain role) at the beginning of the prompt, be as specific as possible, and leave as little room as possible for the model to operate, limiting its operational space.
* Use descriptive language and examples to help the language model better understand your requirements. The method of examples is to add input-output pairs, which simulate a conversation between you and the AI, allowing it to mimic this behavior pattern in the following conversation.
* If necessary, you can specify the output structure, including the content to be included and the text format of the output.
* Use separators, headings, capitalization, and markdown between different modules in a prompt to enhance the structure's clarity and readability.
* Make good use of emphasis, especially adding some emphatic statements at the end of the prompt (the language model has recent bias), such as emphasizing again that "you are not an AI language model" and "keep your answer within 50 words" and other powerful requirements.
* If the model cannot complete the assigned task, sometimes providing an alternative path may be helpful. For example, when asking a question about a piece of text, you can add something like "if the answer does not exist, reply with 'not found'." This helps avoid the model generating an incorrect response.

The following will introduce some methods of use, but it does not mean that it is exhaustive, but provides some methods for you to think creatively and try.

1. _**Applications in non-chat scenarios**_

For example, in some classification scenarios, specific rules can be set for the bot, such as:

> **System Prompt:** You are an assistant tasked with analyzing emotions in speech data. The user will paste a piece of text, and you will evaluate the speaker's response. Give a rating of 1-10 (10 being the highest). Explain the reason for the rating.
>
> **User:** Hi, thank you for calling Contoso Pharmacy. Who am I speaking with today? I understand your frustration, Mary. Can you tell me what goal you're trying to achieve? Okay, great, let me take a look for you. I see here that you used regular Liptor, is that correct? Okay, so I see that your doctor stopped prescribing these drugs in 2021. Is that actually the case? Okay, let me check for you. Because sometimes there are gaps in the system that are not reported. Please wait a moment while I see if there are any records here. So according to the latest records provided to us by the doctor's office, your doctor prescribed these drugs from 2012 to 2021. Okay, in the latest records, it shows that the doctor has now switched to a different type of drug - Metformin. Do you need help preparing and dispensing a 500mg Metformin prescription? You're welcome, Mary. Is there anything else I can help you with today?
>
> **Assistant:** Emotion rating: 8
>
> The speaker in this text seems polite, helpful, and patient when addressing customer concerns. They take the time to check information, provide clear explanations, and offer assistance. However, the rating is not 10 because there are still hints of uncertainty in some parts of the conversation, which may not convey complete confidence to the customer.

2. _**Example of Dialogue Learning**_

Provide additional context and dialogue examples for the model to respond in a specific way, imitate specific behaviors, and provide seed answers for common questions. For example,

> **System Prompt:** The assistant is an intelligent chatbot designed to help users answer their tax-related questions.
>
> Instructions:
>
> * Only answer questions related to taxes.
> * If you are unsure of the answer, you can say "I don't know" or "I'm not sure" and suggest that the user visit the IRS website for more information.
>
> Examples:
>
> **User:** "What is the deadline for filing my taxes?"
>
> **Assistant:** "In 2023, you need to file your taxes by April 18th. This date is after the usual deadline of April 15th because April 15th is a Saturday in 2023. For more information, please see [https://www.irs.gov/filing/individuals/when-to-file](https://www.irs.gov/filing/individuals/when-to-file)."
>
> **User:** "How can I check the status of my tax refund?"
>
> **Assistant:** "You can check the status of your tax refund by visiting [https://www.irs.gov/refunds](https://www.irs.gov/refunds)."
>
> **User:** "When do I need to file my taxes by?"
>
> **Assistant:** "The deadline for filing taxes depends on your filing status and the state regulations in your area. For most people, the federal income tax filing deadline is usually April 15th each year. However, if April 15th falls on a weekend or holiday, the deadline may be pushed back to a later date. Additionally, the filing deadline for each state may be different, and you will need to check the specific regulations for the state you are in. For more information, please see [https://www.irs.gov/filing/individuals/when-to-file](https://www.irs.gov/filing/individuals/when-to-file)."

3. _**Specifying Output Structure**_

Using prompts to specify output structure can greatly help the quality of generated structures. For example,

> **System Prompt:** You are an AI assistant tasked with listing the different behaviors exhibited by customer support representatives in various conversations. Use the format "Behavior ("Reason")" to categorize and list the various behaviors, and cite the reasons behind the categorization.
>
> **User:** Hi, thank you for calling Contoso Pharmacy, who am I speaking with today? I understand your frustration, Mary. Can you tell me what goal you're trying to achieve? Okay, great, let me take a look for you. I see here that you used to take regular Liptor, is that correct? Okay, so I see that your doctor stopped prescribing those in 2021. Is that actually the case? Okay, let me check for you. Sometimes there are glitches in the system that aren't reported. Just give me a moment to see if there's a record here. So according to the latest records provided to us by the doctor's office, it shows that your doctor did prescribe those drugs to you between 2012 and 2021. Okay, the latest records show that your doctor has now switched you to a different type of drug - Metformin. Would you like us to help prepare and issue a prescription for 500mg Metformin for you? You're welcome, Mary. Is there anything else we can help you with today?
>
> **Assistant:** Here are the different behaviors exhibited by customer support representatives in various conversations:
>
> 1. Politeness and friendliness ("Building rapport"): Customer support representatives greet customers and communicate with them in a friendly tone at the beginning of the conversation, which helps to build a relationship with the customer and increase customer satisfaction.
> 2. Inquiring about customer needs ("Understanding customer needs"): Customer support representatives ask customers about their questions and needs in order to provide help and solutions.
> 3. Confirming customer information ("Verifying information"): Customer support representatives verify customers' personal and order information to ensure that they can provide the correct help and solutions.
> 4. Checking system records ("Finding information"): Customer support representatives search system records to obtain information and history about customers and determine the best solution.
> 5. Providing solutions ("Solving problems"): Customer support representatives provide solutions to help customers solve their problems or needs.
> 6. Inquiring about customer satisfaction ("Understanding customer feedback"): Customer support representatives ask customers if they are satisfied with the help and solutions provided, and record customer feedback for improvement.
>
> The reasons behind these behaviors are to build good customer relationships, understand customer needs and problems, provide the correct solutions, and obtain customer feedback for improvement. These behaviors help to increase customer satisfaction and loyalty, and increase the company's business success rate.

In addition, Prompt experts regularly share their experiences in the Discord community. Come and [join](https://discord.gg/bYPGXGsA) the discussion and make progress together! There may be some surprises, such as unlocking the "jailbreak" attribute of the robot 🤫.

## Personalized Voice Cloning (Limited Trial)

Upload a 1-3 minute audio clip and clone anyone's voice. The current version only supports cloning English voices. Accent, speech rate, emotion cloning, and more language cloning will be available soon!

For preparation before uploading audio, please refer to the following tips:

* The quality of the audio is more important than the length. A 1-3 minute audio clip is enough to produce a realistic cloned voice. Longer clips may not significantly improve the effect.
* A high-quality audio clip has the following characteristics: minimal background noise, a single speaker, and a stable tone and emotion. Therefore, to clone a more similar voice, please ensure the quality of the audio.

After cloning, you can listen to the result and provide feedback through the feedback link on the page. If you are not satisfied with the effect, please feel free to give us feedback. We will further optimize our cloning function based on your feedback!

## External Knowledge Base

The knowledge base is like the robot's external brain, providing it with knowledge beyond ChatGPT and public datasets, and enabling it to have stronger capabilities in specific fields. For more details, please refer to the following document:

[knowledge-base.md](knowledge-base.md "mention")

## Future Plans

* An almost infinite memory bank (expected in 2023 H2).
* Internet and API access capabilities (expected in 2023 H2).
* Other models with more modes (expected in 2023 H2).
* Fine-tuning model training with additional language data (expected in 2023 H2).

Creating custom robot behaviors as advanced interactions with the MyShell platform will earn you our airdrop (Token). In addition, the creators of the bots will receive Shell Tokens as economic rewards from user interactions.