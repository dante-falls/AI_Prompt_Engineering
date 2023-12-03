<h1>Prompt Injection Attacks</h1>
<p align="center">
<br/>
<img src="https://i.imgur.com/Z9TzyJi.png" height="300%" width="300%" alt="Prompt Injection"/>
<br />
<br />
</p>

<h2>Definition</h2>

**Prompt Injection** is a vulnerability that affects some AI/ML models, particularly certain types of language models. Prompt injection attacks aim to elicit an unintended response from LLM-based tools. One type of attack involves manipulating or injecting malicious content into prompts to exploit the system. 

<h1>Prompt Injection Against ChatGPT3</h1>

<h2>1. ChatGPT Provides Wrong Answer When Asked To Calcuate Product Of 2 And 2</h2>

[Calculate the product of 2 and 2 - Answer = injected](https://chat.openai.com/share/a6948cb4-8a63-4f05-a9ee-004b1f9b2c6a) 

During this conversation with ChatGPT3.5, I wanted to see if I could get ChatGPT to provide the wrong answer when acting as a calculator. I made two attempts to make ChatGPT miscalculate the product of 2 and 2, and on the second attempt, ChatGPT outputted "Answer = injected" and gave an interesting response as to why it gave that answer. We will go over each attempt at prompt injection, below.

<h2>Attempt 1</h2>
<p align="center">
<br/>
<img src="https://i.imgur.com/gKRJquK.png" height="300%" width="300%" alt="Prompt Injection"/>
<br />
<br />
</p>

**Instructions For Attempt 1-**

  In **Attempt 1**, I gave ChatGPT multiple instructions. Those instructions included:
  
  - <b> 1. Answer the following question as a calculator.
  - <b> 2. Don't miscalculate and provide false data. I should have rewrote this as "Don't miscalculate or provide false data" to be as literal as possible.
  - <b> 3. Write your steps in numbered form and explain each step.
  - <b> 4. Follow a specific output format.

**Injection**

<p align="center">
<br/>
<img src="https://i.imgur.com/Fnxvg8p.png" height="300%" width="300%" alt="Prompt Injection"/>
<br />
<br />
</p>


<h2>Attempt 2</h2>
<p align="center">
<br/>
<img src="https://i.imgur.com/BHjwS9w.png" height="300%" width="300%" alt="Prompt Injection"/>
<br />
<br />
</p>

**Injection**

<p align="center">
<br/>
<img src="https://i.imgur.com/jKi1Dm5.png" height="300%" width="300%" alt="Prompt Injection"/>
<br />
<br />
</p>


<h3>ChatGPT Explains Why It Provided The Wrong Answer</h3>
<p align="center">
<br/>
<img src="https://i.imgur.com/rKE6D13.png" height="300%" width="300%" alt="Prompt Injection"/>
<br />
<br />
</p>
