# Artificial Intelligence (AI) By - SAI CHARITH PUTTABAKULA 
This is my class Work for AI by Akshay Saini

# Episode 1 : The Evolution of AI

> Notes summary from **Namaste AI Notes — Season 1, Episode 02: The Evolution of AI**.

## Overview

This episode traces the development of Artificial Intelligence (AI), from early rule-based systems to Machine Learning, Deep Learning, Transformers, Generative AI, and Agentic AI.

AI is described as the science of making machines perform tasks that normally require human intelligence, such as recommending content, recognizing images, understanding language, and generating text or media.

## 1. History and Key Milestones

| Year / Period | Milestone | Key idea |
|---|---|---|
| 1950 | Alan Turing and the Turing Test | A way to evaluate whether a machine's conversational responses can be distinguished from a human's. |
| 1956 | John McCarthy | The term **Artificial Intelligence** was introduced. |
| 1950s–1980s | Rule-Based AI | Systems used predefined rules and `if/else` conditions to make decisions. |
| 1987–1993 | AI winter (as stated in the notes) | A period when interest and activity in AI declined. |
| 1990s | Machine Learning | Systems increasingly learned patterns from data rather than relying only on manually written rules. |
| 1997 | IBM Deep Blue | Defeated chess champion Garry Kasparov. The notes clarify that Deep Blue relied heavily on search and move evaluation rather than being a modern learning-based AI system. |
| 2000s | Deep Learning | Neural networks became increasingly useful for learning complex patterns. |
| 2012 | AlexNet / ImageNet | A major milestone in deep-learning-based image classification. |
| 2016 | AlphaGo | Defeated Go champion Lee Sedol. |
| 2017 | Transformers | The paper *Attention Is All You Need* introduced the Transformer architecture. |
| November 2022 | ChatGPT | Conversational generative AI became widely accessible to the public. |
| 2025 onward | Agentic AI | Growing focus on AI systems that can use tools and perform multi-step tasks. |

## 2. Rule-Based AI

Early AI systems relied on manually written rules and conditions.

**Example:** An email filter might flag a message as spam when it contains certain words or patterns.

**Limitation:** It is difficult to write rules for every possible situation. Small changes in wording or behavior can cause rule-based systems to fail.

## 3. Machine Learning (ML)

Machine Learning enables systems to learn patterns from examples and use those patterns to make predictions.

**Example:** Train a model using labelled images of cats and dogs, then use it to classify a new image.

Typical workflow:

1. Collect and prepare training data.
2. Train a model to identify patterns.
3. Evaluate its performance.
4. Use the trained model to make predictions on new data.

## 4. Deep Learning (DL)

Deep Learning is a subset of Machine Learning that uses neural networks with multiple layers to learn complex patterns from data.

**Applications mentioned in the notes:**
- Image and face recognition
- Speech recognition
- Computer vision

The notes contrast ML and DL as follows:

| Aspect | Machine Learning | Deep Learning |
|---|---|---|
| Data volume | Often works with smaller datasets | Often benefits from very large datasets |
| Compute | Can require less computational power | Can require substantial compute, often using GPUs |
| Feature engineering | Often requires manually designed features | Can learn useful features during training |
| Training time | Often shorter for simpler models | Can be longer and more resource-intensive |
| Interpretability | Some models are relatively easy to interpret | Complex neural networks can be harder to interpret |

These are general tendencies; actual requirements depend on the model and task.

## 5. Computer Vision

Computer Vision focuses on helping machines interpret visual information.

The notes highlight:
- **ImageNet:** A large image dataset used for visual-recognition research.
- **AlexNet (2012):** A deep neural network that achieved an important image-classification breakthrough.

**Example applications:** Face recognition, driver-assistance and self-driving systems, medical image analysis, and visual product search.

## 6. Natural Language Processing (NLP)

NLP focuses on enabling computers to process and work with human language.

Language is challenging because the same phrase or word can have different meanings depending on context.

**Examples from the notes:**
- “I saw a man with a telescope” — the sentence can have more than one interpretation.
- “River bank” versus “Bank of India” — the word *bank* has different meanings in different contexts.

Techniques and architectures mentioned:
- Bag of Words
- N-grams
- RNNs (Recurrent Neural Networks)
- LSTMs (Long Short-Term Memory networks)

The notes explain that RNNs and LSTMs helped models work with sequential language, while long-range context remained challenging.

## 7. Transformers (2017)

The Transformer architecture was introduced in the research paper **“Attention Is All You Need.”**

Transformers use attention mechanisms to model relationships between tokens and help capture context across a sequence. They became a foundation for many modern language models.

**Why this matters:** Transformers made it practical to build large language models that can process context and generate coherent responses.

## 8. Large Language Models (LLMs)

