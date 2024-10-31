
## Digital Method of the Month: Software Development with Generative AI
05 November 2024
Authors: Martin Disley (m.disley@ed.ac.uk)

## Schedule
12:00 -  Housekeeping (5 minutes)
12:05 -  Overview of this session (5 minutes)
12:10 -  Introductions
12:15 - Document discussion
12:55  - Closing remarks

## What is Generative AI Augmented Software Development
Software development is, fundamentally, a writing practice; and, like every other writing practice, the introduction of Large Language Models (LLMs) in recent years has presented challenges and opportunities for how it will evolve. Of the many benefits its proponents claim it may bring, the most interesting for us is what is often referred to as its "democratising potential": giving the capacity to build computational tools to those who would be unable to write their code and expanding the capacities of those who have some limited programming experience.

This document will discuss how these tools deliver this capacity, their limitations, and some strategies for effectively and safely using LLMs to aid software development.

## Translation and Extrapolation
When we generate code from text prompts using LLMs, we are often initiating a process similar to machine translation, but with some extra steps. Transformer models, the machine learning architecture used in LLMs, have proven to be very adept at translating between languages. Key to this is the idea of vector encoding, a way of representing the relational strength of sub-word units numerically. As numerical representations, independent of natural language, they can be decoded into any other natural language.

In the context of computer code, the model interprets the user's input – a description of a logical or algorithmic process described in a natural language – and generates a version of it in a machine-readable language, such as Python or JavaScript. This is not that different from the task of translating a cake recipe written in English to another that would produce the same cake written in German. So we can think of one part of this process as a kind of translation.

What's happening when we use instructional prompts (when we "ask it for something"), these "extra steps" often account for a kind of information upscaling - a leap from a *reference to a thing*, to *an example of a thing itself*; for instance, inputting the prompt "give me a cake recipe",  and receiving in return something that resembles a complete cake recipe. 

When LLMs are used to link representations of things at different scales, it is helpful to understand what has transpired as a kind of information upscaling or extrapolation – it has taken your reference to a cake recipe and returned a detailed example of one. This extrapolation is statistically guided but ultimately stochastic, and since there are many likely possibilities for cake recipes that it could return, the stochastic processes involved are operating within a broad range of variability, leading to a wide array of potential outcomes. The chances it will return a recipe that will produce the kind of cake you were after are extremely small.

