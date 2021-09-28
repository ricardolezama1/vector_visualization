# vector_visualization

Gensim based vector visualization. The modules here are intended to format corpora into a GENSIM-friendly format. Additionally, the corpora expected is in Spanish.  

# Normalize Corpora

This contains corpora that is somewhat cleaned by running against a stopwords list.


Furthermore, the content not normalized has variations that are needless. The content here shows unnormalized vectors. This contains text that are capitalized and uncapitalized. This leads to a vector space in which China references could be made more accurate: 

![notNormalized](https://user-images.githubusercontent.com/11847222/135047875-001527f4-8abd-437f-aef1-39d2662e70b7.png)

Thus, we also need to consider normalizing terms like "China" & "china" ---> "china". I added an "string".lower() attribute line in the normalization function. This allows for a neater graph. Proper names, like "AMLO" & "amlo" (an acronym for the Mexican president) would rewrite to "amlo". 

![normalized](https://user-images.githubusercontent.com/11847222/135047832-ae216222-b396-4697-9257-f03b432ae383.png)