LLMs are models trained on very large datasets to process and generate language. The notes connect modern LLMs to the Transformer architecture.

Important resource requirements include:
- Large training datasets
- Significant computational power
- GPUs and other specialized hardware

## 9. Generative AI

Generative AI creates new content rather than only classifying, recommending, or predicting.

**Examples:**
- Text and poems
- Software code
- Images
- Audio and video
- Documents and other content

**Multimodal AI** can work with multiple kinds of input or output, such as text, images, audio, and video.

## 10. ChatGPT and Agentic AI

### ChatGPT — November 2022

The notes identify ChatGPT's public release in November 2022 as a major moment in the adoption of conversational AI. They also mention the subsequent growth of other assistants and models.

### Agentic AI — 2025 onward

The episode describes the shift toward AI systems that can do more than respond to a single prompt. Such systems may:
- Plan and reason through steps
- Use tools and APIs
- Search for information
- Write and debug code
- Carry out multi-step workflows with varying degrees of autonomy

The degree of autonomy depends on the system's design, permissions, and safeguards.

## Quick Revision

- **AI:** Machines perform tasks that normally require human intelligence.
- **Rule-Based AI:** Decisions are driven by predefined rules.
- **Machine Learning:** Models learn patterns from data.
- **Deep Learning:** Neural networks learn complex representations.
- **Computer Vision:** Machines process visual information.
- **NLP:** Machines process human language.
- **Transformers:** Attention-based architecture foundational to many modern LLMs.
- **LLMs:** Large models trained to process and generate language.
- **Generative AI:** Creates new content.
- **Agentic AI:** Uses tools and multi-step actions to pursue a goal.

## Main Takeaway

The episode presents AI as an evolving field: from explicit rules, to learning patterns from data, to deep neural networks, to Transformer-based generative models, and increasingly to AI agents that can use tools and complete multi-step tasks.

---

# Episode 2 : Does ChatGPT Know or Does It Guess?

> Summary of the supplied Namaste AI Notes PDF: “Does ChatGPT Know or Does It Guess?”  
> Topics: Google Search vs. LLMs, response generation, knowledge cutoffs, base models, hallucinations, tools, and RAG.

## Overview

This episode explores where ChatGPT gets its answers and whether it retrieves facts or generates responses from learned patterns. It compares traditional search engines with Large Language Models (LLMs) and explains why fluent, confident AI answers can still be incorrect.

## 1. Google Search vs. ChatGPT

### Google Search: Retrieval

According to the notes, Google Search:
1. Takes a user's query.
2. Searches its index of webpages.
3. Ranks relevant pages.
4. Returns links and results that users can inspect.

A **search index** is an organized database of information about webpages. Search engines use crawlers or spiders to discover pages and update the index. Ranking can depend on factors such as relevance, links, page quality, and other signals.

### ChatGPT: Generation

An LLM generates a response based on patterns learned during training and the context available in the conversation. Rather than simply returning a webpage, it creates a new response in natural language.

**Core distinction:** Search primarily retrieves documents; an LLM primarily generates text. Search results can also be misleading or outdated, so neither approach guarantees truth.

## 2. How LLMs Generate Responses

LLMs generate text by predicting likely next tokens based on the preceding context.

**Example:** Given “The sun rises in…”, a model may predict “the east.”

The notes compare this to a sophisticated autocomplete system. Training helps the model learn patterns in language, grammar, facts, associations, and examples. Its output is influenced by probabilities and context; it is not a guarantee that every generated statement is correct.

## 3. What Knowledge Does an LLM Contain?

During training, a neural network adjusts numerical parameters (also called **weights**) to learn patterns from data. The resulting model can use these learned patterns to generate responses.

The notes emphasize that this process involves complex algorithms and that a model's answer is generated from learned patterns and available context.

## 4. Knowledge Cutoff

A model's **knowledge cutoff** is the point up to which its training data or built-in knowledge is generally current. Models are not necessarily retrained every day, and training can be computationally expensive.

A model may still answer questions about recent events when it has access to external tools, such as web search, or when relevant information is supplied in the prompt. The model's built-in knowledge and its access to current information are different things.

## 5. Base Model vs. AI Assistant

A **base model** is trained to predict the next token. On its own, it is not necessarily optimized to follow instructions or behave like a helpful assistant.

An assistant product can add capabilities around a base model, including:
- Instruction tuning and human feedback
- System instructions and conversation management
- Safety rules and content filters
- Tool calling and API access
- Web search or other external information sources

The notes use an analogy: **the base model is the engine, and the assistant is the car**.

## 6. Training vs. Inference

| Concept | Meaning |
|---|---|
| **Training** | The model learns patterns from data by adjusting its parameters. |
| **Inference** | The trained model uses the prompt and available context to produce an output. |

A simple analogy from the notes: training is the learning phase; inference is the working phase when the model answers a question.

