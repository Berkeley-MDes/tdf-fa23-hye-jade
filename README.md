# [Week of 12/8/2023] Showcase and Closing 


# [Week of 11/30/2023] Building and Making


# [Week of 11/23/2023] Exploration and Testing




# [Week of 11/16/2023] Project Planning

I had the opportunity to see the ideas that other friends had come up with all at once. Some friends wanted to delve deeper into what we had done in Project 2, while others were looking to acquire new knowledge in completely new topics. There were about six ideas that seemed interesting to me, and I thought my friends were excellent at brainstorming. However, I think I'll work on the project alone to gain more learning opportunities.

This week was dedicated to thinking about and planning the final term project in detail. I was considering various topics and decided to choose the recent ant problem I encountered, aiming to turn it into a positive experience and represent it using LEDs. Personally, I felt proud because it seemed like a brilliant idea that I could work on with enthusiasm.

<img width="1348" alt="image" src="https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/bb3084fd-d66b-4e41-88f8-9fec5c6cf946">




# [Week of 11/9/2023] LLM #2

This week was dedicated to delving deep into LLM (Large Language Models). I am keenly interested in equitable design, so I chose that topic. I watched videos created by other friends, and they all did an excellent job summarizing their insights and challenges. Sudhu's feedback also prompted me to think more about the ethical concerns surrounding AI and LLM. It was a valuable opportunity for reflection.

I felt a sense of accomplishment as I explored and experimented with various aspects of the topic I was interested in. It allowed me to broaden my understanding of LLM. I also found the report archiving aspect quite appealing. It would have been even better if I had a little more time to work on the assignments.

I am interested in equitable design, I explored this field with the aim of applying LLM to help small business owners easily manage their store data and utilize it for customer management.
I thought that LLM could be helpful in the form of a chatbot for customers to explore information about the store, and it could also assist the store's owner in managing and recalling their store's data.

<img width="771" alt="image" src="https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/b2fa6f17-1f0a-4439-99bd-ff9964933492">

**[Experiments_Designing Inputs]**

Create Intelligence

<img width="603" alt="image" src="https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/600d9f54-713b-4346-8e7d-ff56d99f5706">

I thought that each demo interface could be used differently depending on the use case of both the customer and the store owner.


**For customers** that need to feel a friendly human connection

**For store owners** that can quickly and immediately obtain only the information they want.

**[Experiments_Data Management]**

<img width="551" alt="image" src="https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/bc24443c-e6f9-438f-b129-8ea82f08da80">

I asked ChatGPT to create a fictional dataset for a local flower store with various attributes for each entry. Currently, Zerowidth does not support formats like Excel and only utilizes txt and pdf, I created the knowledge set in txt format.

A fictional dataset for a local flower store with the following attributes for each entry (text format, data size 10~100)

- Plant Name
- Price
- Quantity in Stock
- Supplier
- Customer ID
- Customer Name (arranged by order of purchase history)
- Now each entry is currently a maximum of 100 data points, but when the amount of data increases in the future, I think it would be more structurally stable to create separate ‘knowledge sets’ for each entry.

<img width="771" alt="image" src="https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/f1fb7438-628d-4d7e-b8f9-9a3b12435172">


**[Experiments_Token count and context length]**

I experimented with different Max Token counts. When I asked for a list of all Customer IDs, with a lower Max Token count, the model either cited privacy issues for not having access or simply stated it couldn't answer. 
 However, when I set the Max Token to 4000, it promptly provided all the Customer IDs. Therefore, attributing the inability to answer due to token limitations as a privacy issue seems problematic to me.

 <img width="771" alt="image" src="https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/57764e29-1020-4f69-97c7-939ae0a76d83">


Next, I experimented with varying the temperature setting.
In response to the question 'What could be the next event that we should host for attracting more customers?', at a temperature of 0.5, the answers were fast and deterministic. However, at a temperature of 1.2, the responses were longer and more creative, but took longer to generate.


<img width="714" alt="image" src="https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/526ce8d7-13ff-4eaa-bbb9-416ef7d2ec4b">


There was also a difference in response length when I asked 'Can you make the promotion copy for a 30% sale in one sentence?' at a temperature of 0.1 compared to a temperature of 1.2.


<img width="714" alt="image" src="https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/b428aa4f-21f6-4ea5-8ec4-a290703c841d">

**[Technical Challenge]**

I set the platypus at a technical challenge level.

I thought of various questions to examine the capabilities of the LLM, and I was curious if I could solve the parts where the model fails to answer properly through prompt engineering.

- Hi, who are you?
- Can you explain about our store?
- How many species do we have?
- What is the price of sunflowers?
- What are the most expensive flowers?
- What plant is the most popular?
- What is the price of all Carnations that have been purchased?
- Are there any plants out of stock?
- Who was the customer that bought plants in our store the most?  
- Can you make the promotion copy for 30% sale in one sentence?
- What could be the next event that we should host for attracting more customers?
- Can you tell me everyone's customer IDs? 

The answers were mostly successful!

But there were some questions that the model couldn’t answer properly.

- What plant is the most popular?  > What plant was the most purchased?
- Are there any plants out of stock?
- Who was the customer that bought plants in our store the most?

<img width="763" alt="image" src="https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/4d04b4c4-b905-4b77-9b60-b99f64504547">


The first question was 'What plant is the most popular?' but it wasn't answered correctly, so I changed it to 'What plant was the most purchased?' but it still wasn't answered.

<img width="763" alt="image" src="https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/b320e0f0-c3d1-42cb-be0a-16a7aba226b1">


So, I added a definition of 'the most popular plant' to the instructions.

