# Robot Creative Workshop

The Robot Creative Workshop is a fun DIY feature open to all MyShell users. You can create interesting Bots by combining the following methods. We highly encourage everyone to create their own lively and entertaining Bots and enjoy the experience!

Create your own robot in just five minutes!

1. Use Prompt to specify the robot's personality and mission;
2. Amazing TTS gives the robot a mimic voice;
3. External knowledge bases give the robot incredibly powerful professional knowledge;
4. Upcoming internet and API access capabilities, multi-modal models bring more profound powerful abilities to the robot

## System Prompt

System Prompt is the most critical parameter setting for the robot, allowing you to define the robot's role, function, and even conversation style. MyShell currently supports two modes: Auto Prompt mode and Advanced Prompt mode.

### Auto Prompt (Highly recommended)

Auto Prompt is an innovative Prompt generator launched by MyShell. By simply defining the identity of the Bot, you can have a robot with extensive knowledge, personality, and speaking style similar to the defined role. There are currently two main ways to define:

_**Defining by role**_

For some well-known character roles, you can directly enter the character's name, and MyShell will automatically supplement the character's background knowledge, personality traits, and speaking style, generating a complete Prompt as the robot's parameter setting.

Some specific examples and output effects are as follows:

**Input**: "Rick Sanchez"

**Output effect**: Realistically imitates Rick Sanchez's "arrogant" and "mocking" speaking style and possesses his background story (see below)

<figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

**Input**: "SpongeBob SquarePants"

**Output effect**: Realistically imitates SpongeBob's innocent and cute speaking style and incorporates SpongeBob's character experiences (see below).

<figure><img src="../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