## 7. AI Hallucinations and Fake Fluency

An **AI hallucination** occurs when a model generates information that is incorrect or unsupported but presents it as if it were factual.

The notes explain that fluent language and confident wording do not prove that an answer is true. Potential causes include:
- Insufficient or missing knowledge
- Ambiguous prompts or information
- False assumptions
- Unreliable patterns learned during training
- A tendency to produce an answer rather than acknowledge uncertainty

**Important lesson:** Language quality and factual accuracy are separate. Verify important claims, especially in medical, legal, financial, or other high-impact situations.

## 8. How to Reduce Overconfident Answers

The notes recommend asking the model to:
- Provide evidence or sources.
- State uncertainty.
- Answer only when sufficiently confident.
- Use web search or other external evidence when appropriate.

These techniques may help, but they do **not** guarantee correctness. Sources should still be checked directly.

## 9. Tools and Tool Calling

Tools extend an LLM's capabilities beyond the information present in its prompt and learned parameters. Depending on permissions and implementation, tools may include:
- Web search
- APIs and databases
- Email and calendars
- Files and internal documents
- Code execution
- Other connected services

Without the relevant tool and authorization, a model cannot automatically access private files, emails, or databases. Tool access makes an assistant more useful for specific workflows, but actions should be controlled by appropriate permissions and safeguards.

## 10. Retrieval-Augmented Generation (RAG)

**Retrieval-Augmented Generation (RAG)** combines information retrieval with language generation.

A simplified workflow:

1. A user asks a question.
2. A retrieval system searches relevant external sources.
3. Relevant passages or documents are supplied to the LLM.
4. The LLM generates an answer grounded in the retrieved material.

**Why it matters:** Retrieval can provide current or domain-specific evidence that may not be present in the model's training data. The quality of the result still depends on the sources retrieved and how accurately the model uses them.

## 11. What Information Can Influence an LLM Response?

The notes identify four main sources:
1. **Training data** — patterns learned during model training.
2. **Context** — the current conversation and supplied information.
3. **System prompt / instructions** — guidance about how the assistant should behave.
4. **Tools** — external sources or actions available to the assistant.

These components help turn a base model into a more capable assistant. Tool outputs and supplied documents can provide information beyond the model's built-in knowledge.

## Quick Revision

- **Search engine:** Finds and ranks indexed webpages.
- **LLM:** Generates text from learned patterns and current context.
- **Indexing:** Organizes webpage information so it can be searched.
- **Next-token prediction:** A central mechanism used by language models to generate text.
- **Knowledge cutoff:** The limit of the model's built-in training knowledge.
- **Base model:** The core model trained to predict tokens.
- **Training:** Learning patterns from data.
- **Inference:** Generating output with a trained model.
- **Hallucination:** Plausible-sounding but incorrect or unsupported output.
- **Tool calling:** Letting a model use external services or perform permitted actions.
- **RAG:** Retrieval plus generation, helping ground answers in external information.

## Main Takeaway

ChatGPT does not guarantee that it knows or verifies every fact it states. It generates responses from learned patterns and available context. Search, tools, and RAG can provide external evidence, but users should still verify important information rather than treating confidence or fluency as proof.

---

# Episode 3 : The Secret Language of LLMs

> Summary of the supplied Namaste AI Notes PDF: “The Secret Language of LLMs”.

## Overview

This episode explains how Large Language Models (LLMs) process text. Instead of handling text as humans read it, models process tokenized input represented by numerical token IDs. The notes cover tokenization, subwords, vocabularies, Byte Pair Encoding (BPE), multilingual tokenization, tokenization fertility, special tokens, and context windows.

## 1. What Are Tokens?

When text is sent to an LLM, a **tokenizer** breaks it into smaller units called **tokens**. These units may be whole words, parts of words, characters, or other text units, depending on the tokenizer.

For example, the sentence:

`These notes are awesome`

may be split into tokens such as:

`These` · `notes` · `are` · `awesome`

Each token is associated with a numerical **token ID**. The model processes the sequence of token IDs and predicts the next token ID, which is then converted back into text.

**Important:** One word does not necessarily equal one token.

## 2. Tokenizers and Subword Tokenization

A **tokenizer** converts text into tokens according to its vocabulary and tokenization rules. Different models can use different tokenizers, so the same text may be split differently and receive different token IDs.

**Subword tokenization** lets a tokenizer represent less-common or longer words as smaller pieces. For example, the notes show `untrustable` split into pieces such as `un`, `trust`, and `able`.

However, tokenization does not always follow grammar or meaningful word parts. The notes use `undone` as an example of a word that may be represented as one token if it exists in the tokenizer's vocabulary.

