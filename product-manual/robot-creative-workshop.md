# Robot Creative Workshop

Robot Creative Workshop is a fun DIY feature open to all MyShell users. You can create interesting Bots by combining various elements in the following ways. We highly encourage everyone to create lively and entertaining Bots and enjoy the experience!

Create your own robot in just five minutes!

1. Use Prompt to specify the robot's personality and mission;
2. Amazing TTS gives the robot a pleasant voice;
3. External knowledge base gives the robot unparalleled professional knowledge;
4. Upcoming internet and API access capabilities, multi-modal models give the robot deeper powerful abilities.

## System Prompt

System Prompt is the most critical parameter setting for robots, allowing you to define the robot's role, function, and even conversation style. MyShell currently supports two modes: Auto Prompt mode and Advanced Prompt mode.

### Auto Prompt (strongly recommended)

Auto Prompt is an innovative Prompt generator launched by MyShell. By simply defining the identity of the Bot, you can have a robot with extensive knowledge, personality, and speaking style similar to the defined role. There are currently two main ways to define:

_**Defining by role**_

For some well-known characters, you can directly enter the character's name, and MyShell will automatically supplement the character's background knowledge, personality traits, and conversation style to generate a complete Prompt as the robot's parameter setting.

Some specific examples and dialogue effects are as follows:

**Input**: "Rick Sanchez"

**Dialogue effect**: Realistically imitates Rick Sanchez's "arrogant", "mocking" speaking style and possesses his background story (see below).

<figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

**Input**: "SpongeBob SquarePants"

**Dialogue effect**: Realistically imitates SpongeBob's innocent and cute speaking style, and incorporates SpongeBob's character experiences (see below).

<figure><img src="../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