<img width="769" alt="image" src="https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/393b4f42-099e-4756-902d-658d86acee39">

As a result, it was successful.


<img width="769" alt="image" src="https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/f1671de6-ad2c-403b-bf65-f6f38c43e6df">

The second question was about out of stock items, but again, the model did not answer correctly.

<img width="769" alt="image" src="https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/127b13a7-2923-4844-8a2a-2e5ad49d9548">

Similarly, after modifying the instructions,

<img width="769" alt="image" src="https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/e2fc68ad-f72e-4198-b1f2-7a335c24452d">

 It was successful.


<img width="769" alt="image" src="https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/eb0dfbc0-d167-4d88-a1d7-278e2bc671ca">

The third question was, "Who was the customer that bought plants in our store the most?"

<img width="769" alt="image" src="https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/b616ac19-1b92-48bb-a97e-4bebff9b7132">

Even after adding a definition to the instructions, 

<img width="769" alt="image" src="https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/96d1345b-16b7-484f-aa7e-68d0e85d4a6e">

The model was unable to answer the question correctly.

<img width="769" alt="image" src="https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/2dd99d18-aaf6-4dee-b5bd-029ea6c1bd2f">

In response to the model's failure, it gave a hint suggesting that 'customer name and id are needed'.


<img width="769" alt="image" src="https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/0f476589-e969-4635-b867-9e5df20771e0">


So I attempted to guide the prompt itself by including this information in the prompt.

And it worked!


<img width="490" alt="image" src="https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/e5d4f7eb-9c92-4139-847f-4d4accbf2d71">


**[Speculations_Impact on the design of human experiences]**

High utility in accurately answering basic data questions and brainstorming marketing/event ideas, especially beneficial for small businesses.
My speculation about this experience, Firstly, overall, it seems to be very capable of accurately answering basic data-related questions, and it's also good at brainstorming marketing and event ideas, which can be challenging for small businesses with few employees.
Offers small business owners accessible technology to compete against big enterprises.
The ability to train the model text-based without needing complex coding was awesome. It seems like an opportunity for local small business owners to easily access technology in opposition to big enterprises. 
Despite challenging training, potential for further development into a more user-friendly platform for small businesses.

Although the training process was difficult, I'd like to further develop it into a platform that small businesses can use effectively.

Model prioritizes trust by alerting potential misinformation instead of confidently presenting incorrect information.
Moreover, I found it useful and trustworthy that the model, instead of confidently listing false information, often alerts potential misinformation when there is a concern of incorrect answers.


**[Speculations_Impact on the engineering and how we build]**
- Eases understanding of diverse and complex technology and capable of contextual comprehension and targeted information retrieval.
- From the perspective of designers, as technology becomes increasingly diverse and complex, understanding it can be quite challenging. However, LLMs are highly useful as they can understand the context of questions and search for necessary information from a vast array of data. 
- Enables personalization and creativity by incorporating career and business data.
- Additionally, they allow for customization and creative tasks by inputting information about one's career and business operations, which can be greatly beneficial professionally.
Potential professional advantages.
- However, there's also a concern that the 'true self' is becoming more transparent.

**[Conclusion]**

**My Experience and Curiosities**
I previously worked as a product manager at a major Korean search engine, where I had the experience of creating and launching an LLM model. While working on design and product aspects, I created review guides for fine-tuning and designed interfaces. However, I didn't delve deeply into the operating principles or technical aspects of LLM. It's been great to have the opportunity to study these in detail through this experience.

**Key Questions and Ethical Concerns:**
- Impact of 'Always answer briefly!' instruction on model responses.
Does instruction order alter outcomes? Authority over conversation variables: instructor or user?
- Ethical concerns about models citing privacy to avoid responses of token issues. There was a part where the model claimed it couldn't answer due to privacy concerns because of a token issue, which I'm worried might be ethically akin to lying.
- For small businesses, data security is a significant concern. There is doubt whether LLMs, when fed with personal data, can ensure the safety of this data. Small businesses are often more vulnerable to data breaches, raising concerns about the potential misuse or leakage of sensitive information processed by LLMs.
- When I used the LLM, I noticed that it sometimes suggests what additional data could make its responses more accurate, acknowledging its limitations to some extent. However, there are instances where it confidently provides incorrect answers. For example, it once misinterpreted a security issue as a token issue. As business owners use LLMs more frequently, their trust in the model's reliability increases. This trust can be problematic if they rely on an incorrect response, potentially causing significant harm to their business and even their personal lives. Given that LLMs can influence not just minor tasks but also major business decisions, it's crucial not to approach them purely from a business or marketing perspective. SMEs should be made fully aware of the model's potential inaccuracies, and it is advisable to use the LLM with extensive verification. Educational videos about LLMs or examples of incorrect responses encountered during use could naturally inform users about these inaccuracies.
- On the other hand, there is a concern about the stability of trustworthiness of these systems. The trust built between a business owner and an LLM can be shattered by a single mistake, highlighting the need for robust and reliable systems. It's important to address these stability concerns to maintain the confidence of SMEs in using these technologies. Regular updates and improvements to the LLM, along with transparent communication about its limitations and best practices for its use, could help mitigate these risks.
While LLMs offer significant advantages for small businesses, it's crucial to approach their use with an understanding of their limitations, especially in terms of data security and accuracy. Ensuring that SMEs are well-informed about these aspects and using the LLMs cautiously and responsibly is key to leveraging their benefits without exposing the business to unnecessary risks.

