# [Coursera Deeplearinng.ai: Generative AI for Everyone](https://www.coursera.org/learn/generative-ai-for-everyone/home/week/1)

## 1.1 Introduction to Generative AI

### 1.1.1 What is Generative AI

![](/img/1.04.jpg) 

AI is already pervasive in our lives and many of us use it dozens of times a
day or more without even thinking about it. e.g. Every time you do a web search
on Google or Bing, that's AI.

But many AI systems have been complex and expensive to build, and generative AI
is making many AI applications much easier to build.

1.11.jpg

### 1.1.2 How Generative AI works

1.13.jpg
- supervised learning, which turns out to be really good at labeling things.
- supervised learning and generative AI, are the two most important tools in AI today.

1.15.jpg
- Supervised learning is the technology that has made computers very good when
- given an input, which I'm going to call A, to generate a corresponding output, which I'm going to call B.

In self-driving cars and in driver assistance systems, supervised learning is
used to take as input a picture of what's in front of your car and radar info
and label that with the position of other cars.

Give it a medical x-ray, it can try to label that with a medical diagnosis.

I've also done a lot of work in manufacturing defect inspection where you can
have a system take a picture of a phone as it rolls off the assembly line and
check if the phone has any scratches or other defects, or in speech
recognition, the input A would be a piece of audio and we would label that with
the text transcript, or as a final example, if you run a restaurant or some
other business where occasionally you have reviews written about your business
or your products, supervised learning can read those reviews and label each one
as having either a positive or a negative sentiment.

This is useful for reputation monitoring of the business.

It turns out the decade of around 2010-2020 was a decade of large-scale
supervised learning.

I want to touch on this briefly because it turns out this laid the foundation
for modern generative AI.

But what we found starting around 2010 was that for a lot of applications, we
had a lot of data, but even as we fed it more data, its performance wasn't
getting that much better if we were training small AI models.

This means, for example, if you were building a speech recognition system, even
as your AI listened to tens of thousands or hundreds of thousands of hours of
data, that's a lot of data, it didn't get that much more accurate compared to a
system that listened to only a smaller amount of audio data.

But what more and more researchers started to realize through this period is if
you were to train a very large AI model, meaning an AI model on very fast, very
powerful computers with a lot of memory, then its performance as you fed it
more and more data will just keep on getting better and better.

In fact, years ago when I started and led the Google Brain team, the primary
mission that I set for the Google Brain team in the early days was I said,
let's just build really, really large AI models and feed them a lot of data.

And fortunately, that recipe worked and ended up driving a lot of AI progress
at Google.

Large-scale supervised learning remains important today, but this idea of very
large models for labeling things is how we got to generative AI today.

Let's look at how generative AI generates text using a technology called large
language models.

Here's one way that large language models, which I will abbreviate LLM, can
generate text.

Given an input like, I love eating, this is called a prompt, an LLM can then
complete this sentence with maybe bagels with cream cheese, or if you run it a
second time, it might say, my mother's meatloaf, or if you run it a third time,
maybe it'll say out with friends.

How does an LLM, a large language model, generate this output? It turns out
that LLMs are built by using supervised learning.

That's a technology to input A and output a label B.

It uses supervised learning to repeatedly predict what is the next word.

For example, if an AI system has read on the Internet a sentence like, my
favorite food is a bagel with cream cheese, then this one sentence will be
turned into a lot of data points for it to try to learn to predict the next
word.

Specifically, given this sentence, we now have one data point that says, given
the phrase, my favorite food is a, what do you think is the next word? In this
case, the right answer is bagel.

Also, given my favorite food is a bagel, what do you think is the next word?
It's with, and so on.

This one sentence is turned into multiple inputs A and outputs B for it to try
to learn from where the LLM is learning given a few words to predict what is
the next word that comes after.

When you train a very large AI system on a lot of data, a lot of data for LLMs
means hundreds of billions of words, and in some cases, more than a trillion
words, then you get a large language model like ChatGPT that's given a prompt
is very good at generating some additional words in response to that prompt.

For now, I'm omitting some technical details.

Specifically, next week, we'll talk about a process that makes LLMs not just
predict the next word, but actually learn to follow instructions and also be
safe in what it outputs.

But at the heart of LLMs is this technology that's learned from a lot of data
to predict what is the next word.

That's how large language models work; they're trained to repeatedly predict
the next word.

It turns out that many people, perhaps including you, are already finding these
models useful for day-to-day activities at work to help with writing, to find
basic information, or to be a thought partner to help think things through.

Let's take a look at some examples in the next video.

### 1.1.3 LLMs as a thought partner

### 1.1.4 AI is a general purpose technology

### 1.1.1 Quiz

## 1.2 Generative AI Application

### 1.2.1 Writing

### 1.2.1 Reading

### 1.2.1 Chatting

### 1.2.1 What LLMs can and cannot do

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

