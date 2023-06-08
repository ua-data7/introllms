![banner](assets/dailyprod-banner.png){width=1000}

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.

What tasks do you do every day? What are your daily habits? Where are the pain points that you can improve? Where do you spend time that you wish you had back? 

## Advanced Prompt Engineering

Advanced primpt engineering goes beyond single prompt engineering. It is the process of creating a series of prompts that are designed to help you achieve a more complex goals.

### Example 1: Personal Planner

Suppose you're using ChatGPT as a personal planner. You might give it a set of instructions like this:

??? example "Planning your day"

    ```
    ChatGPT, I need your help planning my day tomorrow.
    First, please list all my scheduled meetings and deadlines from my calendar. 
    Then, taking into account 2 hours of break time, could you suggest a time-managed itinerary for me? 
    Lastly, based on the priority of the tasks, can you create a task list in the order I should tackle them?
    ```

This prompt involves three tasks: **retrieving data**, **creating an itinerary**, and **arranging tasks based on priority**.

### Example 2: Content Creation

Imagine you're using ChatGPT for content creation. Here's how you might chain instructions:

??? example "Blog post creation"

    ```
    ChatGPT, I'd like to write a blog post about sustainable living. 
    First, could you generate a list of five key topics that I should cover? 
    Once we have the topics, can you then provide a brief outline for each of them? 
    Finally, for each of the outlines, could you come up with an engaging introduction paragraph?
    ```

This prompt includes three tasks: **generating topics**, **creating outlines**, and **writing introduction paragraphs**.

## Practical Applications of ChatGPT

Building on our understanding of prompt engineering, let's now delve into the more advanced practical applications of ChatGPT. These applications extend beyond simple question-answering or text generation and can be leveraged for numerous productivity tasks.

### Example 1: Personal Assistant Tasks

ChatGPT can be used as a personal assistant to help you with a variety of tasks. For instance, you can use it to draft emails, manage your calendar, or schedule meetings.

#### Drafting emails

You can ask ChatGPT to draft an email by giving it the main points to include. For instance:

??? example "Drafting an email"

    ```
    ChatGPT, can you help me draft an email? It's for my team, summarizing the key points from our meeting today. The points are:
    We agreed on a new project timeline with a final deadline of July 30th.
    Our client asked for a weekly status update, which we'll rotate among team members.
    We decided to conduct a brainstorming session next Wednesday to come up with new marketing strategies.
    Remember to submit expense reports by the end of this week.
    ```

ChatGPT will then generate a professional and well-structured email draft based on these points.

#### Managing your calendar