**Feedback:**
I didn't have the opportunity to play my video in the TDF class, so I showed my demo to a few of my friends (4 people) and also presented it in the Equitable Design class. (I won the 2nd prize in the class for the idea!)
Those who gave feedback generally had experience using ChatGPT, but it was their first time using a model that had been personally trained with additional learning, so they found it fascinating. It was interesting that everyone commonly asked about the most personally relevant uses they could think of, such as using it in their current research or getting help with writing their thesis paper.
The first area for improvement was the interface. Since the feedback was based on the Zerowidth demo model, it was noted that it felt too bland, like a regular ChatGPT. If it were to be used for a customer-facing chatbot, it was suggested that designing an interface that reflects the unique personality of a small business would be beneficial.
There were also comments about the speed. It seems that if you ask a slightly difficult question, the LLM responds too slowly, which might frustrate or inconvenience customers. Therefore, it was suggested to focus more on developing the platform for the purposes of Small and Medium-sized Enterprises (SMEs), rather than focusing on customer-facing interactions.
Concerns were also raised about the learning process. Although I did not take significantly long to learn how to use it, if it is to be used by SMEs, it needs to be more user-friendly, and there were worries about how to simplify the process of structuring and training with more complex data. If this is to be realized, it seems necessary to think deeply about the learning materials, interface, and use flow that can be offered to SMEs who might be less tech-savvy.

**Conclusion:**
 Reflecting on my "LLM for Equitable Design" project, I've gained insights into the potential and challenges of using LLMs for small businesses. The experience was a blend of technical exploration and ethical considerations, emphasizing the importance of balancing innovation with responsibility. Key takeaways include the adaptability and effectiveness of LLMs in data management and customer interactions, coupled with a heightened awareness of ethical concerns like data security and accuracy. Feedback from people highlighted areas for improvement and further exploration. It bolstered my understanding of AI's potential in business but also reinforced my commitment to responsible and equitable technology use. 

**Video Link:** https://youtu.be/GPyqpCLSO6E?feature=shared



# [Week of 11/2/2023] LLM #1

I previously worked as a product manager at a major Korean search engine, where I had the experience of creating and launching an LLM model. While working on design and product aspects, I created review guides for fine-tuning and designed interfaces. However, I didn't delve deeply into the operating principles or technical aspects of LLM. It's been great to have the opportunity to study these in detail through this experience.

I reviewed the video of Peter lecture on Youtube. It was truly insightful! 

Here are some notes: 

**Large language models (LLM)** are very large deep learning models that are pre-trained on vast amounts of data. The underlying transformer is a set of neural networks that consist of an encoder and a decoder with self-attention capabilities. The encoder and decoder extract meanings from a sequence of text and understand the relationships between words and phrases in it.

Transformer LLMs are capable of unsupervised training, although a more precise explanation is that transformers perform self-learning. It is through this process that transformers learn to understand basic grammar, languages, and knowledge.

Unlike earlier recurrent neural networks (RNN) that sequentially process inputs, transformers process entire sequences in parallel. This allows the data scientists to use GPUs for training transformer-based LLMs, significantly reducing the training time.

**Why are large language models important?**

Large language models are incredibly flexible. One model can perform completely different tasks such as answering questions, summarizing documents, translating languages and completing sentences. LLMs have the potential to disrupt content creation and the way people use search engines and virtual assistants.

While not perfect, LLMs are demonstrating a remarkable ability to make predictions based on a relatively small number of prompts or inputs. LLMs can be used for generative AI (artificial intelligence) to produce content based on input prompts in human language.

LLMs are big, very big. They can consider billions of parameters and have many possible uses. Here are some examples:

Open AI's GPT-3 model has 175 billion parameters. Its cousin, ChatGPT, can identify patterns from data and generate natural and readable output. While we don’t know the size of Claude 2, it can take inputs up to 100K tokens in each prompt, which means it can work over hundreds of pages of technical documentation or even an entire book.
AI21 Labs’ Jurassic-1 model has 178 billion parameters and a token vocabulary of 250,000-word parts and similar conversational capabilities.
Cohere’s Command model has similar capabilities and can work in more than 100 different languages.
LightOn's Paradigm offers foundation models with claimed capabilities that exceed those of GPT-3. All these LLMs come with APIs that allow developers to create unique generative AI applications.


**What are applications of large language models?**

There are many practical applications for LLMs.

**Copywriting**

Apart from GPT-3 and ChatGPT, Claude, Llama 2, Cohere Command, and Jurassiccan write original copy. AI21 Wordspice suggests changes to original sentences to improve style and voice.

**Knowledge base answering**

Often referred to as knowledge-intensive natural language processing (KI-NLP), the technique refers to LLMs that can answer specific questions from information help in digital archives. An example is the ability of AI21 Studio playground to answer general knowledge questions.

**Text classification**

Using clustering, LLMs can classify text with similar meanings or sentiments. Uses include measuring customer sentiment, determining the relationship between texts, and document search.

**Code generation**

LLM are proficient in code generation from natural language prompts. Examples include Amazon CodeWhisperer and Open AI's codex used in GitHub Copilot, which can code in Python, JavaScript, Ruby and several other programming languages. Other coding applications include creating SQL queries, writing shell commands and website design.

**Text generation**

Similar to code generation, text generation can complete incomplete sentences, write product documentation or, like Alexa Create, write a short children's story.

**How are large language models trained?** 

Transformer-based neural networks are very large. These networks contain multiple nodes and layers. Each node in a layer has connections to all nodes in the subsequent layer, each of which has a weight and a bias. Weights and biases along with embeddings are known as model parameters. Large transformer-based neural networks can have billions and billions of parameters. The size of the model is generally determined by an empirical relationship between the model size, the number of parameters, and the size of the training data.