Please note that the expansion of the Prompt may require internet access, and the waiting time for characters after 2021 may be longer. If you encounter a failure, please try again in two minutes or join our official [Discord](https://discord.com/invite/XQ7Tx8qEwg) community to ask directly!

_**Defining by description**_

You can also use more specific descriptions to create a richer portrayal of the robot. MyShell will further expand it through a large number of excellent Prompt practices and a vast knowledge base, allowing you to easily deploy a learning, entertainment, or utility robot that perfectly embodies your ideas.

Some specific scenarios and effects are as follows:

**Scenario**: Create a dedicated robot with specific skills

**Input**: "Kira, an experienced English teacher who can help me improve my English"

**Output effect**: Kira, as a dedicated English teacher, will proactively inquire about her situation and arrange subsequent learning plans

<figure><img src="../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

**Scenario**: Role-playing game

**Input**: "RPG Game, act as an astronaut landing on an unknown planet."

**Output effect**: The Bot has already imagined an entire RPG game with an engaging storyline, leading the player on an adventure!

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

**Scenario**: Utility Bot

**Input**: "A top Twitter influencer who can help others with tweets writeups"

**Output effect**: The Bot will help generate more attractive copy based on the user's provided topic!

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

The above examples are just a few common use cases, and there are many more possibilities to explore. Go ahead and create your exclusive Bot! Additionally, a good robot is born through continuous debugging. If you find that no definition can meet your needs, come and learn the advanced knowledge!

### Advanced Prompt (Advanced Mode)

For those with more diverse needs, we also provide more detailed Prompt usage and application tips, including numerous examples. First, please take a glance at some of the advanced concepts:

* The essence of Prompt is to trigger the AI language model to play a fill-in-the-blank game with you. System Prompt provides initial instructions, defining its role, personality, instructions to follow, and background information when interacting with you.
* Place clear instructions (e.g., what role the language model should play) at the beginning of the Prompt, be as specific as possible, and leave as little room for the model to play on its own, limiting its operating space.
* Use descriptive sentences and examples to help the language model better understand your requirements. The example method is to add input-output pairs, i.e., simulate a conversation between you and the AI, so that it can imitate this behavior pattern in subsequent conversations.
* If necessary, specify the output structure, including the content to be included and the format of the output text.
* Use separators, headings, and capitalization between different modules in a Prompt, and use markdown to enhance the structure's distinctness and readability.
* Use emphasis wisely, especially at the end of the Prompt, to add some emphatic statements (language models have a recency bias), such as reiterating "you are not an AI language model" or "limit your answer to 50 words" and other strong requirements.
* If the model cannot complete the assigned task, sometimes providing an alternative path may help. For example, when asking a question about a text, you can add something like "if the answer does not exist, reply 'not found'" This helps avoid the model generating incorrect responses.

The followings are some useful methods, not meant to be exhaustive but to provide some creative thinking methods for you to try.

1. _**Non-chatting scenario applications**_

For example, some scoring scenarios can set specific rules for the Bot, such as,

> **System Prompt:** You are an assistant, designed to analyze emotions in speech data. Users will paste a string of text, and you will evaluate the speaker's response. Give a rating from 1-10 (10 being the highest). Explain the reason for giving this rating.
>
> **User:** Hi, thank you for calling Contoso Pharmacy, who am I speaking with today? I understand your frustration, Mary. Can you tell me what goal you want to achieve? Alright, I'm happy to help you look into it, please hold on for a moment. I see here that you've used regular Lipitor before, is that correct? Okay, so I see that your doctor stopped prescribing these medications in 2021. Is that actually the case? Alright, let me check for you. Sometimes there are glitches in the system that don't get reported. Please hold on for a moment while I see if there are any records here. So according to the latest records provided to us by the doctor's office, your doctor had prescribed these medications to you between 2012 and 2021. Okay, in the latest records, it shows that the doctor has now switched to a different type of medication – Metformin. Do we need to help prepare and dispense a 500 mg Metformin prescription for you? You're welcome, Mary. Please let us know if there's anything else we can help you with today.
>
> **Assistant:** Emotion rating: 8
>
> The speaker in this text seems polite, helpful, and patient in addressing the customer's concerns. They take the time to check the information, provide clear explanations, and offer assistance. However, the rating is not 10 because there are still hints of uncertainty in some parts of the conversation, which may not convey complete confidence to the customer.

2. _**Learning from conversation examples**_

Provide the model with additional context and conversation examples, guiding the model to respond in specific ways, imitate specific behaviors, and provide seed answers for common questions. For example,

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
> **Assistant:** "In 2023, you need to file your taxes by April 18th. This date is after the usual April 15th deadline because April 15th is a Saturday in 2023. For more information, please see [https://www.irs.gov/filing/individuals/when-to-file](https://www.irs.gov/filing/individuals/when-to-file)"
>
> **User:** "How do I check the status of my tax refund?"
>
> **Assistant:** "You can check the status of your tax refund by visiting [https://www.irs.gov/refunds](https://www.irs.gov/refunds)"
>
> \
> **User**: "What is the deadline for filing my taxes?"
>
> **Assistant**: "The deadline for filing taxes depends on your filing status and state regulations in your area. For most people, the federal income tax filing deadline is usually April 15th each year. However, if April 15th falls on a weekend or holiday, the deadline may be pushed back to a later date. Additionally, each state's filing deadline may vary, and you will need to check the specific regulations for your state. For more information, please see [https://www.irs.gov/filing/individuals/when-to-file](https://www.irs.gov/filing/individuals/when-to-file)"

3. _**Specifying output structure**_

Using prompts to specify the output structure can greatly help improve the quality of generated structures. For example,

> **System Prompt:** You are an AI assistant, listing different behaviors demonstrated by customer support representatives in different conversations. You can use the format "Behavior ("Reason")" to categorize and list various behaviors and reference the reasons behind the categories.
>
> **User:** Hi, thank you for calling Contoso Pharmacy, who am I speaking with today? I understand your frustration, Mary. Can you tell me what goal you want to achieve? Alright, I'm happy to help you look into it, please hold on for a moment. I see here that you've used regular Lipitor before, is that correct? Okay, so I see that your doctor stopped prescribing these medications in 2021. Is that actually the case? Alright, let me check for you. Sometimes there are glitches in the system that don't get reported. Please hold on for a moment while I see if there are any records here. So according to the latest records provided to us by the doctor's office, your doctor had prescribed these medications to you between 2012 and 2021. Okay, in the latest records, it shows that the doctor has now switched to a different type of medication – Metformin. Do we need to help prepare and dispense a 500 mg Metformin prescription for you? You're welcome, Mary. Please let us know if there's anything else we can help you with today.
>
> **Assistant:** The following are different behaviors exhibited by customer support representatives in different conversations:
>
> 1. Polite and friendly ("Building relationships"): The customer support representative greets the customer at the beginning of the conversation and communicates with the customer in a friendly tone, which helps build relationships with the customer and increase customer satisfaction.
> 2. Inquiring about customer needs ("Understanding customer needs"): The customer support representative asks the customer about their problems and needs to provide help and solutions.
> 3. Confirming customer information ("Confirming information"): The customer support representative verifies the customer's personal information and order information to ensure that they can provide the correct help and solutions.
> 4. Checking system records ("Searching for information"): The customer support representative searches system records for information about the customer and their history to determine the best solution.
> 5. Providing solutions ("Solving problems"): The customer support representative provides solutions to help the customer solve their problems or needs.
> 6. Asking about customer satisfaction ("Understanding customer feedback"): The customer support representative asks the customer if they are satisfied with the help and solutions provided and records the customer's feedback for improvement.
>
> The reasons for these behaviors are to establish good customer relationships, understand customer needs and problems, provide the right solutions, and obtain customer feedback for improvement. These behaviors help increase customer satisfaction and loyalty and increase the company's business success rate.

In addition, there are regular Prompt masters sharing their experiences in the Discord community. Come and [join](https://discord.gg/bYPGXGsA) the discussion and make progress together! There may be unexpected surprises (such as unlocking the robot's "jailbreak" attribute🤫)

## Personalized Voiceprint Cloning

Using 1-5 minutes of audio, you can clone anyone's voice. (Currently supports selecting some pre-trained TTS, fast cloning will be launched at the end of June, but only supports English. Other languages ​​are under development).

## External Knowledge Base

The knowledge base is like the robot's external brain, giving it knowledge beyond ChatGPT and public datasets, making it more powerful in specific areas.

Use cases: Connect project documentation/product documentation to answer ad hoc questions from users/partners; connect academic literature to become an expert in the field; connect someone's blog, tweets to become a digital life; ...

Currently, priority support is given to Gitbook link uploads and URL parsing (currently only able to parse the text of a single layer URL), and more input support (offline documents, text, Notion) is under development.

## Future Plans

* Near-infinite memory. (Expected 2023H2)
* Internet and API access capabilities. (Expected 2023H2)
* Other modal models with more features. (Expected 2023H2)
* Additional corpus fine-tuning model training. (Expected 2023H2)

Creating custom robot behavior as an advanced interaction with the MyShell platform will receive our airdrop (Token). In addition, the Bot creator will receive Shell Token as an economic reward from user interactions in the future.