Assuming an integration with a calendar API (see [OpenAI API](../openai_api/#openai-api)), you might use ChatGPT to manage your schedule as follows:

??? example "Managing Calendar"

    ```
    ChatGPT, can you schedule a team meeting for next Tuesday at 3 PM in my calendar? Also, set a reminder for me to prepare the meeting agenda by Monday afternoon.
    ```

ChatGPT would use the calendar API to create the meeting event and set the corresponding reminder.

??? warning "Limitations"
    Often, you will see that ChatGPT is able to generate the correct answer, but it will also issue a warning:

    ```
    Please note, as of my knowledge cutoff in September 2021, 
    this feature would require custom coding and integration with an existing calendar system, 
    as ChatGPT by itself does not have the ability to interact directly with external systems and databases.
    ```

    **However**, with the public release of the OpenAI API, this is no longer a limitation. You can now integrate ChatGPT with external systems and databases. See the [OpenAI API](../openai_api/#openai-api) section for more details.

#### Taking one step further!

??? example "Your AI personal assistant!"
    Very recently, Microsoft announced Windows Copilot which will bring a range of new generative AI-powered features to Windows 11 starting in June. Notably, this is a Windows feature and so far will not be integrated with MAC OS. See this ![article](https://www.theverge.com/2023/5/23/23732454/microsoft-ai-windows-11-copilot-build) for more details.

### Example 2: Creative writing and brainstorming

ChatGPT excels in innovative applications. Whether you're developing a research proposal, constructing a lecture series, or strategizing a campus event, you can harness ChatGPT to cultivate original ideas, write comprehensive narratives, or devise memorable catchphrases. In ideation sessions, it can contribute various perspectives and proposals, invigorating creativity and fostering critical thinking.

#### Research Proposal

 Suppose you're crafting a research proposal about the influence of mythical narratives on modern literature but are stuck on formulating your main hypothesis. You might use ChatGPT in this way:

??? example "Modern literature research Proposal"

    ```
    ChatGPT, I'm constructing a research proposal and I need help formulating a unique hypothesis. 
    The research is about the influence of mythical narratives, such as those featuring wizards and magical creatures, on modern literature. 
    Can you help refine this idea and suggest some potential research questions and methodologies?
    ```

ChatGPT could then generate a refined research idea, list potential research questions, and suggest methodologies, thereby aiding in your research proposal development process.

#### Campus sustainability campaign

Imagine you're brainstorming ideas for a new campus sustainability campaign. You might prompt ChatGPT as follows:

??? example "Campus sustainability campaign"

    ```
    ChatGPT, I need some creative ideas for a sustainability campaign promoting eco-friendly practices on our campus. 
    The campaign should emphasize our institution's commitment to sustainable practices and our role in promoting environmental responsibility. 
    Can you suggest some innovative strategies, potential catchphrases, and engaging events?
    ```

ChatGPT can then provide a variety of strategies, memorable catchphrases, and event ideas to stimulate your brainstorming session, offering different perspectives and creative solutions.

### Example 3: Programming help

Another impressive application of ChatGPT is in the field of programming. You can use it as a coding assistant, where it can help write code, debug issues, or explain complex code snippets. By asking it to convert your high-level descriptions into code, or to suggest improvements for existing code, you can significantly enhance your programming productivity.

#### Coding Assistant 

Suppose you're working on a Python program to perform data analysis, but you're not sure how to write a function to calculate the median from a list of numbers. You might use ChatGPT like this:

??? example "Python median function"
    
    ```
    ChatGPT, I'm trying to write a Python function that takes a list of numbers as an argument and returns the median. I'm not sure about the best way to implement this. Could you help me write the code?
    ```

ChatGPT could then provide you with a suitable Python function, demonstrating the logic to calculate the median from a list of numbers.

#### Debugging

Let's say you're having trouble with a piece of JavaScript code that's not behaving as expected. You could ask ChatGPT for help as follows:

??? example "Debugging JavaScript"

    ```
    ChatGPT, my JavaScript code to add event listeners to buttons isn't working as expected. Here's the code:
    ```
    ```javascript
    let buttons = document.querySelectorAll('.btn');
    for (let i = 0; i < buttons.length; i++) {
    buttons[i].addEventListener('click', function() {
        console.log('Button ' + i + ' clicked');
        });
    }
    ```
    ```
    When I click a button, it always logs 'Button 5 clicked', no matter which button I click. What's going wrong, and how can I fix it?"
    ```

ChatGPT could then explain the issue (in this case, a common pitfall with JavaScript closures) and suggest a corrected version of your code.

??? warning "Limitations"
    Remember, while ChatGPT is knowledgeable in many programming languages and concepts, it doesn't replace a full Integrated Development Environment (IDE) or debugger and should be used as a supplementary tool for coding assistance.

## Bing AI for Advanced Information Gathering and Verification

Bing AI offers a multitude of features encompassing semantic search, image search, and real-time web data extraction. These capabilities are powered by Microsoft's state-of-the-art AI technologies, capable of understanding and interpreting web content on a large scale. For instance, Bing AI can sift through search results, images, and other web content to provide you with concise, accurate, and pertinent information.

Let's consider some advanced use cases where Bing AI can be particularly beneficial:

### Example 1: Complex Web Searches

Suppose you're examining the implications of climate change on polar ice caps for your environmental science class. A conventional search might yield an overwhelming number of results, making it challenging to pinpoint the most relevant information. With Bing AI, however, you can perform a more refined search like:

??? example "Complex web searches"
    
    ```
    Bing AI, find me recent peer-reviewed articles on the rate of polar ice cap melting due to climate change.
    ```

Bing AI would then employ its semantic search abilities to locate relevant scientific articles, even summarizing the key findings.

### Example 2: Data Aggregation

Imagine you're evaluating the impact of a recent educational policy change across several countries for a comparative education study. Instead of manually hunting for data for each country, you could instruct Bing AI:

??? example "Data aggregation"

    ```
    Bing AI, compile the latest data on literacy rates in OECD countries following the 2023 education policy modifications.
    ```

Bing AI could then efficiently mine and aggregate the requested data from various reliable sources.

### Example 3: Information Verification

In a world abundant with misinformation, verifying claims is crucial. For example, if you encounter a claim that a particular university has a certain acceptance rate, you can verify it by asking Bing AI:

??? example "Information verification"

    ```
    Bing AI, validate the current acceptance rate of The University of Arizona, Arizona State University, and Northern Arizona University.
    ```

Bing AI would then cross-check the information from reliable sources and provide you with a verified answer.

These advanced capabilities of Bing AI can significantly enhance productivity in research, information verification, and data analysis.

## Synergistic Use of ChatGPT and Bing AI 

Integrating the capabilities of ChatGPT and Bing AI brings together the strengths of both platforms. While ChatGPT shines in understanding context and generating human-like text, Bing AI excels in web data extraction and advanced search capabilities. By combining these, you can create a powerful AI toolset that can help manage your daily tasks and fulfill your information needs in a more streamlined and efficient manner.

Let's now delve into a couple of practical examples showcasing how to leverage both ChatGPT and Bing AI:

### Example 1: Research Assistance

Imagine you're undertaking a research project on educational policies across various countries. You can prompt:

??? example "Literacy rates"

    ```
    ChatGPT, using Bing AI, find me the latest data on literacy rates in OECD countries after the 2023 education policy changes and 
    summarize the findings.
    ```

In this case, ChatGPT collaborates with Bing AI to extract the relevant data and provide a summarized version of the key findings.

### Example 2: Lecture Preparation

Suppose you're preparing a lecture on climate change impacts on polar ice caps. You could ask:

??? example "Lecture preparation"

    ```
    ChatGPT, using Bing AI, find me recent peer-reviewed articles on the rate of polar ice cap melting due to climate change and create 
    a summarized overview for my lecture.
    ```

Here, Bing AI assists in locating the articles, while ChatGPT uses its language generation abilities to create a lecture-ready summary.

Harnessing the synergies of ChatGPT and Bing AI can result in powerful capabilities that can revolutionize your academic and administrative workflows.