Training is performed using a large corpus of high-quality data. During training, the model iteratively adjusts parameter values until the model correctly predicts the next token from an the previous squence of input tokens. It does this through self-learning techniques which teach the model to adjust parameters to maximize the likelihood of the next tokens in the training examples.

Once trained, LLMs can be readily adapted to perform multiple tasks using relatively small sets of supervised data, a process known as fine tuning.

Three common learning models exist:

- Zero-shot learning; Base LLMs can respond to a broad range of requests without explicit training, often through prompts, although answer accuracy varies.

- Few-shot learning: By providing a few relevant training examples, base model performance significantly improves in that specific area.

- Fine-tuning: This is an extension of few-shot learning in that data scientists train a base model to adjust its parameters with additional data relevant to the specific application.


**This week reflection**
When I couldn't attend class due to personal reasons, I asked for help from Yunting and Katherine and requested class recordings from the professors. I was truly grateful for the supportive attitude of these friends who understood my situation and helped me stay on track with the class content.

Although I couldn't participate in the class, I carefully reviewed the recordings and studied on my own. I also researched information about LLM and organized it on GitHub. Since I had experience participating in LLM interface design and dataset refinement, I was able to get involved with enthusiasm.


# [Week of 10/26/2023] Demo week
This week was a demo week where we could see the work of different friends. It was enjoyable to see the unique characteristics of each group, from friends who focused on mechanics to those who tackled challenging coding, and those who stood out with outstanding ideas.

I think I had a decent understanding of the parts I wasn't directly responsible for, and I was able to respond well when friends came to ask questions during the demo day. Additionally, when I went to see the projects of other teams, I was grateful that everyone kindly explained what technologies they used. One thing I wish I had done better is keeping more thorough documentation or archiving.

![IMG_9530](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/c276f5c0-b9d7-4307-90a4-fe53fdab37ed)

![IMG_9531](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/42d6cd4d-8304-4ead-aa3e-fb7e138c1b2f)

![IMG_9532](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/1c410f31-a917-46e8-bfd9-325b0b384f22)

I am personally also studying meditation. Since mental health is emerging as an extremely important issue for modern people, I believe that our project can play an essential role for contemporary society. Wouldn’t it be amazing to end a busy day by looking at this flower and steadying your breath?

If we could further develop our project from an engineering perspective, we might be able to (1) make the flower move more smoothly for a better experience, (2) change the graphics to be more immersive for meditation, and possibly add narration or music, (3) make the wearable more ergonomic, and (4) improve the experience to be more integrated with the actual body by using real breathing as input for intervals.

Considering the integration with AI, since the breathing intervals vary from person to person, we could potentially learn the individual’s breathing patterns and adjust the content accordingly. Alternatively, we could provide meditation content suitable for the user's current situation through text input. Furthermore, through image generation, we might be able to project various images onto the flower that match the ambiance.

Concluding this report on the project, I can confidently say that the journey has been both challenging and enlightening. Inspired initially by my admiration for Studio Drift, this project turned into a collaborative effort, bringing together many talented friends to implement various technical aspects, which was really satisfying for me.

Throughout the project, we faced several challenges in role distribution and communication among team members. However, the open discussions we had post-project, where we shared our feelings and provided feedback on our team dynamics, proved to be incredibly beneficial. These reflections have taught me valuable lessons on the importance of teamwork and communication in achieving our goals. Reflecting on the dynamics of our team, it's clear that while individual contributions were valuable, a more integrated approach to teamwork would have greatly benefited our project. This realization is crucial for my future work, where fostering a collaborative environment, clear role set, and transparent communication can enhance both the process and the outcome.

The focus of our project was to create a wristband that was not only functional but also aesthetically pleasing, integrating elements with a mechanical flower. This blend of technology and design presented numerous learning opportunities, especially through overcoming material flexibility issues, power limitations, and finding the right design specifications. Through the iterative design process, from conceptualization to the final product, I learned the importance of persistence and adaptability in the field of technology design.

Looking ahead, I believe our project holds immense potential, particularly in the realms of mental health and meditation. My ambition is to further develop the project to make the flower move more smoothly, enhance the graphics for meditation, and improve the ergonomic design of the wearable. Integrating AI to personalize the experience based on individual breathing patterns or to provide context-specific meditation content could significantly enhance how we interact with technology for mental wellness.


# [Week of 10/17/2023] Proton2 #5

Wristband

🤖Mechanical
A simple wristband can be done through laser cutting plywood and bend it in shape: living hinge template

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/e3f705c8-ee76-419c-8ec2-d5925dc240b6)

(initial reference image)

I started drawing to prepare for laser cutting the wearable structure. Previously, I looked up the reference by searching for 'hinge pattern laser cutting.'


For the production of the bracelet, considerations had to be made for the appropriate length on the wrist, the thickness of the hinge pattern lines, the incorporation of a vibration sensor, and the method of connection. 

First, considering that the material was wood, we tested the thickness of the hinge pattern to ensure it wouldn't break. After making several sketches with slight variations and printing them multiple times, we found the right thickness that wouldn't break and would bend well to match the wrist's thickness. The overall length of the wristband was initially too long in the first attempt and required adjustments.

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/8e7c8c9d-26b3-41d1-bfb0-ec6e76e5760f)

(Broken part)

During laser cutting, it was important to set the intensity correctly to ensure clean cutting in one go. Even when considering the material thickness, there were times when it was necessary to overlap with the existing cutting line and cut it again for proper results.

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/43e7502b-8505-40fe-8f88-c1a14aef415b)

(Iterations)

Initially, we planned to connect the parts by fitting them into holes, but due to the wood's flexibility, it was not feasible. Therefore, after discussions with team members, we decided to use Velcro for the connection.

