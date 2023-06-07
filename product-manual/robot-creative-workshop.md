# Robot Creative Workshop

Robot Creative Workshop is a fascinating DIY feature open to all MyShell users. You can combine interesting Bots in the following ways, and we highly encourage everyone to create their own lively and entertaining Bots. Enjoy the experience!

Create your own robot in just five minutes!

1. Use Prompt to specify the robot's personality and mission;
2. Amazing TTS gives the robot a beautiful voice;
3. External knowledge base makes the robot incredibly knowledgeable;
4. Upcoming internet and API access capabilities, multi-modal models bring even more powerful abilities to the robot.

## System Prompt

System Prompt is the most critical parameter setting for the robot, allowing you to define the robot's role, function, and even conversation style. MyShell currently supports two modes: Auto Prompt mode and Advanced Prompt mode.

### Auto Prompt (Strongly Recommended)

Auto Prompt is an innovative Prompt generation tool launched by MyShell. You can have a knowledgeable, characterful, and similar-speaking robot to the defined role with just a simple identity definition of the Bot. There are currently two main ways to define it:

_**By role definition**_

For some well-known character roles, you can directly enter the character's name, and then MyShell will automatically supplement the character's background knowledge, personality traits, and conversation style and generate a complete Prompt as the robot's parameter setting.

Some specific examples and conversation effects are as follows:

**Input**: "Rick Sanchez"

**Conversation effect**: Realistically imitates Rick Sanchez's "arrogant" and "mocking" speaking style and possesses his background story (as shown below)

<figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

**Input**: "SpongeBob SquarePants"

**Conversation effect**: Realistically imitates SpongeBob's innocent and cute speaking style and incorporates SpongeBob's character experiences (as shown below)

<figure><img src="../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