Try the tokenizer demonstrations referenced in the PDF:
- [OpenAI Tokenizer](https://platform.openai.com/tokenizer)
- [TikTokenizer](https://tiktokenizer.vercel.app/)

## 3. Vocabulary and Token IDs

A tokenizer's **vocabulary** is the collection of token units it can represent. Each token in that vocabulary maps to a token ID.

Token IDs are identifiers, not definitions of meaning. The model learns patterns from sequences of tokens during training; the numerical ID itself does not directly express the meaning of a word.

The notes mention different tokenization approaches, including:
- Byte Pair Encoding (BPE)
- WordPiece
- Unigram
- SentencePiece-based approaches

Different models and tokenizers may use different vocabularies and algorithms.

## 4. Byte Pair Encoding (BPE)

The notes describe **Byte Pair Encoding (BPE)** as a method that starts from smaller units and merges frequently occurring neighbouring pairs into larger token units.

A simplified explanation:
1. Begin with smaller text or byte-level units.
2. Identify pairs that commonly occur together.
3. Merge selected pairs into new tokens.
4. Build a vocabulary that can represent common patterns efficiently.

This approach allows token pieces to be reused across multiple words instead of requiring every possible word to have its own token.

## 5. English vs. Other Languages

The notes explain that equivalent text in different languages does not necessarily produce the same number of tokens. Tokenization depends on the text and the tokenizer's vocabulary, not simply on whether the meaning is equivalent.

The PDF compares English with Hindi and Hinglish and notes that Hinglish spellings can vary—for example, `main`, `mai`, and `maii`. Such variation can affect tokenization.

In the examples shown in the PDF, English text uses fewer tokens than the corresponding Hinglish text. This is an illustration from the supplied notes, not a rule that applies to every sentence or tokenizer.

## 6. Tokenization Fertility

**Tokenization fertility** is defined in the notes as the average number of tokens produced per word.

- **Lower fertility:** Fewer tokens are used to represent the text, which can reduce token usage and allow more text to fit within a context window.
- **Higher fertility:** More tokens are used, which can increase processing requirements and API cost and consume more of the context window.

The effect depends on the tokenizer, model, language, and text being processed.

## 7. Emojis, Code, Spaces, and Special Characters

The notes explain that emojis, punctuation, capitalization, spaces, and other text patterns can affect tokenization. A visible emoji is not guaranteed to be one token, and changing a space or adding/removing punctuation can change the token sequence and token count.

LLM conversations can also include **special tokens** used to represent message boundaries or other structural information. Their details vary across model families and formats.

## 8. System Instructions vs. User Instructions

- **System instructions:** High-level instructions that guide how an assistant should behave.
- **User instructions:** The task or question supplied by the user.

The notes explain that prompts and instructions are processed as part of the model's input, along with other context. The exact representation depends on the model and its conversation format.

## 9. Context Window

A **context window** is the amount of tokenized information a model can process within a request or active generation context.

It can include:
- System instructions
- The current user prompt
- Relevant conversation messages
- Documents and other supplied text
- Tool outputs
- Text generated by the model

The context window is shared between input and output in the way described by the notes. A larger context window does not guarantee perfect memory or accuracy, and context should not be confused with permanent chat history.

### What happens when context becomes too large?

The notes recommend:
1. Shortening or truncating unnecessary input.
2. Summarizing earlier messages.
3. Asking for the relevant information instead of including everything.
4. Splitting large projects into separate chats or modules.
5. Avoiding the assumption that every old detail will remain available in active context.

## 10. Common Tokenization Misconceptions

The final page of the PDF lists these misconceptions:

- **One token equals one word:** Incorrect.
- **Every model uses the same tokenizer:** Incorrect.
- **A token ID represents meaning:** Incorrect.
- **One visible emoji is always one token:** Incorrect.
- **A larger vocabulary is always better:** Not necessarily.
- **A larger context window means perfect memory:** Not necessarily.
- **More tokens always produce better results:** Incorrect.

The PDF also emphasizes that longer prompts do not automatically produce better answers and that token usage directly affects API costs.

## Quick Revision

| Term | Meaning |
|---|---|
| Token | A unit of text processed by a model |
| Tokenizer | Converts text into tokens |
| Token ID | Numerical identifier assigned to a token |
| Vocabulary | Collection of tokens supported by a tokenizer |
| Subword tokenization | Splitting text into smaller pieces |
| BPE | Tokenization method that merges frequent neighbouring pairs |
| Tokenization fertility | Average number of tokens per word |
| Special tokens | Structural markers used in model input/output formats |
| Context window | Maximum tokenized context the model can process at a time |

## Main Takeaway

LLMs process text through tokenization: text is split into tokens, mapped to token IDs, and processed by the model. Tokenization varies by model and language and affects token counts, cost, and how much information fits into a context window. Understanding these concepts helps when writing prompts and building applications that use LLM APIs.


