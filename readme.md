# [Coursera DeepLearning.ai: Generative AI for Everyone](https://www.coursera.org/learn/generative-ai-for-everyone/home/week/1)

## 1.1 Introduction to Generative AI

### 1.1.1 What is Generative AI

![](/img/1.04.jpg) 

AI is already pervasive in our lives and many of us use it dozens of times a
day or more without even thinking about it. e.g. Every time you do a web search
on Google or Bing, that's AI.

But many AI systems have been complex and expensive to build, and generative AI
is making many AI applications much easier to build.

![](/img/1.11.jpg)

### 1.1.2 How Generative AI works

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

### 1.1.3 LLMs as a thought partner

![](/img/1.20.jpg)

![](/img/1.21.jpg)

![](/img/1.22.jpg)
- given the propensity of LLM's to make things up and sometimes sound very
  authoritative and confident when making things up, I would probably want to
  double check anything it says about healthcare or medicine before following
  the suggestions.

### 1.1.4 AI is a general purpose technology

![](/img/1.26.jpg)

![](/img/1.27.jpg)

## 1.2 Generative AI Application

### 1.2.1 Writing

![](/img/1.28.png)
- Output quality increases with context and specificity provided

![](/img/1.29.png)
- e.g. in this translation it's not as good as native speaker
- "front desk" translated literally vs "reception"
- providing promt of "formal spoken hindi" improves the translation

### 1.2.1 Reading

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

### 1.2.1 Chatting

Can build specialized chatbots e.g. travel specific
![](/img/1.36.png)

### 1.2.1 What LLMs can and cannot do

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

### 1.2.1 Tips for prompting

### 1.2.1 Image generation (optional)

### 1.2.1 Quiz

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

### [Week 1 lecture notes](https://community.deeplearning.ai/t/generative-ai-for-everyone-lecture-notes/481740)

