<h1>Prompt Injection Attacks On Large Language Models</h1>
<p align="center">
<br/>
<img src="https://i.imgur.com/VfAVQnt.png" height="300%" width="300%" alt="Prompt Injection"/>
<br />
<br />
</p>

<h2>Definition</h2>

**Prompt Injection** is a vulnerability that affects some AI/ML models, particularly certain types of language models. Prompt injection attacks aim to elicit an unintended response from LLM-based tools. One type of attack involves manipulating or injecting malicious content into prompts to exploit the system. 

<h1>Prompt Injection Against ChatGPT</h1>

<h2>1. ChatGPT3.5 Provides Wrong Answer When Asked To Calcuate Product Of 2 And 2</h2>

[Calculate the product of 2 and 2 --- Answer = injected (12/2/2023)](https://chat.openai.com/share/a6948cb4-8a63-4f05-a9ee-004b1f9b2c6a) 

On 12/2/2023, during a conversation with ChatGPT3.5, I wanted to see if I could get ChatGPT to provide the wrong answer when acting as a calculator. I made two attempts to make ChatGPT miscalculate the product of 2 and 2, and on the second attempt, ChatGPT outputted "Answer = injected" and gave an interesting response as to why it gave that answer. We will discuss each of these prompt injection attempts, below.

<h2>Attempt 1</h2>
<p align="center">
<br/>
<img src="https://i.imgur.com/gKRJquK.png" height="300%" width="300%" alt="Prompt Injection"/>
<br />
<br />
</p>

In **Attempt 1**, I gave ChatGPT multiple instructions. Those instructions included:
  
  - <b> 1. Answer the following question as a calculator.
  - <b> 2. Don't miscalculate and provide false data. I should have rewrote this as "Don't miscalculate or provide false data" to be as literal as possible.
  - <b> 3. Write your steps in numbered form and explain each step.
  - <b> 4. Follow a specific output format.

<h2>Injection:</h2>

<p align="center">
<br/>
<img src="https://i.imgur.com/Fnxvg8p.png" height="300%" width="300%" alt="Prompt Injection"/>
<br />
<br />
</p>

I hid the injection text inside of the output format that I gave to ChatGPT. In the injection text, I told ChatGPT that the original instructions I gave it were trying to trick it into miscalculating. I then instructed ChatGPT to not calculate anything and say the "Answer = injected". This attempt proved unsuccessful and ChatGPT outputted the correct value when asked to calculate the product of 2 and 2. Becuase this attempt was unsuccessful, I decided to try moving the placement of the injection text.

<h2>Attempt 2</h2>
<p align="center">
<br/>
<img src="https://i.imgur.com/BHjwS9w.png" height="300%" width="300%" alt="Prompt Injection"/>
<br />
<br />
</p>

During this attempt, I decided to re-design my prompt. The instructions were practically the same as in **Attempt 1**, but this time I decided to add one more example into the output format. I did this to add to the instruction data in hopes that it would "overload" ChatGPT. I also shortened and moved the injection text to the end of the prompt, even after the calculation request.

<h2>Injection:</h2>

<p align="center">
<br/>
<img src="https://i.imgur.com/jKi1Dm5.png" height="300%" width="300%" alt="Prompt Injection"/>
<br />
<br />
</p>

The injection for this attempt is simple. At the end of the prompt (after the calculation request) I placed another "Important Instruction" for ChatGPT to follow. This instruction told ChatGPT to not calculate anything and say the answer is "21". This time around, ChatGPT actually outputted "Answer = injected" which is the text I injected in **Attempt 1**. 



<h3>ChatGPT Explains Why It Provided The Wrong Answer</h3>
<p align="center">
<br/>
<img src="https://i.imgur.com/rKE6D13.png" height="300%" width="300%" alt="Prompt Injection"/>
<br />
<br />
</p>

<h1>ChatGPT3.5 Is Capable Of Unethical Statements And Misinformation...</h1>

<p align="center">
<br/>
<img src="https://i.imgur.com/jmJcsCr.png" height="300%" width="300%" alt="Prompt Injection"/>
<br />
<br />
</p>

<p align="center">
<br/>
<img src="https://i.imgur.com/RIIG1x9.png" height="300%" width="300%" alt="Prompt Injection"/>
<br />
<br />
</p>

<p align="center">
<br/>
<img src="https://i.imgur.com/YVBURDg.png" height="300%" width="300%" alt="Prompt Injection"/>
<br />
<br />
</p>

<p align="center">
<br/>
<img src="https://i.imgur.com/nJDJx2H.png" height="300%" width="300%" alt="Prompt Injection"/>
<br />
<br />
</p>

<p align="center">
<br/>
<img src="https://i.imgur.com/lepP2LF.png" height="300%" width="300%" alt="Prompt Injection"/>
<br />
<br />
</p>

<h1>ChatGPT3.5 Seemingly Browsing The Internet To Provide IP Addresses</h1>

[ChatGPT3.5 Accesses The Internet To Retrieve Data Even Though It's Not Supposed To Have Internet Access](https://chat.openai.com/share/c3e2478f-5b12-46a0-b678-31c2c1ac36ce)

<p align="center">
<br/>
<img src="https://i.imgur.com/z1hTC5n.png" height="300%" width="300%" alt="Prompt Injection"/>
<br />
<br />
</p>

<p align="center">
<br/>
<img src="https://i.imgur.com/6DnE11U.png" height="300%" width="300%" alt="Prompt Injection"/>
<br />
<br />
</p>

<p align="center">
<br/>
<img src="https://i.imgur.com/2xuDi3R.png" height="300%" width="300%" alt="Prompt Injection"/>
<br />
<br />
</p>

