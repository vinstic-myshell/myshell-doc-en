# Robot Creative Workshop

Robot Creative Workshop is a fun DIY feature, open to all MyShell users. You can combine interesting Bots in the following ways, and we strongly encourage everyone to create their own lively and entertaining Bots to enjoy!

Create your own robot in just five minutes!

1. Use Prompt to specify the robot's personality and mission;
2. Amazing TTS gives the robot a pleasing voice;
3. External knowledge base gives the robot incredibly powerful professional knowledge;
4. Upcoming internet and API access capabilities, multi-modal models bring even more powerful abilities to the robot

## System Prompt

The System Prompt is the most critical parameter setting for the robot, allowing you to define the robot's role, function, and even conversation style. MyShell currently supports two modes: Auto Prompt mode and Advanced Prompt mode.

### Auto Prompt (strongly recommended)

Auto Prompt is an innovative Prompt generation tool launched by MyShell. You can have a knowledgeable, characterful, and similar-speaking robot with a simple identity definition for the Bot. There are currently two main ways to define it:

_**Defining by role**_

For some well-known character roles, you can directly enter the character's name, and then MyShell will automatically supplement the character's background knowledge, personality traits, and conversation style to generate a complete Prompt as the robot's parameter setting.

Some specific examples and conversation effects are as follows:

**Input**: "Rick Sanchez"

**Conversation effect**: Realistically imitates Rick Sanchez's "arrogant", "mocking" way of speaking and has his background story (as shown below)

<figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

**Input**: "SpongeBob SquarePants"

**Conversation effect**: Realistically imitates SpongeBob's innocent and cute way of speaking, and brings in SpongeBob's role experience (as shown below)

<figure><img src="../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

