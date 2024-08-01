# Herodotus

This repository was created during my participation in the Makeathon competition organized by UniAI. It pertains to NOVA's challenge, which requested the development of a tool capable of generating knowledge from public sources.

## Our Solution

**Herodotus** is a knowledge-generation tool that gathers data from Greek newspaper news reports and correlates it with NOVA, as well as the employee using it, to produce useful information for the user.

## How it works

The user provides input data in the form of keywords related to what is being written in the press about the company NOVA. Then, he specifies the department in which he works. Herodotus applies **web scraping** on the **search page** of **Kathimerini** using the keywords entered earlier. The articles from the search results are collected and **processed** through **Cohere's API** with the LLM model to be summarized and produce a **report**. Finally, Herodotus sends this report back to the LLM model, and based on the **department** specified by the user, **knowledge** is generated on how the report could be utilized by the department.