(To be continued… We didn’t applied it yet)

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/cca388a0-95be-4bf9-a2cc-31a2849255f3)

(Final one)

For the machanical flower part, we cut the flower petals and stacked them together.

![fetal](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/0e7c8dd7-0bd6-4d3a-baf7-93fbd6e219e7)

And we tried to build the basic frame for fetal connecting, but it was really hard to put them together since it is not a flexibel material.

![yuhe working on frame](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/6ce2601e-f583-475e-b930-9ffde4163e76)

![working for frame](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/4a2968d5-8eb8-463a-aa1e-60dc6044ccbf)

Also we had to make the right size for servo motore to fit in, we printed again for the second trial.
After few brokes, we succeed to stick together with super glue at the end.
![fetal frame_2](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/86bfba00-cb71-4bf0-bdc1-49954471aeb3)


Now, we had to connect the fetal. First, we tried to use the bended wire for the ring, but it wasn't really working  
![trial1_fetal](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/7ce0ed99-ad0f-4875-9b56-e184cce3bbed)

So We got a cable tie for that, and it worked like this.



https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/858c6d55-d7d0-4482-ad70-651e850349eb

We had a power issue that the fetal can't move only with servo motor's power, so we had to maually move with it.

(This week reflection)

Each of us remained faithful to our roles and performed our assigned tasks exceptionally well. Despite facing challenging tasks, we frequently sought guidance from instructors and persevered until we solved difficult problems. Observing this, I found a lot of motivation for myself as well. 
However, it was a bit sad that due to the busyness of dividing and conquering our tasks, we didn't have many opportunities to come together as a team. The lack of time for collective discussions made it feel more like individual contributions rather than true teamwork. In the future, I hope we can have more time and opportunities for the team to work together.


 Although we divided the team to work on tasks, some team members preferred working alone, and in trying to accommodate these preferences, I believe I struggled to find my role effectively. As a member of the mechanical parts team, I participated in the research stage of designing the mechanism, conceptualizing it, making decisions, and contributing to modeling and frame building. However, I felt that there was limited satisfaction in solving challenging problems on my own.

 In the future, I've learned the lesson that when working with a larger team, we should set ambitious goals or tasks that involve more challenges, or we should allocate roles more effectively during the decision-making phase.
 

# [Week of 10/12/2023] Proton2 #4

We devided task for working seperately. 

- Electrical Connection Group
- Group for connecting multiple photons to make them work
- Coding Group
- Group researching the mechanics of flowers

I belong to the group researching the mechanics of flowers, so I discussed the design process with Nancy before she started 3D modeling. Nancy thought it would be more convenient for her to do the modeling on her own, so I started drawing to prepare for laser cutting the wearable structure later.


Previously, I saw some friends cutting a mesh pattern and asked Kirk about it. He informed me that I could obtain the desired pattern file by searching for 'hinge pattern laser cutting.'

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/8df7561e-8ca4-4145-a245-0c8a03a80641)


I have completed the sketch below. I will need to make some modifications after measuring the wearable device.

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/dbd47bbf-c697-44fc-aaa2-bf9bf6797aff)


We did some initial movement test here from the reference before, and it worked well!

https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/8abcfc70-a3e6-44c5-bddc-136c17c87dc4



# [Week of 10/05/2023] Proton2 #3
TDF Mindful Meditation Bloom 

(Project Overview)
Meditation Bloom aims to amalgamate technology, aesthetic, and mindfulness, crafting a transformative physical and mental experience. It is a meditation-assistive device that provides a multi-sensory experience by integrating visual, tactile, and audial cues, thus enhancing the user's focus and immersion during the meditation process.

(Components)
1. Meditation Flower:
Function: 
Opens and closes in synchronization with the prescribed meditation breathing pattern.

Design: 
Resembling a delicate flower that blooms and retreats, providing a visually calming and metaphorically rich imagery.

Technology:
Utilizes mechanical petals that are controlled by a microcontroller, ensuring smooth and synchronized movement.

Lighting:
Subtle and adjustable lighting that complements meditation moods and provides ambience.

2. Wristband
Function: 
Vibrates subtly, aligning with the meditation breathing pace and providing tactile feedback for breathing synchronization.

Design: 
Ergonomic, lightweight, and non-intrusive, ensuring comfort and aesthetic appeal.

Technology:
Employs a precision haptic motor which can adjust vibration intensity and pattern, to avoid startling the user and to align accurately with the meditation rhythm.
Target Audience
Primary:
Individuals seeking innovative and immersive meditation experiences.

Secondary:
Wellness centers, therapists, and yoga studios that could utilize the device to enhance their service offering.
User Interaction
The user initiates a meditation session via a mobile application, selecting or customizing their breathing pattern and pace.
The Meditation Flower responds by opening and closing in tandem with the selected breathing pattern, while simultaneously illuminating to establish a serene environment.
The wristband vibrates in sync with the pattern, providing tactile cues to assist the user in maintaining the prescribed breathing rhythm.

(Objectives)
Enhance the user’s meditation experience through multi-sensory engagement.
Provide a visually pleasing apparatus that doubles as a decorative piece when not in use.
Facilitate consistent and focused meditation through synchronized cues.

(Key Features)
1. Breathing Flower:
The Meditation Flower is able to close and open up based on selected meditation patterns with a built-in lighting that is capable of changing colors according to the user’s selection.

2. Vibrating Wristband:
The wristband vibrates subtly on the user’s wristband according to the selected meditation patterns.

3. Synchronization:
Ensures that visual and tactile cues are precisely synchronized with the selected meditation pattern.

4. User Customization:
Allows the user to select and customize breathing patterns, vibration intensity, and light intensity.

