# Prompt Engineering

When can you use ChatGPT for research and education? 

``` mermaid
graph TB
  A((Start)) --> B("Does it matter if the outputs are true?  &nbsp");
  B -->| No | F("Safe to use ChatGPT");
  B -->| Yes | C("Do you have the ability to verify output truth and accuracy? &nbsp &nbsp");
  C -->| Yes | D("Understand legal and moral responsibility of your errors?  &nbsp &nbsp");
  C -->| No | E("Unsafe to use ChatGPT");
  D -->| Yes | F("Safe to use ChatGPT");
  D -->| No | E("Unsafe to use ChatGPT");

  style A fill:#2ECC71,stroke:#fff,stroke-width:2px,color:#fff
  style B fill:#F7DC6F,stroke:#fff,stroke-width:2px,color:#000
  style C fill:#F7DC6F,stroke:#fff,stroke-width:2px,color:#000
  style D fill:#F7DC6F,stroke:#fff,stroke-width:2px,color:#000
  style E fill:#C0392B,stroke:#fff,stroke-width:2px,color:#fff
  style F fill:#2ECC71,stroke:#fff,stroke-width:2px,color:#fff
```

Figure credit, based on: :fontawesome-brands-creative-commons-by: [ChatGPT and Artificial Intelligence in Education, UNESCO 2023 :fontawesome-regular-file-pdf:](https://www.iesalc.unesco.org/wp-content/uploads/2023/04/ChatGPT-and-Artificial-Intelligence-in-higher-education-Quick-Start-guide_EN_FINAL.pdf)


!!! Success "Writing ChatGPT Prompts"
        
    Strategies to keep in mind when writing prompts.

    | Ws | Reasons |
    |----|---------|
    | Who | do you want ChatGPT to role-play: an engineer, an editor, a teacher, or a student? |
    | What | is the specific context of your prompts? |
    | When | is the specific time period of interest? Specify if so. |
    | Where | is the geographic region or conceptual area? |
    | In what way | do you want ChatGPT to respond? Are you asking for language, software code, or specific references? |

??? info "Create a ChatGPT account"

    When you go to [https://chat.openai.com](){target=_blank} you will be redirected to sign in or sign up. 

    If you have a Microsoft account affiliated institutional email address, we suggest you use it.

    !!! success "ChatGPT Plus"

        Demand for ChatGPT is so high you may be denied access to the platform for minutes to hours.

        Paying $20 / month for a "ChatGPT Plus" account will eliminate the wait, and give access to ChatGPT `GPT-4` (currently throttled to 25 responses every 3 hours).

## How does ChatGPT Work?

Read the [:simple-openai: ChatGPT Documentation](https://openai.com/blog/chatgpt){target=_blank}

ChatGPT's `GPT-3.5-turbo` and `GPT-v4` models use natural language prompts to elicit contextual responses. 

ChatGPT can respond with either langauge (prose) or computer code. 

Other LLM models (like [DALL-E](https://openai.com/product/dall-e-2){target=_blank} or [MidJourney](https://www.midjourney.com/){target=_blank}) produce images based on prompts.

ChatGPT uses a form of syntax called [MarkDown](){target=_blank}

## :simple-openai: Prompt Writing

### **Types**

ChatGPT asks for a message to begin its conversation. These messages are called "Prompts". 

Begin a conversation with a specific type of prompt. This will help narrow the potential range of responses and improve results to subsequent prompts. 

We are specifically working with ChatGPT in this section, but the same prompt types and traits can be used in all other LLMs.

??? Tip "ChatGPT :simple-awesomelists: Awesome Lists"

    There is an ever changing meta-list of :simple-awesomelists: Awesome lists curated around ChatGPT plugins and extensions.

    [:simple-github: search: `chatgpt+awesome`](https://github.com/search?q=awesome-chatgpt+&type=repositories&s=stars&o=desc){target=_blank}

    Check out lists around:

    * [:simple-awesomelists: ChatGPT Prompts](https://github.com/f/awesome-chatgpt-prompts){target=_blank}
    * [:simple-awesomelists: API plugins, extensions, & applications](https://github.com/humanloop/awesome-chatgpt){target=_blank}

**Role-based**

Set the role for ChatGPT to play during your session. 

"I want you to act as ..." will establish what type of conversation you are planning to have. 

Examples of roles you might ask for are: a domain science expert, an IT or DevOps engineer, software programmer, journal editor, paper reviewer, mentor, teacher, or student. You can even instruct ChatGPT to respond as though it were a Linux [terminal](https://www.engraved.blog/building-a-virtual-machine-inside/){target=_blank}, a web browser, a search engine, or language interpreter.

??? Abstract "ChatGPT as a Research Software Guru"

    Let's try an example prompt with role-playing to help write code in the R programming language.

    ```markdown
    I want you to act as a research software guru with complete knowledge of the R language 
    and its libraries in the TidyVerse and the integrated development environment RStudio. 
    
    Please output any code results in R as MarkDown syntax code blocks in R MarkDown format 
    Ideally I would like R code to be written in RMD or Quarto syntax. 
    It is okay to insert BASH or Linux commands into R to install system dependencies for libraries.

    I want you to write the code required to plot the regression of body mass, 
    bill length, and width for the species of Penguins in the Palmer Penguins dataset. 
    You will need to download the Palmer Penguins dataset and then create the RMD notebook.
    ```

    Example can use `GPT-3.5-Turbo` or `GPT-4`

**Question and Answer**

Prompts which return informative responses to questions like "What is ..." or "How does ..."

Because of ChatGPT's proclivity at making up information, using it without a way of validating the authenticity of its responses makes it less trustworthy than regular search engines. 

Bing and Bard fill an important space in these types of prompts - they return websites which match the query criterion and allow you to research your own answers.

There are extension tools for ChatGPT which allows you to prompt with references.

!!! Tip "Grant ChatGPT access to the Internet"

    By default, ChatGPT does not have access to the Internet, and is limited to the time period before September 2021 (as of mid-2023) for its training data time frame. 

    There are extension tools, like [WebChatGPT](https://www.webchatgpt.app/) which you can install in your browser (Firefox or Chrome), that will extend ChatGPT's reach to the internet.

    What you're actually doing with this extension is automating the creation of a much larger promt message, which includes hyperlinks to resources on the internet.

**Instructional**

You can also ask ChatGPT to explain complex topics or to act as a cook-book step-by-step guide. 

ChatGPT can provide instructional details about how to do specific tasks. 

??? Abstract "ChatGPT as a documentation writer"

    ```markdown
    I want you to act as a DIY expert. You will help me develop the skills necessary 
    to complete simple lab documentation, create tutorials and guides for beginners and experts, 
    and explain complex concepts in layman's terms using visual techniques, and develop helpful resources.

    I want you to create a tutorial for building and deploying a github.io website using the MkDocs Material Theme
    ```

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

??? Danger "Indirect Prompt Injection and Malware"

    One of the risks of allowing LLMs and GPTs to access our personal documents and email clients involves the use of malware and malicious attacks.

    [Indirect prompt injection](https://www.wired.com/story/chatgpt-prompt-injection-attack-security/){target=_blank}

## :simple-openai: Software Development

ChatGPT is trained on langauges, including software language. Use ChatGPT as your new paired-programming AI assistant. 

:material-run-fast: Go to our lesson on  [:octicons-copilot-48: GitHub CoPilot](github_copilot.md)

For novice programmers, ChatGPT likely fills a long unfilled hole in your knowledge map. It can write code faster than you can, and with the proper prompts, create programs in minutes which may have taken you hours or days. 

??? Abstract "ChatGPT as Data Scientist"

    ChatGPT is trained on common data science languages, like Python, Julia, and R. Use ChatGPT to help develop basic code or to explain and debug code you're trying to write. 

    Using ChatGPT can be a time savings, reducing the time it takes to look for the answers yourself over conventional search.

    ```markdown
    I want you to act as a humble data scientist who works a lot with Python and scientific visualization

    Create a Python script which generates a visually pleasing and compelling heat map for a CSV dataset
    ```

    You can also use it to summarize code or to help explain its operation

    ```markdown
    I want you to act as a humble data scientist who works a lot with Linux 

    Explain to me what the following code does:

    $ find /home/www \( -type d -name .git -prune \) -o -type f -print0 | xargs -0 sed -i 's/subdomainA\.example\.com/subdomainB.example.com/g'
    ```

    Other valuable uses:
    
    * Change variable names and file names! When you have a large dataset with many files and folder names, you can ask ChatGPT to help design a schema for renaming your project's content

    * Regular Expressions, or `regex` is a bane of many programmers. ChatGPT can write, edit, and explain complex `regex`

    ```markdown
    I want you to act as a regex generator. Your role is to generate regular 
    expressions that match specific patterns in text. You should provide the regular 
    expressions in a format that can be easily copied and pasted into a regex-enabled 
    text editor or programming language. Do not write explanations or examples of 
    how the regular expressions work; simply provide only the regular expressions themselves. 

    remove any numbers from a string and replace them with a capital X
    ```

For more advanced programmers, ChatGPT's weaknesses may become apparent when optimizing or linting complex code bases. However, there are already extension tools which can evaluate code performance and make changes or suggestions. 

??? Abstract "ChatGPT as DevOps"

    ChatGPT can automate tasks and write tests

    ```markdown
    I want you to act as a DevOps engineer who specializes in SQL and Docker.

    I am running an Ubuntu 22.04 server with a dockerized web service which appears to have a memory leak. Write a unit test for the PostgreSQL web server using SQL, JSON, or Python that can find the process which is causing the leak and restart the docker-compose service.
    ```

    You can also use ChatGPT to help optimize your code's performance.

    ```markdown
    Make this code run faster and use less memory using BASH

     ```
     import os 
     # folder path
     dir_path = os.getcwd()
     # list to store files
     res = [] 
     # Iterate directory
     for path in os.listdir(dir_path):
         # check if current path is a file
         if os.path.isfile(os.path.join(dir_path, path)):
             res.append(path)
     print(res)
     ```
    ```

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

??? Abstract "Research scholarly articles"

    With the [WebChatGPT](https://www.webchatgpt.app/) Chrome or FireFox extension enabled, ChatGPT can search websites for content to questions.

    What is really happening is that WebChatGPT is annotating your prompt upon execution with a list of web search results which match your prompt question.

    ```markdown
    /site:scholar.google.com,https://users.math.yale.edu/mandelbrot/webbooks/wb_multi.html

    I want you to respond as though you are the mathematician Benoit Mandelbrot

    Explain the relationship of lacunarity and fractal dimension for a self-affine series
    ```


Again, this is no guarantee that the results ChatGPT provides are factual, but it does greatly improve the odds that they are relevant to the prompt. Most importantly, these extensions provide citations for their results, allowing you to research the results yourself. 
