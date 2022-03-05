# «Visualization of literary techniques in *Anna Karenina* film adaptations»

This code is an essential part of my MA thesis, which was dedicated to the literary techniques’ reproduction in film adaptations of "Anna Karenina".

The problem of the fiction *"translation"* from verbal language into the language of cinema was being relevant throughout the 20th century. The most structured translation model was formulated in the 1970s by the literary critic and film semioticist Yu.M. Lotman, who wrote about the existence of a special *"system of equivalences"* that allows transforming a literary text into a visual form. The main goal of my research was the reconstruction of the *"system of equivalences"* (proposed by Lotman) for different film adaptations with the aid of statistical methods.

I used computer vision technologies as tools for working with visual material. In particular, the study of **Tolstoy's technique of repetition and parallelism of plots** was carried out using the VGG16 convolutional neural network, the initial task of which is to classify images in accordance with the objects shown on them. As a result of using this technology, I managed to cluster film frames according to which compositional patterns are used in them, as well as to trace the intensity of repetitions within the cinema narrative.

Close-up analysis, which could potentially convey **Tolstoy's attention to detail and his desire to show the characters from different angles**, was implemented using face recognition technology. Thanks to this, I could calculate the area allotted in the frame for the image of the face, as well as investigate the frequency of directors turning to close-ups, the purpose of which, first of all, is to convey the emotions of the characters.

Finally, I analyzed the thematic and lexical affinity of the novel's text and subtitles to the 1967 film. The choice of these subtitles was motivated by the fact that there are no subtitles for domestic serials. In addition, there is no sense to compare Tolstoy's text with subtitles of foreign films, since they represent a translation of the original text, and the structures of the Russian and English languages are fundamentally different. As a result, I found out what themes were common for the film and the novel, as well as how similar the text of the screenplay was to the artistic source.

## What do I have in this repository (in alphabet range):

- **AK_1967_P1.str** and **AK_1967_P2.str** - the subtitles for two parts of Anna Karenina 1967 (Soviet version of the film)
- **Anna_Karenina.txt** - the full text of Tolstoy's novel
- **Anna_Karenina_Color_Clusterization.ipynb** - trial but working code for color clusterization of shots and images in general.
- **Composition_Clusterization.ipynb** - one of the main Jupyter notebooks for my MA thesis. In this one, all films are divided into frames and all frames are clusterized in accordance with their composition and content. Unfortunately, the interactive plots don't work in Github, so below you can find the .gif with the results.
- **Face_Recognition.ipynb** - one more main Jupyter notebook for my MA thesis. Here I detect faces in the shots, count their number, choose only those frames where only one face is detected, calculate the percentage of the square which face takes in the frame, and investigate the distribution of close-ups in the films. Moreover, I define which third of the frame (left, central, or right) contains the face.
- **Frame Extraction.ipynb** - basic code allowing to divide films into frames (one frame per second, but you can change this parameter).
- **Keras&K-Means.ipynb** - trial code
- **Lemma_Token_Sub_Novel.ipynb** - lemmatization and tokenization of direct and reported speech of novel
- **Novel_Preprocessing.ipynb** - extraction of direct and reported speech from the novel and division of the novel into 8 parts
- **Scenes_Length.ipynb** - trial but working code to automatically count the length of scenes in feature Karenina adaptations
- **Sub_Intensity_and_TM.ipynb** - main Jupyter notebook for work with text aspect of 1967 movie and original source. Investigation of speech intensity in the film, similarity of subtitles and speech in novel, comparison of subtitles and novel by topics, which were developed in different parts of texts.
- **TSNE.ipynb** - trial code for dimensionality reduction of matrix