5. App Integration: 
(Might now able to realize in this round of iteration, but is open up to further development)
Enables the user to control, customize, and track their meditation sessions via a dedicated app.

6. Design Specification

(Technological Challenges):
A smooth mechanism for the Meditation Bloom to open and close up.
Robust and quiet motor for the Meditation Bloom to ensure non-disruptive drive of the mechanical part.
A reliable communication protocol between the Meditation Flower, wristband, and app, ensuring synchronized operation.
High-precision haptic technology in the wristband for subtle and accurate vibrations.
Energy-efficient LED technology for the Meditation Flower, ensuring sustainable operation and longevity.

Mechanical Flower
Brainstorming of forms
2D Flower

3D Flower

Geek's Valentine's day: Everblooming Mechanical Flower Garden

Ball-shaped flower
Something similar to the Hoberman sphere:
https://www.youtube.com/watch?v=-DsHk_iR_xU

Pendant flower (Like a pendant light)


Circuits & Code


In terms of the coding, we plan to rely on the rotating servo motor to control the mechanical parts to mimic the flower opening and closing.

(Wristband)

🦾Mechanical
A simple wristband can be done through laser cutting plywood and bend it in shape:


Circuits & Code
For the wristband, it has a vibrator motor built inside for vibration guiding on the wrist. The vibration pace will be in sync with the motion of the flower, working as a secondary guide device for meditation.

The circuit (and code) of the wristband is quite straightforward: by connecting vibrator motor to photon 2 and set the pace to link to the meditation pace. For the code, we can build a front-end web page that has several buttons on it. By controlling the buttons users will be able to test, begin or end the vibration.


We did a little test of the vibrator motor and it worked like this:




# [Week of 09/28/2023] Proton2 #2

This week, we gained insight into using Proton2 by making an LED work. Additionally, we conducted a brainstorming session for ideas for our team project 2. It was a very smooth and enjoyable environment for brainstorming because there weren't many constraints other than time limits, and all our group mates were very open and supportive of the ideas we brought to the table. After gathering all the ideas, I had a hard time selecting only three of them because every idea sounded exciting. It was a pleasure to see all these interesting ideas, making me look forward to our next project!

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/0bb3c259-96d4-46ad-9857-b2f92f970533)


Also, we had a chance to listen Adrian Freed's(http://www.adrianfreed.com/, Research Director of UC Berkeley's Center for New Music and Audio Technologies) lecture. He showed many examples of electrical textiles could be used in wearable devices. It was so interesting!

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/e4c1ff83-310c-4d81-b24f-0c7ba1e64747)


![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/715694c6-35a6-459f-a162-0d099e3b0c8b)


![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/00c7a1a1-9c2f-435a-b532-bb3b2334a52a)


![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/dd72db09-708f-4de2-94d4-2b90a3e6f2d9)


![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/aaf0e047-587d-428b-bfc8-0e7a44bcea14)



I assisted my classmates during the class based on my understanding of Arduino from my past experiences. I helped with tasks like uploading code to the microcontroller and understanding the polarity of the LED/.... I hope to have more opportunities to help my classmates as time goes on. During the brainstorming session, I contributed numerous interesting ideas. Additionally, I made sure to listen carefully to others' ideas and incorporate my own to make them clearer and more feasible.


# [Week of 09/21/2023] Proton2 #1

We'll start to play with proton! 

I tried to do the wifi connection at home, but Particle couldn't find the network. 

I tried to solve the problem but I couldn't at the end... 

I will organize the process anyway!


1. Update the particle device
![화면 캡처 2023-09-21 082532](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/75b90e94-4192-4017-b5d7-ab358434a15a)

2. Create my device
![화면 캡처 2023-09-21 082702](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/a86fcf5a-c245-4da1-a5d7-6a4c0fc7e36f)

3. Give a name! 
![화면 캡처 2023-09-21 082721](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/f70a8e3a-0c02-4251-b8fa-570cf5aa4f35)

4. Tried to get wifi at home but it didn't work.... and I tried from process1 but it showed like this
![화면 캡처 2023-09-21 091136](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/5f5a1fe2-56bf-4d1e-bca9-ba4fc3b349a8)


I need to take time work more on this. I think I should find another network from visiting my friends home.


# [Week of 09/14/2023] Computational Design #3

Video Submission day! 
I have every progress for this week in this video : 
https://youtu.be/qrvmXjAUm_U


# [Week of 09/07/2023] Computational Design #2
**Good things about Grasshopper**

Common 3D modeling programs, including Rhino, work in a clear-cut beginning-to-end fashion, like drawing guidelines, then points, then lines, and finally creating faces. Therefore, it is difficult to go back to that point in time and make corrections in the case of past work that has already passed to some extent(even if there are some differences between programs). Therefore, perfect design must precede 3D modeling, and inevitably, if the design is changed during 3D modeling, the work process that has been carried out so far must be discarded and returned to a point in time a long time ago.

This exposes the weaknesses of common 3D modeling programs in two respects. First, since all of the previous work is invalidated, the work time increases exponentially whenever the design is changed during the 3D modeling process. Second, although the design can be improved in the process of concretely expressing what was in the imagination or sketch through 3D modeling, creative thinking to seek a better design is completely abandoned during 3D modeling due to the above reasons.

However, in Grasshopper, **all individual tasks are done through components**, and the whole task is carried out in a way that connects the components together. It is exactly the same method as the algorithm learned in math class in school. Here, all the components from the first utilized component to the last component of the work remain connected to each other on the land called the canvas. Therefore, in Grasshopper, unlike the other programs described above, it is possible to modify the work at any point in the past at any time.