The further the information in your input is scaled or extrapolated, the greater the chance of misaligned output (the wrong kind of cake) or errors (adding extra ingredients that shouldn't be there). Thinking about code generation as the combination of *extrapolation* and *translation* is very useful for understanding how to get the most out of LLMs regardless of how proficient in programming you already are. Translation is often a one-to-one or a near one-to-one mapping. Extrapolation is always a one-to-many mapping.

The more domain knowledge you bring - the more able to specify in your input -  whether that's about baking or programming the less *extrapolation* the model has to do. It would be therefore follow to suggest that to minimise errors we must minimise extrapolation. However, taken too far, this would defeat the purpose of using a Generative AI tool. *Extrapolation* is a utility of these models that we want to leverage. If it were simply a machine translator, generative AI would be of no use to proficient programmers, since they would be required to type nearly as many words in natural language as they were in their chosen programming language, or no-coders, whose natural language inputs would not be successfully translated. 

Using generative AI for software development is therefore a game of min-max optimisation, a balancing act: crafting the most minimal input that will generate code producing behaviour closest to your intentions, or finding the smallest expression of the logic that you want, that minimises the errors or hallucinations when extrapolated.

## Strategies
### Least-to-Most Prompting: 
Least-to-Most prompting is a prompting strategy that minimises extrapolation. It involves building the instruction's complexity up incrementally. Starting with simple requests and gradually increasing complexity to ensure the model is on track before advancing. However, for those with minimal programming experience, this can be tricky since they may not be able to describe the implementation of what they want at the lowest level.

### Self-Ask Prompting: 
Those with less programming experience might find self-ask prompting more useful instead. Self-ask prompting involves encouraging the model to ask clarifying questions along the way. For example, you want to build a portfolio site for your project but are not aware of the relative merits of using Django or Flask, so you ask the model to give you these and then, informed with this knowledge, make the decision yourself.

### Chain-of-Thought Prompting:
Encouraging the model to "think step-by-step" by explicitly prompting it to break down complex tasks into intermediate reasoning steps enhances its ability to solve problems that require logical deduction. Learn more about chain-of-thought prompting

### ReAct (Reason + Act):
This method focuses on eliciting advanced reasoning, planning, and even tool use from the LLM. By structuring prompts to encourage these capabilities, developers can unlock more sophisticated and powerful applications. Learn more about ReAct

## Sandboxing 
A good principle in software development is not to run code you cannot fully interpret yourself. But, like any principle, in practice there are, of course, many times when this is not followed. Frustrated, time-pressured programmers (myself very much included!) will often copy potential solutions from sources like Stack Overflow and paste them into their own scripts without thoroughly reviewing them. It is important, though, to keep in mind how scale and scope affect this practice, though. Pasting in a couple of lines from Stack Overflow that might rectify some broken logic is a very different scenario to generating and executing a complete application script without being able to read and interpret it.

Running code that you cannot read introduces several dangers. The code may contain malicious elements, such as backdoors or exploits, putting your system or data at risk. Moreover, the code might manipulate or delete data in ways you do not expect, resulting in the loss or corruption of important files. Additionally, the code could be inefficient, consuming excessive resources such as CPU and memory, leading to a slowdown or even system failure.

One way to explore generated code safely is by sandboxing it, a safety and security practice where code is executed in a controlled and isolated environment, known as a sandbox. This environment allows the application to operate without access to the host computer's file system or applications. Virtual machines are one method of creating a sandbox, but a much simpler method would be a browser-based interactive programming environment such as Google's Colab or the University's own Noteable platform. Using a browser-based interactive programming environment such as Noteable, you can execute code generated by an LLM without it being able to access your own computer's file system.

# Tools to Explore
## Natural Language Based Editors
1. [**Claude Artifacts**](https://claude.ai/): A feature of Anthropic's Cluade taht turns conversations into a basic development environment. It's consists of live document and preview window for media generated by the Claude along with methods for export. This allows for easier iteration as changes are applied to the live document in the session rather than being required to be copied out. [Docs](https://support.anthropic.com/en/articles/9487310-what-are-artifacts-and-how-do-i-use-them)
2. [**GitHub Spark**](https://githubnext.com/projects/github-spark/): An AI-enabled platform for developing and sharing micro applications (“sparks”), which can be customised to meet your precise needs and preferences, and can be used directly on your desktop and mobile devices, eliminating the necessity to write or deploy any code. Not fully released, currently on waitlist.

## Browser-Based Interactive Programming Environments (IDEs) with AI tools
1. [**Google Colab**](https://colab.research.google.com/): A cloud-based Jupyter notebook environment that allows you to write and execute Python code in your browser, with powerful features for data analysis, machine learning, and collaboration. [Documentation](https://colab.research.google.com/notebooks/welcome.ipynb)
5. [**Replit Ghostwriter**](https://replit.com/ai): An AI tool within the Replit coding platform that provides real-time suggestions, refactoring, and debugging assistance. [Blog Post](https://blog.replit.com/ghostwriter)

## Stand alone IDEs with AI tools
1. [**Cursor**](https://www.cursor.com/): An AI-powered code editor that enhances the coding experience with intelligent code suggestions and real-time collaboration features. [Documentation](https://www.cursor.com/)
7. [**Zed**](https://zed.dev/ai): A collaborative code editor designed for real-time pair programming and integrated AI assistance, helping developers write code more efficiently. [AI Features](https://zed.dev/ai)

## IDE Extensions
1. [**GitHub Copilot**](https://github.com/features/copilot): An AI-powered code completion tool that suggests code snippets and entire functions as you type, improving productivity. [Documentation](https://docs.github.com/copilot)
2. [**Tabnine**](https://www.tabnine.com/): An AI-driven code completion tool that integrates with popular IDEs and learns from your codebase to provide relevant suggestions. [Documentation](https://docs.tabnine.com/)
3. [**Kite**](https://www.kite.com/blog/product/kite-is-saying-farewell/): An AI-powered coding assistant that offers code completions and documentation as you code, working with various IDEs. Kite has shut down as a commercial enterprise but have open-sourced there tools
7. [**Codeium**](https://codeium.com/): A code completion tool that integrates with IDEs to provide real-time suggestions, explanations, and examples based on the context. [Documentation](https://docs.codeium.com/overview/getting-started)
8. [**DeepCode**](https://snyk.io/platform/deepcode-ai/): An AI-powered static analysis tool that reviews code and suggests improvements or identifies bugs before the code is executed. [Snyk Platform](https://snyk.io/)

## Chatbots

1. [**OpenAI Codex**](https://openai.com/index/openai-codex/): The underlying model for tools like GitHub Copilot, Codex can translate natural language prompts into code snippets across multiple programming languages. [Playground](https://platform.openai.com/playground)
4. [**ChatGPT for Developers**](https://platform.openai.com/): A conversational AI tool that can assist with answering programming questions, troubleshooting, and generating code based on user prompts. [API Introduction](https://openai.com/index/introducing-chatgpt-and-whisper-apis/)

## For Designers
1. [**Figma Dev Mode**](https://www.figma.com/dev-mode/): A feature in Figma that enables developers to access design specifications, assets, and code snippets directly from design files, streamlining the handoff process between designers and developers. [Documentation](https://www.figma.com/dev-mode/)

## CDCS Upcoming training
[**Efficient Prompting for Generative AI Tools**](https://www.cdcs.ed.ac.uk/events/efficient-prompting-generative-ai-tools-nov24)
>This training workshop aims to introduce the main strategies of prompt engineering including tips and certain practices to achieve optimal outputs with Gen-AI tools. After providing a hands-on overview of prompt engineering, certain features of ChatGPT will be discussed for fostering the research practices. The target audience for this workshop is mainly researchers and practitioners working in different fields who are interested in using the Gen-AI tools more efficiently and responsibly in their daily work.

## CDCS Past training Resources
https://github.com/DCS-training/Digital-Method-of-the-Month/blob/main/DMM%20Docs/Machine%20Learning.md


## Feedback
https://forms.office.com/r/YYNrqvuNr8