Please note that expanding the Prompt may require internet access, and characters after 2021 may have a longer wait time. If you encounter a failure, please try again in two minutes or join our official [Discord](https://discord.com/invite/XQ7Tx8qEwg) community to ask questions directly!

_**Defining by description**_

You can also complete a richer portrayal of the robot through more specific descriptions. MyShell will further expand it through a large number of excellent Prompt practices and a huge knowledge base, and you can easily deploy a learning, entertainment, or utility robot that perfectly embodies your ideas.

Some specific scenarios and effects are as follows:

**Scenario**: Create a dedicated robot with specific skills

**Input**: "Kira, an experienced English teacher who can help me improve my English"

**Conversation effect**: Kira, as a dedicated English teacher, will proactively inquire about her situation and arrange a follow-up study plan

<figure><img src="../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

**Scenario**: Role-playing game

**Input**: "RPG Game, act as an astronaut landing on an unknown planet."

**Conversation effect**: The Bot has already imagined a whole RPG game with an engaging storyline, leading the player on an adventure!

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

**Scenario**: Utility Bot

**Input**: "A top Twitter influencer who can help others with tweet writeups"

**Conversation effect**: The Bot will help generate more attractive copy based on the topic provided by the user!

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

The above lists some common use cases, and you're welcome to explore more possibilities. Go create your exclusive Bot! Also, a good robot is born through constant debugging. If you find that no definition can meet your needs, come and learn the advanced knowledge!

### Advanced Prompt (Advanced Edition)

For friends with more diverse needs, we also provide more detailed usage and application tips for Prompt, including a wealth of examples. First, please understand the advanced concepts of Prompt:

* The essence of Prompt is to trigger the AI language model to play a fill-in-the-blank game with you. The System Prompt provides initial instructions, defining its role, personality, instructions to follow, and background information when interacting with you.
* Put clear instructions (such as what role the language model should play) at the beginning of the Prompt, be as specific as possible, and leave as little room for the model to play, limiting its operating space.
* Use descriptive statements and examples to help the language model better understand your requirements. The example method is to add input-output pairs, i.e., simulate a conversation between you and the AI, so that it can imitate this behavior pattern in subsequent conversations.
* If necessary, specify the structure of the output, including the content to be included and the format of the output text.
* Use separators, headings, capitalization, etc., between different modules in a Prompt, and markdown can also be used to enhance the distinctiveness and readability of the structure.
* Use emphasis, especially at the end of the Prompt, to add some emphasis statements (the language model has a recency bias), such as re-emphasizing "you are not an AI language model" or "keep your answer within 50 words" and other strong requirements.
* If the model cannot complete the assigned task, sometimes providing an alternative path may help. For example, when asking a question about a piece of text, you can add something like "if the answer does not exist, reply 'not found'". This helps to avoid the model generating incorrect responses.

The following will introduce some usage methods, but it does not mean exhaustive, but to provide some creative thinking methods that you can try.

1. _**Non-chat scenario applications**_

For example, some scoring scenarios can set specific rules for the Bot, such as,

> **System Prompt:** You are an assistant, aimed at analyzing the emotions in voice data. Users will paste a string of text, and you will evaluate the speaker's response. Give a 1-10 rating (10 being the highest). Explain the reason for giving this rating.
>
> **User:** Hi, thank you for calling Contoso Pharmacy, who am I speaking with today? I understand your frustration, Mary. Can you tell me what goal you want to achieve? Okay, I'd be happy to take a look for you, please hold on for a moment. I see here that you've used regular Lipitor before, is that correct? Okay, so I see that your doctor stopped prescribing these medications in 2021. Is that actually the case? Alright, let me check for you. Because sometimes there are glitches in the system and they don't get reported. Please hold on for a moment, let me see if there's any record here. So according to the latest records provided to us by the doctor's office, your doctor had prescribed these medications to you between 2012 and 2021. Alright, in the latest records, it shows that the doctor has now switched to a different type of medication – Metformin. Do we need to help prepare and dispense a 500 mg Metformin prescription for you? You're welcome, Mary. Please let us know if there's anything else we can help you with today.
>
> **Assistant:** Emotion Rating: 8
>
> The speaker in this text seems to be polite, helpful, and patient when addressing the customer's concerns. They take the time to check the information, provide clear explanations, and offer assistance. However, the rating is not 10 because some parts of the conversation still hint at uncertainty, which may not convey complete confidence to the customer.

2. _**Dialogue example learning**_

Provide the model with additional context and dialogue examples to guide the model to respond in a specific way, imitate specific behaviors, and provide seed answers for common questions. For example,

> **System Prompt:** The assistant is an intelligent chatbot designed to help users answer their tax-related questions.
>
> Instructions
>
> * Answer tax-related questions only.
> * If you are unsure of the answer, you can say "I don't know" or "I'm not sure" and suggest the user visit the IRS website for more information.
>
> Example
>
> **User:** "What is the deadline for filing my taxes?"
>
> **Assistant:** "In 2023, you need to file your taxes by April 18th. This date is after the usual April 15th deadline, as April 15th is a Saturday in 2023. For more information, please refer to \[[https://www.irs.gov/filing/individuals/when-to-file](https://www.irs.gov/filing/individuals/when-to-file)]"
>
> **User:** "How can I check my tax refund status?"
>
> **Assistant:** "You can check your tax refund status by visiting \[[https://www.irs.gov/refunds](https://www.irs.gov/refunds)]"
>
> \
> **User:** "What is the deadline for filing my taxes?"
>
> **Assistant:** "The deadline for filing your taxes depends on your filing form and the state regulations in your area. For most people, the federal income tax filing deadline is usually April 15th each year. However, if April 15th falls on a weekend or holiday, the deadline may be pushed back to a later date. In addition, each state's filing deadline may vary, and you will need to check the specific regulations in your state. For more information, please refer to \[[https://www.irs.gov/filing/individuals/when-to-file](https://www.irs.gov/filing/individuals/when-to-file)]"

3. _**Specify output structure**_

Using the prompt to specify the output structure will greatly help the quality of the generated structure. For example,

> **System Prompt:** You are an AI assistant, listing the different behaviors exhibited by customer support representatives in different conversations. Classify and list the various behaviors using the "Behavior ("Reason")" format and reference the reasons behind the classifications.
>
> **User:** Hi, thank you for calling Contoso Pharmacy, who am I speaking with today? I understand your frustration, Mary. Can you tell me what goal you want to achieve? Okay, I'd be happy to take a look for you, please hold on for a moment. I see here that you've used regular Lipitor before, is that correct? Okay, so I see that your doctor stopped prescribing these medications in 2021. Is that actually the case? Alright, let me check for you. Because sometimes there are glitches in the system and they don't get reported. Please hold on for a moment, let me see if there's any record here. So according to the latest records provided to us by the doctor's office, your doctor had prescribed these medications to you between 2012 and 2021. Alright, in the latest records, it shows that the doctor has now switched to a different type of medication – Metformin. Do we need to help prepare and dispense a 500 mg Metformin prescription for you? You're welcome, Mary. Please let us know if there's anything else we can help you with today.
>
> **Assistant:** Below are the different behaviors exhibited by customer support representatives in different conversations:
>
> 1. Polite and friendly ("Building relationships"): The customer support representative greets the customer at the beginning of the conversation and communicates with the customer in a friendly tone, which helps build relationships with the customer and increase customer satisfaction.
> 2. Inquiring about customer needs ("Understanding customer needs"): The customer support representative asks the customer about their problems and needs in order to provide help and solutions.
> 3. Confirming customer information ("Confirming information"): The customer support representative verifies the customer's personal information and order information to ensure that they can provide the correct help and solutions.
> 4. Checking system records ("Finding information"): The customer support representative searches the system records for information and history about the customer and determines the best solution.
> 5. Providing solutions ("Solving problems"): The customer support representative provides solutions to help the customer solve their problems or needs.
> 6. Asking about customer satisfaction ("Understanding customer feedback"): The customer support representative asks the customer if they are satisfied with the help and solutions provided and records the customer's feedback for improvement.
>
> The reasons for these behaviors are to establish good customer relationships, understand customer needs and problems, provide the correct solutions, and obtain customer feedback for improvement. These behaviors help to increase customer satisfaction and loyalty and increase the company's business success rate.

In addition to this, there are regular Prompt masters sharing their insights in the Discord community, so come [join](https://discord.gg/bYPGXGsA) the discussion and make progress together! There may be unexpected surprises (such as unlocking the robot's "jailbreak" attribute 🤫)

## Personalized Voiceprint Cloning

Using 1-5 minutes of audio, you can clone anyone's voice. (Currently, you can choose some pre-trained TTS, and fast cloning will be launched at the end of June, but only supports English, and other languages are under development).

## External Knowledge Base

The knowledge base is like the robot's external brain, giving it knowledge beyond ChatGPT and public datasets, and making it more powerful in specific domains.

Use cases: Connect to project documentation/product documentation to answer user/partner ad hoc questions; connect to academic literature to become an expert in the field; connect to someone's blog/tweets to become a digital life;...

Currently, Gitbook link upload and URL parsing are prioritized (currently only able to parse one level of URL text), and more input format support (offline documents, text, Notion) is under development.

## Future Plans

* Near-infinite memory. (Expected 2023H2)
* Internet and API access capabilities. (Expected 2023H2)
* More modalities of other models. (Expected 2023H2)
* Additional corpus fine-tuning model training. (Expected 2023H2)

Creating custom robot behavior as an advanced interaction with the MyShell platform will earn our airdrop (Token). In addition, the Bot creator will receive Shell Token as an economic reward from user interactions.