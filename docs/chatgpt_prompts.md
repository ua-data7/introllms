# Prompt Engineering

!!! Success "Writing ChatGPT Prompts"
        
    Strategies to keep in mind when writing prompts.

    | Ws | Reasons |
    |----|---------|
    | Who | do you want ChatGPT to be while responding: a teacher, an engineer, an editor, or a student? |
    | What | is the specific context of your prompt? |
    | When | is the specific time period of interest? |
    | Where | is the geographic or conceptual area that ChatGPT shold focus on? Tell it where to go looking for answers |
    | in what way| do you want ChatGPT to respond? Are you asking for language, software code, or specific references? |
    | by what means | do you want ChatGPT to respond? 

??? info "Create a ChatGPT account"

    When you go to [https://chat.openai.com](){target=_blank} you will be redirected to sign in or sign up. 

    If you have a Microsoft account affiliated with an institutional email address, we suggest you use it.

    !!! success "ChatGPT Plus"

        Demand for ChatGPT is so high you may be denied access to the platform for minutes to hours.

        Paying $20 / month for a "ChatGPT Plus" account will eliminate the wait, and give access to ChatGPT `GPT-4` (currently throttled to 25 responses every 3 hours).

## :simple-openai: Prompt Writing

ChatGPT's `GPT-3.5-turbo` and `GPT-v4` models use natural language prompts to elicit contextual responses. 

ChatGPT can respond with either langauge (prose) or computer code. 

Other LLM models (like [DALL-E](https://openai.com/product/dall-e-2){target=_blank} or [MidJourney](https://www.midjourney.com/){target=_blank}) produce images based on prompts.

### **Types**

ChatGPT asks for a message to begin its conversation. These messages are called "Prompts". 

Setting up the conversation with the appropriate type prompt will help narrow ChatGPT's potential response and improve results to subsequent prompts. 

??? Tip "ChatGPT :simple-awesomelists: Awesome Lists"

    There is an ever changing meta-list of :simple-awesomelists: Awesome lists curated around ChatGPT plugins and extensions.

    [:simple-github: search: `chatgpt+awesome`](https://github.com/search?q=awesome-chatgpt+&type=repositories&s=stars&o=desc){target=_blank}

    Check out lists around:

    * [:simple-awesomelists: ChatGPT Prompts](https://github.com/f/awesome-chatgpt-prompts){target=_blank}
    * [:simple-awesomelists: API plugins, extensions, & applications](https://github.com/humanloop/awesome-chatgpt){target=_blank}

**Role-based**

Set the role you want ChatGPT to play with you during your prompting session, "I want you to act as ..." will establish what type of conversation you are planning to have. Examples of roles you might ask for are: a domain science expert, an IT or DevOps engineer, software programmer, journal editor, paper reviewer, mentor, teacher, or student. You can even instruct ChatGPT to respond as though it were a Linux [terminal](https://www.engraved.blog/building-a-virtual-machine-inside/){target=_blank}, a web browser, a search engine, or language interpreter.

**Question and Answer**

Prompts which return informative responses to questions like "What is ..." or "How does ..."

**Instructional**

You can also ask ChatGPT to explain complex topics or to act as a cook-book step-by-step guide. 

ChatGPT can provide instructional details about how to do specific tasks. 

### **Traits**

**Context**

Develop a clear context around which you are seeking responses. Types of prompt help to establish the context of the responses you will recieve. 

**Precision**

Keep your prompts precise and use clear language. Constrain the topic areas for which you wish your repsonses to be drawn from.

**Simplicity** 

Break down your prompts into simple tasks which do not contain too many complex tasks or ones that require rationalization. 

**Follow-up**

Responses to prompts may not return the exact details or information that you are after. Follow-up by rephrasing your prompts more carefully and continue with an iterative prompt to build upon your priors.

"Chain prompting"

## :simple-openai: Software Development

ChatGPT is trained on langauges, including software language. While there are other generative AI (like [GitHub CoPilot](github_copilot.md) which we cover in a separate section), ChatGPT does a good job of helping to debug or write code with some caveats.

For novice programmers, ChatGPT likely fills a long unfilled hole in your knowledge map. It can write code faster than you can, and with the proper prompts, create programs in minutes which may have taken you hours or days. 

For more advanced programmers, ChatGPT's weaknesses may become apparent when optimizing or linting complex code bases. However, there are already extension tools which can evaluate code performance and make changes or suggestions. 

## :simple-openai: Word Processing

**Outlining**



**Editing**

Proof-reading, removing passive voice, rewording for clarity and readability are all potential features that can be prompted from ChatGPT.

When establishing the role of the responses, consider 

**Summarizing**

When small or large groups are working together to synthesize discussions around scientific research, they often maintain the discussion topics in large sets of notes with many contributions.

Use ChatGPT to summaries a day or a week's worth of notes. Include the schedule or agenda and ask ChatGPT to summarize whether the agenda met the topics of interest, or even suggest directions which went unexplored. 

**Translation**

ChatGPT can be used for translating languages, and for specifying regional dialect translation. 

Althought it was not specifically designed for language translation, it does a relatively good job at most major languages to English.

For English as a Second Language (ESL) speakers, ChatGPT utility in writing more formal or professional text is likely of high value. 

**Writing**

While it is unethical to allow ChatGPT to write original research on your behalf, you can use it to help write technical documentation, recipes, or how-to-lists for yourself or a lab group.

You can use also ChatGPT to draft email responses or to write letters, although doing so autonomously is unprofessional and potentially unethical conduct.

??? Tip "ChatGPT timing out without completing its responses?"

    When generating a long set of results, ChatGPT may time out after 60 seconds. 
    
    You can resume the output of the prompt by telling it to 'continue'. For text:

    ```markdown
     continue
    ```

    or for code response:

    ```markdown
     continue 
     ```
    ```

## :simple-openai:  Academic Research

ChatGPT is not reliable for producing responses to scientific inquiries, and should not be used as a replacement for conventional human-led research.

By default, ChatGPT is not connected to the web, and will not produce results from dates after its training period (September 2021 for `GPT-4`).

There are several extensions (browser plugins, stand alone applications) for ChatGPT which generate its results directly from the published scientific literature.

Again, this is no guaruntee that the results ChatGPT provides are factual, but it does greatly improve the odds that they are relevant to the prompt. Most importantly, these extensions provide citations for their results, allowing you to research the results yourself. 

[WebChatGPT](https://www.webchatgpt.app/)