Please note that during the expansion of the Prompt, you may need to connect to the network, and the waiting time for characters after 2021 may be longer. If you encounter a failure, please try again in two minutes or join our official [Discord](https://discord.com/invite/XQ7Tx8qEwg) community to ask directly!

_**By description definition**_

You can also complete a more comprehensive depiction of the robot through more specific descriptions. MyShell will further expand it through a large number of excellent Prompt practices and a vast knowledge base, and you can easily deploy a learning, entertainment, or utility robot that perfectly reflects your ideas.

Some specific scenarios and effects are as follows:

**Scenario**: Creating a dedicated robot with specific skills

**Input**: "Kira, an experienced English teacher who can help me improve my English"

**Conversation effect**: Kira, as a dedicated English teacher, will proactively ask about her situation and arrange subsequent learning plans

<figure><img src="../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

**Scenario**: Role-playing game

**Input**: "RPG Game, act as an astronaut landing on an unknown planet."

**Conversation effect**: The Bot has already imagined an entire RPG game with an engaging storyline in just one sentence, leading players on an adventure together!

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

**Scenario**: Utility Bot

**Input**: "A top Twitter influencer who can help others with tweets writeups"

**Conversation effect**: The Bot will help generate more attractive copy based on the user's provided topic!

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

The above are some common use cases. Feel free to explore more possibilities and create your exclusive Bot! Also, a good robot is born through continuous debugging. If you find that no definition can meet your needs, come and learn about the advanced knowledge!

### Advanced Prompt (Advanced Edition)

For friends with more diverse needs, we also provide more detailed Prompt usage and some application tips, including a wealth of examples. First, please understand the advanced concepts of Prompt:

* The essence of Prompt is to trigger the AI language model to play a fill-in-the-blank game with you. System Prompt provides initial instructions, defining its role, personality, instructions to follow, and background information when interacting with you.
* Place clear instructions (such as what role the language model should play) at the beginning of the Prompt, be as specific as possible, and leave as little room for the model to improvise, limiting its operating space.
* Use descriptive statements and examples to help the language model better understand your requirements. The example method is to add input-output pairs, i.e., simulate a conversation between you and the AI so that it can imitate this behavior pattern in subsequent conversations.
* If necessary, specify the structure of the output, including the content to be included and the format of the output text.
* Use separators, headings, capitalization, etc., between different modules in a Prompt, and use markdown to enhance the structure's distinctiveness and readability.
* Use emphasis, especially at the end of the Prompt, to add some emphatic statements (language models have a recency bias), such as re-emphasizing "you are not an AI language model" or "keep your answer within 50 words" and other strong requirements.
* If the model cannot complete the assigned task, sometimes providing an alternative path can help. For example, when asking a question about a text, you can add something like "If the answer does not exist, reply 'not found.'" This helps avoid the model generating incorrect responses.

The following are some methods of use, but they do not mean exhaustive but provide some creative thinking methods that you can try.

1. _**Non-chat scenario applications**_

For example, some scoring scenarios can set specific rules for the Bot, such as,

> **System Prompt:** You are an assistant, aiming to analyze emotions in speech data. Users will paste a string of text, and you will evaluate the speaker's response. Give a 1-10 rating (10 being the highest). Explain the reason for this rating.
>
> **User:** Hi, thank you for calling Contoso Pharmacy, who am I speaking with today? I understand your frustration, Mary. Can you tell me what goal you want to achieve? Alright, I'm happy to help you take a look, please wait a moment. I see here that you have used regular Lipitor before, is that correct? Okay, so I see that your doctor stopped prescribing these medications in 2021. Is that actually the case? Alright, let me check for you. Because sometimes there are loopholes in the system that don't get reported. Please wait a moment while I see if there are any records here. So according to the latest records provided to us by the doctor's office, your doctor has prescribed these medications for you between 2012 and 2021. Alright, the latest records show that the doctor has now switched to a different type of medication – Metformin. Do we need to help prepare and dispense the 500 mg Metformin prescription for you? You're welcome, Mary, please let us know if there's anything else we can help you with today.
>
> **Assistant:** Emotion rating: 8
>
> The speaker in this text seems to be polite, helpful, and patient when addressing the customer's concerns. They take the time to check the information, provide clear explanations, and offer assistance. However, the rating is not 10 because some parts of the conversation still imply uncertainty, which may not convey complete confidence to the customer.

2. _**Dialogue example learning**_

Provide additional context and conversation examples for the model, guiding the model to respond in a specific way, imitate specific behaviors, and provide seed answers for common questions. For example,

> **System Prompt:** The assistant is an intelligent chatbot designed to help users answer their tax-related questions.
>
> Instructions
>
> * Answer only tax-related questions.
> * If you are unsure of the answer, you can say "I don't know" or "I'm not sure" and suggest the user visit the IRS website for more information.
>
> Example
>
> **User:** "What is the deadline for filing my taxes?"
>
> **Assistant:** "In 2023, you need to file your taxes by April 18th. This date is after the usual April 15th deadline because April 15th is a Saturday in 2023. For more information, please see \[[https://www.irs.gov/filing/individuals/when-to-file](https://www.irs.gov/filing/individuals/when-to-file)]"
>
> **User:** "How do I check the status of my tax refund?"
>
> **Assistant:** "You can check the status of your tax refund by visiting \[[https://www.irs.gov/refunds](https://www.irs.gov/refunds)]"
>
> \
> **User**: "What is the deadline for filing my taxes?"
>
> **Assistant**: "The deadline for filing your taxes depends on your filing form and the state regulations in your area. For most people, the federal income tax filing deadline is usually April 15th each year. However, if April 15th falls on a weekend or holiday, the deadline may be extended to a later date. Additionally, each state's filing deadline may vary, and you will need to check the specific regulations for your state. For more information, please see \[[https://www.irs.gov/filing/individuals/when-to-file](https://www.irs.gov/filing/individuals/when-to-file)]"

3. _**Specify output structure**_

Using prompts to specify the output structure can greatly help the quality of the generated structure. For example,

> **System Prompt:** You are an AI assistant, listing the different behaviors exhibited by customer support representatives in different conversations. You can categorize and list various behaviors using the format "Behavior ("Reason")" and cite the reasons behind the classifications.
>
> **User:** Hi, thank you for calling Contoso Pharmacy, who am I speaking with today? I understand your frustration, Mary. Can you tell me what goal you want to achieve? Alright, I'm happy to help you take a look, please wait a moment. I see here that you have used regular Lipitor before, is that correct? Okay, so I see that your doctor stopped prescribing these medications in 2021. Is that actually the case? Alright, let me check for you. Because sometimes there are loopholes in the system that don't get reported. Please wait a moment while I see if there are any records here. So according to the latest records provided to us by the doctor's office, your doctor has prescribed these medications for you between 2012 and 2021. Alright, the latest records show that the doctor has now switched to a different type of medication – Metformin. Do we need to help prepare and dispense the 500 mg Metformin prescription for you? You're welcome, Mary, please let us know if there's anything else we can help you with today.
>
> **Assistant:** The following are the different behaviors exhibited by customer support representatives in different conversations:
>
> 1. Polite and friendly ("Building relationships"): The customer support representative greets the customer at the beginning of the conversation and communicates with the customer in a friendly tone, which helps build relationships with the customer and increase customer satisfaction.
> 2. Asking for customer needs ("Understanding customer needs"): The customer support representative asks the customer about their problems and needs so that they can provide help and solutions.
> 3. Confirming customer information ("Confirming information"): The customer support representative verifies the customer's personal information and order information to ensure that they can provide the correct help and solutions.
> 4. Checking system records ("Searching for information"): The customer support representative searches system records for information and historical records about the customer and determines the best solution.
> 5. Providing solutions ("Solving problems"): The customer support representative provides solutions to help the customer resolve their problems or needs.
> 6. Asking for customer satisfaction ("Understanding customer feedback"): The customer support representative asks the customer if they are satisfied with the help and solutions provided and records the customer's feedback for improvement.
>
> The reasons for these behaviors are to establish good customer relationships, understand customer needs and problems, provide the correct solutions, and obtain customer feedback for improvement. These behaviors help increase customer satisfaction and loyalty and increase the company's business success rate.

In addition to this, there are regular Prompt masters sharing their experiences in the Discord community. Come and [join](https://discord.gg/bYPGXGsA) the discussion, progress together, and there may be unexpected surprises (such as unlocking the robot's "jailbreak" attribute 🤫).

## Personalized Voiceprint Cloning

Use 1-5 minutes of audio to clone anyone's voice. (Currently supports selecting some pre-trained TTS, fast cloning will be launched at the end of June, but only supports English, other languages ​​are under development).

## External Knowledge Base

The knowledge base is like the robot's external brain, giving it knowledge beyond ChatGPT and public data sets, making it more powerful in specific fields.

Use cases: Connect project documentation/product documentation to answer user/partner ad hoc questions; connect academic literature to become an expert in the field; connect someone's blog/tweets to become a digital life; ...

Priority support is currently given to Gitbook link uploads, and more input support (offline documents, text, blog articles, and other online links, Notion) is under development.

## Upcoming Plans

* Near-infinite memory. (Expected 2023H2)
* Internet and API access capabilities. (Expected 2023H2)
* More modalities of other models. (Expected 2023H2)
* Additional corpus fine-tuning model training. (Expected 2023H2)

Creating custom robot behavior as an advanced interaction with the MyShell platform will earn our airdrop (Token). In addition, the subsequent Bot creator will receive Shell Tokens as an economic reward from user interactions.