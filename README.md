# Fine Tuning News Dataset

**Exploring Fine-Tuning: A Journey from General to Specific**

This exploration began with a simple question I had: How do AI prompt features in services like Google Colab’s Gemini or other AI-based prompt services deliver responses so specific to their use cases, while these models are trained on vast amounts of general data, the magic happens when they are **fine-tuned**.

### The Dataset:

For this project, I chose the **Mistral Smashed** model and created a dataset using the **Beautiful Soup** library to scrape the latest news from **Yahoo Finance**. These articles provided a wealth of information on financial markets, investments, and economic updates, which I found perfect for my experiment.
The next step was to clean the data, divide it into **train** and **test** sets, and upload the dataset to **Hugging Face's data hub**. The goal was to teach the model to respond specifically to financial news queries based on this dataset rather than using general knowledge it had from its initial training.

### The Fine-Tuning Process:

In a separate notebook, I loaded the dataset and began the fine-tuning process with the Mistral Smashed model. This part was particularly exciting because it involved watching the model evolve from providing general responses to honing in on financial insights directly relevant to the news articles I fed into it.

### The Story of Prompts:

This is where the most interesting comparison comes in. I’ve always been fascinated by how AI models can be prompted to give answers suited to specific tasks. In the past, when I would prompt a base model with financial questions, the responses were broad, filled with generic knowledge about the industry. While informative, they lacked the **specificity** I wanted.
After fine-tuning the model with my dataset, the difference in the responses was stark. Suddenly, instead of receiving generic answers about the financial world, the model began responding with insights and details that directly correlated to the news articles I had scraped from Yahoo Finance. The model wasn’t just spitting out pre-trained data; it was delivering **context-specific answers** based on the **latest financial news**.

### The Power of Fine-Tuning:

This experiment reinforced how fine-tuning allows a model to move beyond general knowledge into specialized domains. For example, prompting the base model with "What are the key market movements today?" resulted in a vague, historical answer, while prompting the **fine-tuned model** generated a response based on the **latest news**—covering topics like recent stock market movements, the economic impact of certain global events, or major company announcements.
By aligning the model’s knowledge with my dataset, I effectively created a financial news expert out of the Mistral Smashed model.

### Why This Matters:

This experiment taught me how crucial fine-tuning is in the evolution of AI services. Every business, every industry has unique datasets, and general-purpose models, while impressive, often need that extra layer of training to meet specific needs. Whether it's finance, healthcare, or any other specialized sector, fine-tuning ensures that AI can become a real asset, providing tailored insights and responses.
I encourage anyone who has wondered how these AI-based services deliver such specialized answers to try fine-tuning a model themselves. It’s an eye-opening process that transforms a generalist into an expert in whatever field or dataset you provide.
If you're interested in learning more, the code and process I used for this project are documented in my latest blog, along with a comparison of the **base model** vs. the **fine-tuned model** results.

***MODEL ANSWERS***

**Prompt** 

Provide a concise summary of the following article, this is latest article from Yahoo, this is the news about stocks and comments from the business leaders. Please give sentiments of the stock or crypto currency mentioned in the article, users should be able to tell if that is a good opportunity to invest or should they backout?
Provide the summary in bullet points.

**Question**

What did Mark Cuban said in the latest news? 

**Base Model Generated Answer**

- Mark Cuban, billionaire entrepreneur and Dallas Mavericks owner, shared his thoughts on the stock market and cryptocurrencies in a recent interview.
- Cuban expressed his belief that the stock market is in a "melt-up" phase, meaning it's experiencing a rapid and sustained upward trend. He believes this trend will continue until it's no longer sustainable, at which point there will be a significant correction.

**Fine Tuned Model Answer**

- Mark Cuban, the billionaire entrepreneur and Dallas Mavericks owner, expressed his bullish outlook on Bitcoin (BTC) and Ethereum (ETH) in a CNBC interview.
- He believes that Bitcoin and Ethereum are here to stay and that they will continue to be a part of the financial system.
- Cuban also mentioned that he owns some Bitcoin and Ethereum, and he encourages others to educate themselves about these digital assets.
