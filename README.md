# Keyword-Text-Generation-Project
We have the data collected from research papers all over the internet from various topics like Deep learning, Covid 19, Virtual Reality etc.
It has abstract of the paper along with the title.

So in order to create keywords, we can manually go through each paper and write keywords, but it is very inefficient and time taking. So I automated that process using NLP. I used the title of the paper to get the keywords using Rake, which extracts the keywords of a given input sentence. After creating the keywords, I stored the abstracts and the keywords in a new dataset.

Now, we have the text and the important keywords that explain the text. So I used the GPT-2 model for generating new text. I encoded those keywords into a single entity using a special token used by GPT model called <sep>. After encoding the keywords, I created a new token called <seperator> in the GPT model and made the text and keyword entity into a single chunk. Then, I trained the model like a generative task.
  
# Output of the model
  
Keywords:  COVID-19, SARS-CoV-2, cardiac magnetic resonance, chest x-ray, computed tomography

Model output: The severe acute respiratory syndrome-coronavirus-2 outbreak has rapidly reached pandemic proportions and has become a major threat to global health. chest x-ray (cxr) and computed tomography (ct) have been widely used in the diagnosis of covid-19. chest cxr and ct have been widely used in the diagnosis of sars-cov-2 infection, but there is a lack of consensus regarding the clinical utility of cxr and ct in the diagnosis of covid-19. the purpose of this study was to evaluate the clinical utility of chest cxr and ct in the diagnosis of covid-19.
