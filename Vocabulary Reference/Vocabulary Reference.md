# Vocabulary Reference

**Large language model (LLM)** is a term that refers to AI models that can generate natural language texts from large amounts of data. See [learn.microsoft.com](https://www.linkedin.com/in/elizaveta-shavlova/)

**Labels** are marks we use labels to teach model how to recognize different things. For example, if we want the model to learn how to recognize pictures of animals, we show it many pictures and tell it which ones are dogs, cats, birds, and so on. We put labels on these pictures so the computer knows what each picture represents.

**Labelspace** in ML is like a special place where we put labels or tags on things to help a computer understand what they are.

_Example of Labels within Labelspace:_

    Level 1: Labelspace
    ┌─────────────┐
    │   Animal    │
    └─────────────┘

    Level 2: Labels within Labelspace
    ┌─────────────┐
    │    Dog      │
    ├─────────────┤
    │    Cat      │
    ├─────────────┤
    │    Bird     │
    └─────────────┘

    Level 3: Instances or Data Points
    ┌─────────────┐
    │  Dog Image  │
    ├─────────────┤
    │  Cat Image  │
    ├─────────────┤
    │  Bird Image │
    └─────────────┘

**Gold labels** refer to the ground truth labels assigned to instances in a dataset. In supervised machine learning, during the training phase, a dataset is typically labeled with these gold labels, indicating the correct or desired output for each instance. These labels serve as a reference or benchmark for training the machine learning model to make accurate predictions or classifications.

For example:

    Level 1: Labelspace
    ┌─────────────┐
    │   Animal    │
    └─────────────┘

    Level 2: Labels within Labelspace
    ┌─────────────┐
    │    Dog      │
    ├─────────────┤
    │    Cat      │
    ├─────────────┤
    │    Bird     │
    └─────────────┘

    Level 3: Instances or Data Points with Gold Labels
    ┌─────────────┬─────────────┐
    │  Dog Image  │   Gold: Dog │
    ├─────────────┼─────────────┤
    │  Cat Image  │   Gold: Cat │
    ├─────────────┼─────────────┤
    │  Bird Image │  Gold: Bird │
    └─────────────┴─────────────┘