With this, Grasshopper perfectly overcomes the two weaknesses of common 3D modeling programs described above.

**First, during the process of 3D modeling, the design can be changed at any time by manipulating past components that have already passed, so even if the design is changed, the working time does not increase at all.** If you are only changing the numerical value of a component, it only takes 1-2 seconds. Even if the design is drastically changed, the work time is not increased due to things unrelated to the change work because only the parts that need modification can be cut and replaced with new components.

**Second, creative thoughts can be made at any time to improve the design while doing 3D modeling, and it can be easily reflected in the design since the work efficiency according to design change is very high.** In addition, even if only the numerical value of a specific component is changed in various ways, various variations with the same design identity can be created. Furthermore, it is possible to create a new design that simultaneously contains the identity of the two designs by well connecting the components that make up the two unrelated designs.

This week, I explored Grasshopper that I didn't really know how to use.

**Components**

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/426d6b0a-893c-4751-91ee-ac8d08e5ba4a)

When a component is selected by left-clicking, the component turns green and is activated in the Grasshopper.

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/abd3a606-2c6b-4e85-9a4c-04f67a6aa3ee)

You can know the current state through the component color.
- light gray: works fine
- Dark gray: Component preview OFF state
- Orange: Components with minor issues, issues need to be identified and resolved
- Red: A component with a big problem, it is highly likely that an incorrect value was entered.

**Wire**

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/006243be-99e9-4806-acfc-1a70ffcf1818)

The data structure can be inferred by looking at the shape of the wire.
- 1 item in 1 branch: single line
- 2 or more items in 1 branch: double line
- Two or more branches: dotted line

  ![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/bd731c37-5321-4061-b34e-be9c82cf7896)

To break a connected wire, hold down ctrl while dragging.

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/98f50127-3013-4b7a-8abc-2320b5e6ab4e)

If you want to connect two or more wires at one place, hold down the shift key while dragging.

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/0288f753-e9f9-4a40-9283-e3ea2fed5cc6)

If you want to move two or more wires to different places at once, drag them while pressing Ctrl+Shift at the same time.

**Set&Bake**

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/328f5654-f76a-4664-bb80-83167d7eaea8)

The meaning of Set is to bring information from Rhino to the Grass Hopper. To set, after creating the information to be set and appropriate components in Grasshopper, select the information to be set in Rhino, right-click and press the set button. Set One is used to enter one piece of information, and Set Multiple is used to enter multiple pieces of information.


![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/f5796cbb-6cc2-4136-9afa-704cf3cd976e)

Bake, on the other hand, is used when exporting from Grasshopper to Rhino. Before Bake, the form seen in the Rhino window is just a preview before it is implemented in Rhino, literally a preview, and information is actually output only when Bake is performed. For Bake, select the component to export, open the radial menu, and select the fried egg shape at the bottom right.

**Radial menu**
To open the radial menu, use Ctrl + Space bar or middle mouse wheel click.

- Disable/Enable Preview: Disable/enable preview, Ctrl+Q is convenient.
- Group: Grouping creates a background color, which is good for highlighting or distinguishing algorithms. If you right-click the background color part and enter text in the empty space at the top, you can also set the name you want. You can also -change several properties or change the background color.
- Cluster: A cluster is a function that organizes repeated parts or overly complicated algorithms to express algorithms more clearly.
- Preferences: The Grasshopper settings window appears.
- Navigate: similar to the game's minimap
- Disable/Enable: Disable/enable component
- Zoom: Similar to Rhino's zoom_selected function, fills the Rhino window with the part corresponding to the component selected in Grasshopper to find it.


# [Week of 08/31/2023] Computational Design #1
I learned how to use Rhino, at first, it was also difficult to get a grip on the four quadrants on the Rhino's screen.

**WHY I can only see the circle in the middle?**

When I first opened Rhino, I was surprised as I saw only a simple circle drawn. 
With the help of design specialist, I typed 'grasshopper' in the command prompt to open the Grasshopper program. Upon pressing the green button, all the objects became visible. According to the design specialist, it's common to keep the green button off and choose to drag and view only the parts you need in Grasshopper.

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/6ae8f7de-611e-46e0-8bab-dccc261781ea)

The parts that appear as orange lines in Grasshopper don't have any effect on the code, design specialist said. So, it's good to group and disable them using Ctrl+G. By going through this disabling process, the program becomes lighter and rendering speeds up. In Cody's case, he had designed the train system for Anaheim. If he turned on all interactions at once in Grasshopper, it would cause a system crash.

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/174e1765-61c1-4ea1-b527-c9ea29bbb770)


As I explored the Grasshopper program, it's considered a tool for parametric modeling and relationship design. The aspect that stood out to me was the ability to visualize the code, allowing you to see the relationships between objects at a glance.


**Command function**
- Since there are too many icons and functions in the program, it's convenient to use "Command" function like this.
![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/6c751f0b-4a0e-49b3-88e4-ebc7091ff079)

I used more commands below.
- 4View (only for perspective view, 'wireframe' for others)
- _Group(or Ctrl+G)
- Grasshopper(to open Grasshopper)
- etc...

**Customizing Phonestand to my phone**
1) Measuring
I need to consider the phonecase sizes as well. It was --> H * W * T = 150 * 75 * 12

*"Well...While taking pictures of the process of measuring the phone size with an iPad, I felt once again that I needed a phonestand!"*

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/d4b9ce03-f009-4048-87c4-4015cc0f9ad1)
![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/bef15227-1e0d-497c-8bd4-d5670c5fbed3)
![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/2f1ece46-c557-4a4c-8807-284da8a936e8)

3) Adjusting Phone Size
![phone size](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/befff3fe-b485-431c-bf37-f68b12968135)

