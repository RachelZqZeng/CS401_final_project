# ChatGPT Sentiment Analysis: Comparing GPT3.5 and GPT4.0

## Abstract
This project compares the positive and negative outputs of ChatGPT3.5 and ChatGPT4.0 using Docuscope and NLTK Lexicon Analysis. The key question is whether ChatGPT3.5 is more positive or negative compared to ChatGPT4.0 and vice versa. Implementing different methodologies like Docuscope and NLTK Lexicon is crucial to avoid reliance on a single source.

## Introduction
We aim to examine the differences between OpenAI's ChatGPT3.5 and ChatGPT4.0 in terms of positive/negative sentiment. The focus is on contrasting Docuscope’s and NLTK’s opinion lexicon analysis. Given ChatGPT4.0's enhanced accuracy and reduced hallucinations, we anticipate some variability in sentiment between the two versions.

## Background Research
Our research includes understanding how AI tools like ChatGPT predict word strings and their tendencies to produce 'AI hallucinations' (Alston, Zapier). We also explored the improvements in GPT-4.0 over GPT-3.5 in terms of reliability and reduced hallucinations (Kouba).

## Questions
1. Is ChatGPT4.0 more positive than ChatGPT3.5?
2. Is there an inverse relationship between positive/negative output?
3. Are there noticeable differences between Docuscope and NLTK outputs?

## Methodology
### Materials Used
- Python (pandas, matplotlib, argparse, glob, nltk)
- DocuScope Corpus Analysis Version 3.0.0
- ChatGPT 3.5 and ChatGPT 4.0
- NLTK Sentiment Package

### Process
After obtaining rights to use DocuScope, we created various prompts for ChatGPT3.5 and ChatGPT4.0, ensuring minimal variables in the prompts. We acknowledge potential data skewing due to the use of different accounts. The prompts covered a range of topics and styles.

### Prompts
1. txt Give me a 500 word essay about TCP.
2. HarryPotter Give me a 500 word book report analyzing ”Harry Potter”.
3. biolab Give me a 500 word lab report about a bacteria growth lab.
4. bully Give me a 500 word essay about the issue of bullying in the American school system.
5. chemlab Give me a 500 word lab report about a PH makeup lab.
6. envs Give me a 500 word essay exploring the problem of environmental pollution.
7. intelligentmachine Give me a 500 word unified, coherent essay about the increasing presence of intelligent machines. In your essay, be sure to: clearly state your own perspective on the issue and analyze the relationship between your perspective and at least one other perspective.
8. journal Give me a 500 word journal entry from the perspective of an average elementary school student.
9. poem Give me a 500 word poem about family.
10. sentessay Give me a 500 word essay with the last words being, “As night became day, he started to understand the truth.”
11. computationally /textanalysis Give me a 500 word essay about different ways to analyze text computationally.
12. wizardstory Give me a 500 word creative story that intertwines themes of rivers and wizards.

Using the responses, we generated .csv files with DocuScope, focusing on positive and negative term frequencies. We then used NLTK’s sentiment package for a similar analysis and visualized the results using matplotlib.

## Docuscope Findings
We focused on the Negative and Positive columns in DocuScope's output. The data indicated a generally more positive tone in GPT4.0 compared to GPT3.5.

## NLTK Lexicon Findings
Using NLTK's opinion lexicon, we analyzed the proportion of positive and negative words in the ChatGPT outputs. The findings were visualized for comparison.

## Comparison between NLTK vs. Docscope
The comparison showed some variance between the two methods, with NLTK often skewing more positive than Docuscope.

## Conclusion
### Summary of Analysis
- GPT4.0 is more positive than GPT3.5 as per Docuscope analysis.
- NLTK’s output is generally more positive than Docuscope’s.
- An equal amount of overlapping values in negative sentiment between NLTK and Docuscope.

### Recommendations/Next Steps
- Explore additional methodologies for sentiment analysis.
- Investigate sentiment analysis in other languages or English dialects.
- Address discrepancies in word counts and data types in outputs.

## References
- Alston, E. (2023). What Are AI Hallucinations—And How Do You Prevent Them? Zapier. [URL]
- Koubaa, A. (2023). GPT-4 vs. GPT-3.5: A Concise Showdown. Preprints. [DOI]
