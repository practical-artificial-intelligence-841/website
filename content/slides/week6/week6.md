---
marp: true
draft: true
theme: uncover
headingDivider: 2
paginate: true
style: |
  section {
    text-align: left;
    font-size: 28px;
  }
  ul, ol, li {
    margin-left: 0;
  }
  h2 {
    font-size: 110%;
    color: #0000DD;
  }

_class:
 - lead
 - invert
---

# Transformer Models
COMP 741/841 Week 5
Fall 2023

## Agenda

- Presentations (15 min)
- Reading notes feedback (5 min)
    - References and citations
    - Quoting
- Lab 4: Transformers(50 min)
- Due next week (5 min)

## Presentations

##### RN

- Ananthaswamy, Anil. 2020. “AI’s next Big Leap.” _Knowable Magazine | Annual__Reviews_ , 2020. https://knowablemagazine.org/article/technology/2020/what-is-neurosymbolic-ai
- Roose, Kevin. 2022. “We Need to Talk About How Good A.I. Is Getting.” _The_New York Times_ , August 24, 2022, sec. Technology. https://www.nytimes.com/2022/08/24/technology/ai-technology-progress.html.

##### Presenters

- M2: Neerajaand Naveen
- M1: Rani and Pradeep
- M4: Karthik and Akhil
- M3: Shireeshaand Shravani

## RN Feedback: References and Citations

##### Reference writing style : ACM style

- Name. Year. Article title. Publication/source name. Optional: pages, URL.
    If journal/magazine: volume, number, exact date.
- Examples:
    - Henry A. Kautz, Bart Selman, and Michael Coen. 1994. Bottom-up design of software agents. Communications of the ACM 37, 7 (July 1994), 143–146. https://doi.org/10.1145/176789.
    - Adam Sadilekand Henry Kautz. 2012. Location-based reasoning about complex multi-agent behavior. Journal of Artificial Intelligence Research 43, 1 (January 2012), 87–133.

## RN Feedback: References and Citations

##### Reference citation style: (Last name, Year)

- Examples:
    - (Kautz et al., 1994)
    - (Sadilekand Kautz, 2012)

## Transformer Models

- Are **language models** : trained on large amounts of text in a **_self-supervised_** way
- Solve natural language processing (NLP) tasks

###### Self-supervised learning for general statistical understanding of the language

- Humans are not needed to label the data
    - Outputs are automatically computed from inputs
- Pretraining:
    - On huge amounts of data
    - Initial weights are randomly chosen
    - Takes weeks
    - The model has some statistical understanding of the language

## Transformer Models

###### Transfer learning: fine-tuning in a supervised way for specific practical tasks

- Additional training with dataset specific to a task, less time, less data, less environmental cost
- Task examples
    - predict next word based on previous words, predict missing word from a sentence

Source: Hugging Face. 2023. Transformers Models: What can they do? https://huggingface.co/learn/nlp-course/chapter1/ 


## Origin of the Transformer Model

***_In the Proceedings of the 31stConf. on Neural Information Processing Systems, 2017_***

###### Attention Is All You Need

Ashish Vaswani, Noam Shazeer, Niki Parmar, Jakob Uszkoreit, Llion
Jones,Aidan N. Gomez, Lukasz Kaiser, Illia Polosukhin

The dominant sequence transduction models are based on complex recurrent or convolutional neural networks in an encoder-decoder configuration. The best performing models also connect the encoder and decoder through an attention mechanism.**We propose a new simple network architecture, the Transformer , based solely on attention mechanisms , dispensing with recurrence and convolutions entirely. Experiments on two machine translation tasks show these models to be superior in quality while being more parallelizable and requiring significantly less time to train.**

## Origin of the Transformer Model

Our model achieves 28.4 BLEU on the WMT 2014 English-to-German translation task, improving over the existing best results, including ensembles by over 2 BLEU. On the WMT 2014 English-to-French translation task, our model establishes a new single-model state-of-the-art BLEU score of 41.8 after training for 3.5 days on eight GPUs, a small fraction of the training costs of the best models from the literature. **We show that the Transformer generalizes well to other tasks by applying it successfully to English constituency parsing both with large and limited training data.**

## Transformer Model

#### Self-supervised learning

#### Transfer learning

Source: Hugging Face. 2023. Transformers Models: How Transformers Work? https://huggingface.co/learn/nlp-course/chapter1/

## Transformer Model Architecture
##### Task-based architectures

- Encoder-only architecture
    - For sentence classification
- Decoder-only architecture
    - For text generation