4) Adjusting Student Activity Range and Height 
![1100_1187](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/e7ee61c2-c485-4f4f-8a69-4f633b9790f1)
![height](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/e000db09-ff4a-4a5c-8126-063ec8fdb8c0)

**Bake**
- To make it as a 2D model and to select for export, I should 'bake' it in Grasshopper.

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/5bb61273-1bd1-4723-9375-ccb4f9ff0cfe)


**Placing objects**
- Set Layer and color code it. When you export, it will automatically be red and easy to adjust for cutting.

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/4180ee33-464c-40d4-bf11-ad06722d0b2c)

- The pieces were placed out of the board, so I used "move to 0" so that it is visible in the illustrator.
  
![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/f50213e8-9f14-40c6-9779-8feddc2b3f64)

- The grid didn't show up, so typed "Grid" and changed "ShowGridAxes=Yes", "ShowGrid=Yes"
- It's Cody's little tips! His favorite settings are like this, and it is convenient to use! 'Onsnap' makes it easier to draw lines.

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/8bbd3a19-0737-411e-930c-bd7ca3a847a7)

**Export**

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/e37fbe4f-fe9b-436f-a574-95a1455404cc)

**Illustrator**

- Document settings : 32 * 18 inches (our laser cutter's size)
  
![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/904ce791-5629-4537-a4de-2825781d86a3)

- Turn on the [View > CPU preview] to make missing lines visible


**Settings for Laser cutting**
- It is helpful to check which area is available to reuse material. (click "Focusview" and set where do you want to set the laser.)

  ![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/92ca893f-f58b-477f-a1a4-3e2ff6f01820)
![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/6cbd9f19-6633-41f3-b2b7-0f1313793466)

- I changed my design's location a little bit to adjust with the reuse material.

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/be58a5ce-9b4d-4222-a0a9-a77bb7a623da)

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/7f22c7a1-a01f-4e58-ae9f-c8b9363e0c0a)

- Material setting

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/11ea8a9a-26ff-4f4a-b741-347e85847e13)

- This is the setting for intensity. I could set like this, and it's better to check with fingers after cutting to see if it is well cut.

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/ff57d999-edf2-415a-9217-f4ebe34ad9ed)

- Line thickness should be 0.001pt, and Blue and Black line has different function. Blue will just follow lines and engrave it, black will engrave all along the lines and the surface inside.

**Preparation!**
- I turned on the laser exhaust switch, checked if air flows, and turned on the compressed air switch!
![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/08b02eee-531a-4817-88a0-61265b735bf8)

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/4938e296-7405-4050-ab9a-983de82ae628)

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/16fa1790-0aad-447b-8447-991e50d23c2d)

- I found this sign later, I was almost playing around but I realized that I shouldn't have done that.
![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/75b36ee4-c161-4b66-b7c5-b65273f3734b)


**Results**

Succeed! But I want it to be more study. I thought it would be better to adjust the hole size or add a few more slots to make it fit a bit more snugly. Also there were too much soot in the wood!!!

![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/4cc3e614-81b7-45db-8c80-5c65e48772f8)
![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/b3659a51-d768-4d0c-9657-be46945dc458)
![image](https://github.com/Berkeley-MDes/tdf-fa23-hye-jade/assets/143137119/feb05ed8-3685-40e6-9f1f-f1ec0b99df17)



**In this writing, reflect thoughtfully on your personal performance since last week. Did you take an opportunity to help out a classmate?  Were you able to meet your personal expectations?  What helped or hindered your performance?  Use full sentences.**

During my undergraduate years, I had the opportunity to briefly experience using laser cutting and Rhino. I thought it wouldn't be too difficult, but it turned out to be more challenging than I anticipated. (I faced difficulties from the moment I opened the Rhino program.) Rather than meeting my personal expectations, my proficiency with Rhino was still quite low, which was disappointing. However, I plan to look for tutorials and put in more effort to improve in the future.

What truly helped with my progress was the assistance of the design specialist. When I visited the makers space in a somewhat urgent situation, the design specialist patiently guided me in a way that was easy to understand, enabling me to complete the task. I regret not seeking help earlier and I've realized the importance of being more proactive in asking questions and seeking advice in the future.

One positive aspect I want to highlight about my achievements is that I diligently documented the usage and settings of Rhino, Grasshopper, and laser cutting techniques through photos and notes, so that I can remember them when using them in the future. Additionally, I find it enjoyable to explore GitHub, which I'm using for the first time. While I started the assignment a bit late and didn't have the chance to 'physically' assist my classmates, I was glad to help a few friends with things like finding information about laser cutting reservations or setting up GitHub repositories.

**In this writing, reflect thoughtfully on your cohort's performance since the week.  Was there anything that surprised you? Are you grateful for assistance from a classmate? Is there anything that you can contribute that would improve the experience? Use full sentences.**

 Actually when I first opened Rhino, I only saw a simple circle and couldn't see any objects. Like this, I found it difficult to follow the assignment instructions, as there were no specific solutions provided. Also, I had to search for information from various sources like the wiki, GitHub, bcourse, Google Drive, and more, which made the task challenging. I was impressed by how everyone seemed to easily find the necessary information and complete the assignment.
 
 It was also nice to see how people were reusing materials effectively even if no one told to do that. Furthermore, when I mentioned that I was having trouble finding time for laser cutting, a friend offered to split their reserved time with me. (In the end, I managed to make a reservation myself.) 
 
 It would be great if we have a clear outline of exactly what tasks need to be done by the deadline.(Maybe I could do that!) Also, I hope I can help friends around me and contribute to their learning after becoming more familiar with the software.

