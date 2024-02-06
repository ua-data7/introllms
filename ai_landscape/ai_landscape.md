## AI landscape

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.

!!! info "Language Model Family Tree"

    [![tree](assets/tree.jpeg){width=800}](https://arxiv.org/abs/2304.13712){target=_blank}
    
    Image Credit: [Yang et al. :simple-arxiv:](https://arxiv.org/abs/2304.13712){target=_blank} examine the history of LLMs 

**Table**: Dominant LLM models currently in public use

| Name | Creator | Application | Access | Publications |
|------|---------|-------------|--------|--------------|
| [:llama: LLaMa](https://github.com/facebookresearch/llama){target=_blank} | [:simple-meta: Meta]() | LLM | by request | [:simple-github: facebookresearch/llama](https://github.com/facebookresearch/llama){target=_blank}, [(Touvron et al. :simple-arxiv:)](https://doi.org/10.48550/arXiv.2302.13971){target=_blank} | 
| [Segment-Anything](https://segment-anything.com/) | [:simple-meta: Meta]() | Computer Vision | free |[:simple-github: facebookresearch/segment-anything](https://github.com/facebookresearch/segment-anything){target=_blank}, [(Kirillov et al. :simple-arxiv:)](https://doi.org/10.48550/arXiv.2304.02643){target=_blank} |
| [:material-lambda: LaMDA](https://blog.google/technology/ai/lamda/){target=_blank} | [:simple-google: Google](https://aitestkitchen.withgoogle.com/) | LLM | by request | [(Thoppilan et al. :simple-arxiv:)](https://arxiv.org/abs/2201.08239){target=_blank} | 
| [BARD](https://bard.google.com/){target=_blank} | [:simple-google: Google](https://bard.google.com/){target=_blank} | Search, chat | free |
| [:material-microsoft-bing: Bing](https://www.bing.com/){target=_blank} | [:simple-microsoft: Microsoft](){target=_blank} | Search, chat | free | |
| [ChatGPT](https://chat.openai.com/chat){target=_blank} | [:simple-openai: OpenAI](https://openai.com/){target=_blank} | Chat | free, subscription |
| [DALL·E](https://labs.openai.com/){target=_blank} | [:simple-openai: OpenAI](https://openai.com/){target=_blank} | Computer Vision, Chat | free | [:simple-github: openai/DALL-E](https://github.com/openai/DALL-E){target=_blank}, [(Ramesh et al.:simple-arxiv:)](https://doi.org/10.48550/arXiv.2102.12092)
| [Megatron-Turing NLG](https://developer.nvidia.com/megatron-turing-natural-language-generation){target=_blank} | [:simple-nvidia: NVIDIA](https://developer.nvidia.com/megatron-turing-natural-language-generation){target=_blank} | LLM | by request | [:simple-github: NVIDIA/Megatron-LM](https://github.com/NVIDIA/Megatron-LM){target=_blank}, [(Shoeybi et al. :simple-arxiv:)](https://doi.org/10.48550/arXiv.2201.11990){target=_blank} | 


## Image Analysis

??? Tip "Stable Diffusion & Image Segmentation Models"

    **Stable Diffusion**

    [Stable Diffusion](https://huggingface.co/CompVis){target=_blank} was released by the [CompVis Lab](https://ommer-lab.com/){target=_blank} group at [Ludwig Maximilian University of Munich](https://www.lmu.de/de/index.html){target=_blank}. 

    Stable Diffusion models are available via [HuggingFace](https://huggingface.co/CompVis){target=_blank}

    Diffusion models have two modes, forward and reverse. Forward diffusion adds random noise until the image is lost. Reverse diffusion uses Markov Chains to recover data from a Gaussian distribution, thereby gradually removing noise.

    Stable Dffusion relies upon [Latent Diffusion Model (LDM) (:simple-arxiv:)](https://doi.org/10.48550/arXiv.2112.10752){target=_blank}

    **Example Image Generation Models**

    [DALL·E](https://labs.openai.com/){target=_blank} uses GPT to create imagery from natural language descriptions

    [MidJourney](https://www.midjourney.com/){target=_blank} uses a proprietary machine learning technology, believed to be stable diffusion, along with natural langauge descriptions in the same way as DALL·E and Stable Diffusion models. MidJourney is only available via Discord, and requires a subscription for premier access after a 30-day free trial.

    [Segment-Anything (Meta)](https://segment-anything.com/){target=_blank}, [Kirillov et al. :simple-arxiv:](https://doi.org/10.48550/arXiv.2304.02643){target=_blank}, is a recently released image and video segmentation technology that allows you to 'clip' a feature from an image with a single click. 

    **Example Video Generation and Segmentation Models**

    [Project AIRA (Meta)](https://about.meta.com/realitylabs/projectaria/){target=_blank} 

    [AIRA datasets](https://about.meta.com/realitylabs/projectaria/datasets/){target=_blank}

Meta's [Segment Anything](https://segment-anything.com/) can instantly identify objects in complex images and videos. Built on the SA-1B dataset, one of the largest image segmentation datasets ever publicly released, it saves technicians time and helps generate new training datasets for more refined computer vision model development.

??? Info "Understanding Embeddings"

    [What are Embeddings? - Vicki Boykis](https://vickiboykis.com/what_are_embeddings/){target=_blank} - [download PDF :fontawesome-regular-file-pdf:](https://raw.githubusercontent.com/veekaybee/what_are_embeddings/main/embeddings.pdf)
    
    Embedded space for geospatial applications:
    
    <blockquote class="twitter-tweet"><p lang="en" dir="ltr">Visualizing how embeddings can organize satellite imagery. Millions of points covering the state of Alabama move between their geographic position and their location in the embedding space. <a href="https://t.co/Z6FtoMQ84B">pic.twitter.com/Z6FtoMQ84B</a></p>&mdash; Caleb Kruse (@clkruse) <a href="https://twitter.com/clkruse/status/1658131846121803777?ref_src=twsrc%5Etfw">May 15, 2023</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

    Embedded space for natural language:

    [Credit: Stephen Wolfram](https://writings.stephenwolfram.com/2023/02/what-is-chatgpt-doing-and-why-does-it-work/){target=_blank}

    [![wolfram](https://content.wolfram.com/uploads/sites/43/2023/02/hero3-chat-exposition.png)](https://writings.stephenwolfram.com/2023/02/what-is-chatgpt-doing-and-why-does-it-work/)

## Programmer Q/A

[Phind.com](https://phind.com){target=_blank} - is a search engine optimized for developers and technical questions with simple explanations and relevant code snippets from the web, drawing from sources like [StackOverFlow](https://stackoverflow.com/){target=_blank}.