Please note that during the expansion of the Prompt, network access may be required, and the waiting time for characters after 2021 may be longer. If you encounter a failure, please try again in two minutes or join our official [Discord](https://discord.com/invite/XQ7Tx8qEwg) community to ask directly!

_**Defining by description**_

You can also use more specific descriptions to create a more detailed portrayal of the robot. MyShell will further expand it through a large number of excellent Prompt practices and a vast knowledge base, allowing you to easily deploy a learning, entertainment, or utility robot that perfectly reflects your ideas.

Some specific scenarios and effects are as follows:

**Scenario**: Create a dedicated robot with specific skills

**Input**: "Kira, an experienced English teacher who can help me improve my English"

**Dialogue effect**: Kira, as a dedicated English teacher, will proactively ask about her situation and arrange a follow-up study plan.

<figure><img src="../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

**Scenario**: Role-playing game

**Input**: "RPG Game, act as an astronaut landing on an unknown planet."

**Dialogue effect**: The Bot has imagined an entire RPG game with an engaging storyline in just one sentence, leading players on an adventure together!

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

**Scenario**: Utility Bot

**Input**: "A top Twitter influencer who can help others with tweets writeups"

**Dialogue effect**: The Bot will help generate more attractive copy based on the topics provided by the user!

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

The above are some common use cases; feel free to explore more possibilities and create your exclusive Bot! Also, a good robot is born through constant debugging. If you find that no definition can meet your needs, learn about the advanced version of knowledge!

### Advanced Prompt (Advanced Edition)

For those with more diverse needs, we also provide more detailed usage and application tips for Prompt, including a wealth of examples. First, please understand the advanced concepts of Prompt:

* The essence of Prompt is to trigger the AI language model to play a fill-in-the-blank game with you. The System Prompt provides initial instructions, defining its role, personality, instructions to follow, and background information when interacting with you.
* Place clear instructions (e.g., what role the language model should play) at the beginning of the Prompt, be as specific as possible, and leave as little room for the model to improvise as possible, limiting its operating space.
* Use descriptive statements and examples to help the language model better understand your requirements. The example method is to add input-output pairs, i.e., simulate a conversation between you and the AI so that it can imitate this behavior pattern in subsequent conversations.
* If necessary, specify the output structure, including the content to be included and the format of the output text.
* Use separators, headings, and capitalization between different modules in a Prompt, and use markdown to enhance the structure's distinctiveness and readability.
* Use emphasis wisely, especially at the end of the Prompt, to add some emphasis statements (language models have a recency bias), such as reiterating "you are not an AI language model" or "keep your answer within 50 words" and other strong requirements.
* If the model cannot complete the assigned task, sometimes providing an alternative path may help. For example, when asking a question about a text, you can add content like "if the answer does not exist, reply 'not found'". This helps to avoid the model generating incorrect responses.

The following are some methods of use, but it does not mean exhaustive, but rather provides some creative thinking methods that you can try.

1. _**Non-chat scenario applications**_

For example, some game-like scenarios can set specific rules for the Bot, such as,

> **System Prompt:** You are an assistant, aimed at analyzing emotions in speech data. Users will paste a string of text, and you will evaluate the speaker's response. Give a score of 1-10 (10 being the highest). Explain the reasons for giving this score.
>
> **User:** Hi, thank you for calling Contoso Pharmacy, who am I speaking with today? I understand your frustration, Mary. Can you tell me what goal you want to achieve? Okay, I'd be happy to help you take a look, please hold on for a moment. I see here that you've used regular Lipitor before, is that correct? Alright, so I see that your doctor stopped prescribing these medications in 2021. Is that actually the case? Okay, let me check that for you. Sometimes there are glitches in the system, and they don't get reported. Please hold on for a moment, and let me see if there are any records here. So, according to the latest records provided to us by the doctor's office, your doctor has prescribed these medications for you between 2012 and 2021. Alright, in the latest records, it shows that the doctor has now switched to a different type of medication – Metformin. Do we need to help prepare and dispense the 500 mg Metformin prescription for you? You're welcome, Mary. Please let us know if there's anything else we can help you with today.
>
> **Assistant:** Emotion rating: 8
>
> The speaker in this text seems to be polite, helpful, and patient in addressing the customer's concerns. They take the time to check the information, provide clear explanations, and offer assistance. However, the score is not 10 because some parts of the conversation still imply uncertainty, which may not convey complete confidence to the customer.

2. _**Learning from dialogue examples**_

Provide additional context and dialogue examples for the model, guiding the model to respond in a specific way, imitate specific behaviors, and provide seed answers for common questions. For example,

> **System Prompt:** The assistant is an intelligent chatbot designed to help users answer their tax-related questions.
>
> Instructions
>
> * Only answer tax-related questions.
> * If you are unsure of the answer, you can say "I don't know" or "I'm not sure" and suggest that the user visit the IRS website for more information.
>
> Examples
>
> **User:** "What is the deadline for filing my taxes?"
>
> **Assistant:** "In 2023, you need to file your taxes by April 18th. This date is after the usual April 15th deadline because April 15th falls on a Saturday in 2023. For more information, please see \[[https://www.irs.gov/filing/individuals/when-to-file](https://www.irs.gov/filing/individuals/when-to-file)]"
>
> **User:** "How can I check the status of my tax refund?"
>
> **Assistant:** "You can check the status of your tax refund by visiting \[[https://www.irs.gov/refunds](https://www.irs.gov/refunds)]"
>
> \
> **User**: "What is the deadline for filing my taxes?"
>
> **Assistant**: "The tax filing deadline depends on your filing status and state regulations where you reside. For most people, the federal income tax filing deadline is usually April 15th each year. However, if April 15th falls on a weekend or holiday, the deadline may be pushed back to a later date. Additionally, each state's tax filing deadline may vary, and you will need to check the specific regulations for your state. For more information, please see \[[https://www.irs.gov/filing/individuals/when-to-file](https://www.irs.gov/filing/individuals/when-to-file)]"

3. _**Specifying output structure**_

Using prompts to specify the output structure can greatly help the quality of the generated structure. For example,

> **System Prompt:** You are an AI assistant, listing the different behaviors exhibited by customer support representatives in different conversations. Use the "Behavior ("Reason")" format to categorize and list various behaviors and reference the reasons behind the categories.
>
> **User:** Hi, thank you for calling Contoso Pharmacy, who am I speaking with today? I understand your frustration, Mary. Can you tell me what goal you want to achieve? Okay, I'd be happy to help you take a look, please hold on for a moment. I see here that you've used regular Lipitor before, is that correct? Alright, so I see that your doctor stopped prescribing these medications in 2021. Is that actually the case? Okay, let me check that for you. Sometimes there are glitches in the system, and they don't get reported. Please hold on for a moment, and let me see if there are any records here. So, according to the latest records provided to us by the doctor's office, your doctor has prescribed these medications for you between 2012 and 2021. Alright, in the latest records, it shows that the doctor has now switched to a different type of medication – Metformin. Do we need to help prepare and dispense the 500 mg Metformin prescription for you? You're welcome, Mary. Please let us know if there's anything else we can help you with today.
>
> **Assistant:** Here are the different behaviors exhibited by customer support representatives in different conversations:
>
> 1. Polite and friendly ("Building rapport"): Customer support representatives greet customers at the beginning of the conversation and communicate with them in a friendly tone, which helps build rapport with customers and increase customer satisfaction.
> 2. Inquiring about customer needs ("Understanding customer needs"): Customer support representatives ask customers about their problems and needs in order to provide help and solutions.
> 3. Confirming customer information ("Confirming information"): Customer support representatives verify the customer's personal information and order information to ensure that they can provide the correct help and solutions.
> 4. Checking system records ("Finding information"): Customer support representatives search system records for information and history about the customer and determine the best solution.
> 5. Providing solutions ("Solving problems"): Customer support representatives provide solutions to help customers solve their problems or needs.
> 6. Asking about customer satisfaction ("Understanding customer feedback"): Customer support representatives ask customers if they are satisfied with the help and solutions provided and record customer feedback for improvement.
>
> The reasons for these behaviors are to establish good customer relationships, understand customer needs and problems, provide the correct solutions, and obtain customer feedback for improvement. These behaviors help to increase customer satisfaction and loyalty and improve the company's business success rate.

In addition, there are regular Prompt experts sharing their experiences in the Discord community. Come and [join](https://discord.gg/bYPGXGsA) the discussion, progress together, and there may be unexpected surprises (such as unlocking the robot's "jailbreak" attribute🤫).

## Personalized Voice Cloning

Use 1-5 minutes of audio to clone anyone's voice (currently supports selecting some pre-trained TTS, quick cloning will be launched at the end of June, but only supports English, other languages are under development).

## External Knowledge Base

The knowledge base is like the external brain of the robot, giving it knowledge beyond ChatGPT and public datasets, and making it more powerful in specific fields.

Use cases: Connect project documents/product documents to answer user/partner ad hoc questions; connect academic literature to become an expert in the field; connect someone's blog, tweets to become a digital life; ...

Priority support is given to Gitbook link uploads and URL parsing (currently only able to parse one level of URL text), and more input format support (offline documents, text, Notion) is under development.

## Future Plans

* Near-infinite memory storage. (Expected 2023H2)
* Internet and API access capabilities. (Expected 2023H2)
* More modalities of other models. (Expected 2023H2)
* Additional corpus fine-tuning model training. (Expected 2023H2)

Creating custom robot behavior as an advanced interaction with the MyShell platform will earn our airdrop (Token). In addition, the subsequent Bot creator will receive Shell Token as an economic reward from user interactions.