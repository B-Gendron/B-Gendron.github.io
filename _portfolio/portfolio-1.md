---
layout: archive
title: "Meta-Learning for Emotion Detection in Conversational Context"
collection: portfolio
---

_Master Thesis_  
_From March to August 2023_  
_Supervision: University of Luxembourg, LORIA (Nancy, France) by [Gaël Guibon](https://gguibon.github.io/)_

<style>
    form button {
        background-color: #4CAF50; /* Green background color */
        color: white; /* White text color */
        padding: 10px 15px; /* Padding inside the button */
        border: none; /* No border */
        border-radius: 5px; /* Rounded corners */
        cursor: pointer; /* Cursor style on hover */
    }

    /* Style for the second button */
    form:nth-child(2) button {
        background-color: #008CBA; /* Blue background color */
    }
</style>

<td>
    <nobr>
<form style="float: left; width=150px; margin-right: 10px" action="https://B-Gendron.github.io/files/Master_thesis.pdf" method="get" target="_blank"><button type="submit">PDF</button></form> 
<form style="float: left; width=150px; margin-right: 10px" action="https://B-Gendron.github.io/files/ref_mt.txt" method="get" target="_blank"><button type="submit">Cite</button></form>
    </nobr>
</td>

## Abstract
<!-- > <img align="center" width="35" height="20" src="https://logos-marques.com/wp-content/uploads/2021/03/GitHub-Embleme.png"/>  All the code for this project is publicly available. Feel free to explore [the Git repository](https://github.com/B-Gendron/meta_dyda)! -->
 
In this work, we use a deep learning-based meta-learning model to predict emotions in conversations. For this purpose, we have built utterance representations that take into account their conversational context. By adding such information, we aim to ensure the relevance of predictions, as well as good generalization to previously unseen dialogues and emotions.  

The main goal is to use deep learning models based on meta learners to produce accurate emotion predictions in user generated conversations. At the best of our knowledge, the latest methods that use meta-learning to do Emotion Recognition in Conversation (ERC) do not integrate the conversational context. The goal of this Master Thesis is therefore to adapt existing methods, not only metric-based meta-learning approaches, but also all kinds of meta-learning schemes. The first step is to review some existing meta-learning approaches and then continue to look for a good method to integrate the conversational context into a meta-learning framework.

From a technical point of view, the aim is to develop and test alternative approaches that have not been previously considered, making this a research assignment with development phases. It therefore consists in numerous explorations and modifications of deep learning models. The final model will not necessarily have to obtain the best results, since the goal is to provide a baseline for meta-learning on ERC.
