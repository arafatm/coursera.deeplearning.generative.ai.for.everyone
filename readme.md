# [Coursera DeepLearning.ai: Generative AI for Everyone](https://www.coursera.org/learn/generative-ai-for-everyone/home/week/1)

[Generative AI for Everyone: Lecture Notes](https://community.deeplearning.ai/t/generative-ai-for-everyone-lecture-notes/481740)

## Introduction to Generative AI

### What is Generative AI

![](/img/1.04.jpg) 

AI is already pervasive in our lives and many of us use it dozens of times a
day or more without even thinking about it. e.g. Every time you do a web search
on Google or Bing, that's AI.

But many AI systems have been complex and expensive to build, and generative AI
is making many AI applications much easier to build.

![](/img/1.11.jpg)

### How Generative AI works

![](/img/1.13.jpg)
- supervised learning, which turns out to be really good at labeling things.
- supervised learning and generative AI, are the two most important tools in AI today.

![](/img/1.15.jpg)
- Supervised learning is the technology that has made computers very good when
- given an input, which I'm going to call A, to generate a corresponding output, which I'm going to call B.

![](/img/1.16.jpg)
- But what we found starting around 2010 was that for a lot of applications, we
  had a lot of data, but even as we fed it more data, its performance wasn't
  getting that much better if we were training small AI models.
- This means, for example, if you were building a speech recognition system,
  even as your AI listened to tens of thousands or hundreds of thousands of
  hours of data, that's a lot of data, it didn't get that much more accurate
  compared to a system that listened to only a smaller amount of audio data.
- But what more and more researchers started to realize through this period is
  if you were to train a very large AI model, meaning an AI model on very fast,
  very powerful computers with a lot of memory, then its performance as you fed
  it more and more data will just keep on getting better and better.

![](/img/1.18.jpg)
- It uses supervised learning to repeatedly predict what is the next word.
- But at the heart of LLMs is this technology that's learned from a lot of data
  to predict what is the next word.

### LLMs as a thought partner

![](/img/1.20.jpg)

![](/img/1.21.jpg)

![](/img/1.22.jpg)
- given the propensity of LLM's to make things up and sometimes sound very
  authoritative and confident when making things up, I would probably want to
  double check anything it says about healthcare or medicine before following
  the suggestions.

### AI is a general purpose technology

![](/img/1.26.jpg)

![](/img/1.27.jpg)

## 1.2 Generative AI Application

### Writing

![](/img/1.28.png)
- Output quality increases with context and specificity provided

![](/img/1.29.png)
- e.g. in this translation it's not as good as native speaker
- "front desk" translated literally vs "reception"
- providing promt of "formal spoken hindi" improves the translation

### Reading

Can be used for e.g. 
- proofreading
- summarizing text
- summarizing conversations
- automating tasks
- reputation monitoring

![](/img/1.30.png)
![](/img/1.31.png)
![](/img/1.32.png)
![](/img/1.35.png)

When building your own app, be very specific
![](/img/1.33.png)
![](/img/1.34.png)

### Chatting

Can build specialized chatbots e.g. travel specific
![](/img/1.36.png)

### What LLMs can and cannot do

Mental framework for LLM, can a fresh college grad perform the task...
![](/img/1.37.png)
![](/img/1.38.png)
![](/img/1.39.png)

Assume:
- no access to internet nor external resources
- no training specific on your company/business
- no memory of previous task completed

Other limitation:
- knowledge cutoffs: 
  - last time it 'scraped' the internet e.g. what is highest grossing film of <this year>
  - learns erroneous information from "common" wrong information e.g. temperature of superconducter LK-99 
- Hallucinations: will sometimes make up information in an authorative voice
- input and output length is limited e.g. trying to summarize a very long paper
- Does not work well with structured data 
  - e.g. given table of home prices, estimate median price
  - in this case can use supervised learning instead
- Works best with unstructured data
- Has bias and toxicity learned from the internet
![](/img/1.40.png)

### Tips for prompting

- Be detailed and specific
- Guide the model to think through its answer
- Experiment and iterate

![](/img/1.41.png)
![](/img/1.42.png)
![](/img/1.43.png)
![](/img/1.44.png)

### Image generation (optional)

__Diffusion Models__ have learned from huge numbers of images. This is an example of supervised learning.

![](/img/1.45.png)
- Learn to generate slightly less noisy image from noisy image at every step
- This takes lots of steps

## 1.3 Week 1 resources

### Web UI chatbots to try

If you'd like to experiment with prompting a large language model (LLM), you
can visit one of the chatbots linked below:
- [ChatGPTOpens in a new tab](https://chat.openai.com/) from OpenAI
- [BardOpens in a new tab](https://bard.google.com/chat) from Google
- [Bing ChatOpens in a new tab](https://www.bing.com/search?q=Bing+AI&showconv=1&FORM=hpcodx) from Microsoft
    
### Generative AI and the Economy

You can learn about the impact of generative AI on the economy by reading these reports and articles:
- McKinsey: [The economic potential of generative AI: The next productivity frontierOpens in a new tab](https://www.mckinsey.com/capabilities/mckinsey-digital/our-insights/the-economic-potential-of-generative-ai-the-next-productivity-frontier#introduction), McKinsey Digital report, June 2023 
- [GPTs are GPTs: An Early Look at the Labor Market Impact Potential of Large Language ModelsOpens in a new tab](https://arxiv.org/pdf/2303.10130.pdf), Tyna Eloundou, Sam Manning, Pamela Miskin, and Daniel Rock, March 2023 (arXiv:2303.10130)
- Goldman Sachs: [The Potentially Large Effects of Artificial Intelligence on Economic GrowthOpens in a new tab](https://www.gspublishing.com/content/research/en/reports/2023/03/27/d64e052b-0f6e-45d7-967b-d7be35fabd16.html), Joseph Briggs and Devesh Kodnani, March 2023

## 2.1 Software Applications

### Using generative AI in software applications

Generative AI makes deploying apps like sentiment analysis much simpler
![](/img/2.01.png) 

### Trying generative AI code yourself (optional)

[DLAI - Learning Platform Beta](https://learn.deeplearning.ai/genai4e/lesson/1/activity1)

```python
import openai
import os

openai.api_key = os.getenv("OPENAI_API_KEY")

def llm_response(prompt):
    response = openai.ChatCompletion.create(
        model='gpt-3.5-turbo',
        messages=[{'role':'user','content':prompt}],
        temperature=0
    )
    return response.choices[0].message['content']

prompt = '''
    Classify the following review 
    as having either a positive or
    negative sentiment:

    The banana pudding was really tasty!
'''

response = llm_response(prompt)
print(response)
```

### Lifecycle of a generative AI project

![](/img/2.02.png)
- Here the sentiment was classified as positive even though it shouldn't have
- Have to continuously improve the system

![](/img/2.03.png) 
- list of techniques to improve the system

### Cost intuition

![](/img/2.04.png) 
![](/img/2.05.png) 
- Given typical adult reads at 250 words/min, cost is approx 8cents per hour

## 2.2 Advanced Technologies: Beyond Prompting

### Retrieval Augmented Generation (RAG)

RAG enables LLM to have context
![](/img/2.06.png) 
![](/img/2.07.png) 
![](/img/2.08.png) 

Examples of RAG Applications
![](/img/2.09.png) 
![](/img/2.10.png) 
![](/img/2.11.png) 

![](/img/2.12.png) 

### Fine-tuning

Fine tuning is another technique
- more complicated that RAG
- used to get output to fit a certain style

e.g. Want output to be "optimistic"
![](/img/2.34.png) 
- Give it additional words (10-100k or more) to learn from

Also used for apps where task isn't easy

e.g. summarizing customer service calls
![](/img/2.36.png) 

e.g. mimicking a writing/speaking style
![](/img/2.37.png) 

Also used to learn specific domain knowledge e.g.
- medical notes for patient with shortness of breat `Pt c/o SOB, DOE. PE: RRR,
  JVD absent, CTAB. EKG: NSR. Tx: F/u w/ PCP, STAT CXR, cont. PRN O2.`
- legal doc: `Licensor grants to Licensee, per Section 2(a)(iii), a
  non-exclusive right to use the intellectual property, contingent upon
  compliance with fiduciary duties outlined in Section 8, paragraphs 1-4, and
  payment as specified in Schedule B, within 15 days hereof.`

Some models don't require an expensive 100B+ parameter model
![](/img/2.41.png) 
- With fine tuning you can have a small model with 500-1k parameters work

### Pretraining an LLM

Pretraining is effective but very expensive
![](/img/2.43.png) 

### Choosing a model

Some guidelines for choosing a model size
![](/img/2.45.png) 

![](/img/2.46.png) 

### How LLMs follow instructions: Instruction tuning and RLHF (optional)

Given standard trianing from internet, output might not be what you expect
![](/img/2.48.png) 
- want output to be 'paris'

Pre-tuning is to train with "good answers" when training
![](/img/2.49.png) 

RLHF: Reinforcement Learning from Human Feedback, is technique to "score"
answers to train LLM
![](/img/2.51.png) 
- Score is a reward to LLM when it learns good answers

### Tool use and agents (optional)

Given order taking app 
![](/img/2.52.png) 
- Add a user confirmation step to avoid mistakes
- Do not use LLMs in mission/life critical apps

LLMs aren't great at precise math
![](/img/2.55.png) 

can use external commands e.g. `CALCULATOR` to improve functions
![](/img/2.56.png) 

"Reasoning" Agents also extend capabilities
![](/img/2.57.png) 

## 3.1 Generative AI and Business

### Day-to-day usage of web UI LLMs

![](/img/3.03.png) 
![](/img/3.04.png) 
![](/img/3.05.png) 
![](/img/3.06.png) 
- can be ok at writing simple code

### Task analysis of jobs

Framework by Erik Brynjolfsson, Tim Mitchell, and Daniel Rock for analyzing the
work tasks for possible automation using AI
![](/img/3.08.png) 

![](/img/3.09.png) 
- Businesses start with augmentation and iterate into automation

![](/img/3.11.png) 
- experiment with LLM to see if it has potential to automate a task

![](/img/3.12.png) 

### Additional job analysis examples
### New workflows and new opportunities
### Teams to build generative AI software
### Automation potential across sectors
## 3.2 Generative AI and Society
### Concerns about AI
### Artificial General Intelligence
### Responsible AI
### Building a more intelligent world