- Sequence-to-sequence
    - For text generation based on translation or summarization

## Encoder Models

- Encoder models are concerned with _analyzing_ text
    - What are the main topics?
    - What is the overall sentiment?
- Trained by studying _sequences_ of words
    - Has access to context to _left and right_ of current word
    - Can 'see' the whole sentence
    - These sequences create context for the model
       - The more times the encoder is trained on a given sequence, the more likely it is to predict this sequence in the future
       - ex. "I live in New Hampshire." <-seen 5 times
       - "I live in Massachusetts." <-seen 2 times, less likely to be predicted

## Encoder Models

- Encoder models are best for
    - Sentence (zero-shot) classification
    - Sentiment analysis
    - Mask-filling (fill-in-the-blank)
- BERT is an example of an encoder-only model
Source: Hugging Face. 2023. Encoder Models https://huggingface.co/learn/nlp-course/chapter1/

## Decoder Models

- Decoder models are concerned with _generating_ text
    - Chatbots
- Similar to encoder models, decoder models study sequences of words
- Unlike encoder models, decoder models don’t “see” the entire sentence
    - Trained iteratively word by word using context from only one direction
       - "The model can't see <mask> <mask>" (where mask is "the future.")
- Decoder models are best for tasks requiring text generation
    - Only have access to context to the _left or right_ the current word –is not aware of
       full sentence
          - Can perform encoder tasks –but not as well
- GPT-2 is an example of a decoder-only model

Source: Hugging Face. 2023. Decoder Models https://huggingface.co/learn/nlp-course/chapter1/

## Sequence-to-sequence Models

- Encoder-decoder models
    - Makes use of both an encoder and a decoder
- Encoder-decodermodels are concerned with _analyzing input and generating_
    _output_
       - Translation
       - Summarization
- Encoder analyzes input and passes to decoder
    - Decoder is given starting context
       - For translation models, this could be the language being translated to
    - This is why AI summarization is easily identifiable -decoder probabilistically predicts next word based on the weights for words, sentences, phrases that are passed to it by encoder

## Sequence-to-sequence Models

- BART is an example of an encoder-decoder model

Source: Hugging Face. 2023. Sequence-to-sequence Modelshttps://huggingface.co/learn/nlp-course/chapter1/

## Hugging Face

##### Shares pretrained models and datasets

- Building a language model on trained weights reduces the carbon footprint

##### Transformers library: pipeline(<task>, model=“...”) function:

##### to directly input any text and get an intelligible answer

- Select a pretrained model fine-tuned for a particular NLP task, e.g.,

## Hugging Face

##### sentiment analysis

- Download and cache the model to create the classifier object
- Preprocess input text so the model understands it
- Pass the input text to the model
- Model computes the predictions
- Postprocess the predictions so a human understands them.

## Lab4: Transformers

- Experiments with transformer models using Hugging Face's transformers library
- Fork **lab4-transformer-models** from the GitHub course org by accepting the GitHub
classroom invitation shared in your section Discord channel
- Clone lab to your SageMaker CPU instance
- Follow instructions in README.mdto
    - setup the model **.cache**
    - create the virtual environment
- Run through the cells and experiment with the input as directed
- Read scenarios in BUSINESS-CASES.md
    - Answer the scenario questions
    - Justify your answers and reference supportive evidence in the slides and/or Hugging Face tutorial
- Version control your experiments in the notebook and completion of business cases
- Convert BUSINESS-CASES.mdto PDF and submit in Canvas under lab

## Due Next Week

###### Oct 2

- Lab4: complete the lab as instructed in README.md and BUSINESS-CASES.md
- RN5: Responsible dataset documentation and responsible AI development
- Prepare reading notes for ONE of the two assigned readings.
    - Antony Unwin, Kim Kleinman. 2021. The Iris Data Set: In Search of the Source of _Virginica_ ,
       _Significance_ , Volume 18, Issue 6, December 2021, Pages 26–
       29. https://doi.org/10.1111/1740-9713.
    - Kirkpatrick, Keith. 2023. The Carbon Footprint of Artificial Intelligence. _Communications of the_
       _ACM_ , 66, 8 (August 2023), 17-19. https://cacm.acm.org/magazines/2023/8/274925-the-
       carbon-footprint-of-artificial-intelligence/fulltext.

## Due Next Week

- Presentation slides
    - See **presentation-schedule.docx** in OneDrive for RN4 additional guidelines (if any)
    - Presenters
       - M2: Sanghavi and Chandu
       - M1: Janani and Rikitha
       - M4: Rishi
       - M3: Sanjay and Vijay