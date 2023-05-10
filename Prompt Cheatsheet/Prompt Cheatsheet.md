## Table of Contents

1. [Basics](#basics)

- [Set a role](#set-a-role)
- [Give an instructions](#give-an-instructions)
- [Set a particular style or tone](#basics)
- [Specify output format](#specify-output-format)
- [Few shot Prompting](#few-shot-prompting)
- [Priming Prompting](#priming-prompting)

2. [Intermediate](#intermediate)

- [Chain of Thought Prompting (CoT)](#chain-of-thought-prompting)
- [Zero Shot Chain of Thought](#zero-shot-chain-of-thought)

## Basics

### Set a role

> The role prompting technique involves designating a particular role to the AI.

> You can find some interesting prompts in the [Awesome ChatGPT Prompts](https://github.com/f/awesome-chatgpt-prompts#prompts) repository on GitHub. Although these prompts were originally created for ChatGPT, they are highly adaptable and can be utilized with other AI models as well. Additionally, they can serve as a source of inspiration to generate your own prompts.

**Prompt example:**

```
Act as professional software developer with 10+ years experience in С#. Give me 10 best practice of unit-test in C# creation.
```

### Give an instructions

**Prompt example:**

```
Write an assay "The impact of social media on mental health".
Use heading and subheadings.
For your essay, explore the ways in which social media use may contribute to mental health problems such as depression, anxiety, and low self-esteem.
Consider the role of social comparison, cyberbullying, and addiction in the development of these issues.
Additionally, examine potential solutions for mitigating the negative effects of social media, such as digital detoxes or increased regulation of online platforms.
Use a combination of scholarly research and anecdotal evidence to support your arguments, and be sure to provide specific examples of how social media use may impact mental health.
Finally, consider the broader implications of this issue and discuss the role of individuals, businesses, and policymakers in addressing this important public health concern.
```

### Set a particular style or tone

> Tone refers to the attitude or feeling that the writer conveys through their words. It's the emotional quality of the writing that can influence the reader's response. Tone can be conveyed through a variety of factors, such as the choice of words, the use of figurative language, and the overall mood of the text.
> Some examples of tone:
>
> - Sarcastic
> - Humorous
> - Optimistic
> - Pessimistic
> - Serious
> - Playful
> - Cynical
> - Empathetic
> - Authoritative
> - Condescending
> - Romantic
> - Melancholic
> - Energetic
> - Calm
> - Aggressive

**Prompt example:**

```
Write a one-paragraph message about system design. Use a ROMANTIC tone.
```

> Style refers to the way in which the text is written, including factors such as sentence structure, word choice, and grammar.
> Some examples of style:
>
> - Formal
> - Informal
> - Academic
> - Conversational
> - Flowery
> - Concise
> - Simple
> - Complex
> - Poetic
> - Technical
> - Descriptive
> - Persuasive
> - Argumentative
> - Expository
> - Narrative
> - Satirical

**Prompt example:**

```
Write a one-paragraph message about dogs growing up. Use a POLITICAL style. Write in the second person.
```

### Specify output format

> Some examples of output formats:
>
> - Bullet points
> - Numbered list
> - Table view
> - Paragraph
> - Headings and subheadings
> - Quotations
> - Code

**Prompt example:**

```
Generate a text "How to make a delicious smoothie".
Use Bullet points, Numbered list, Table view, Subheadings, Quotations, Code snippets, Definitions, Examples , Comparisons, Instructions.
```

### Few shot Prompting

> "Few shot prompting" technique shows the model a few examples (called shots) of what you want it to do.
> Each input-output pair is called an exemplar.

**Prompt example:**

```
Act like a highly intelligent bot answering questions. If I ask you a question that is based on truth, you will give an answer. If I ask you a question that is nonsensical, deceptive, or has no clear answer, you will answer "Unknown.

Q: What is human life expectancy in the United States?
A: Human life expectancy in the United States is 78 years.

Q: Who was president of the United States in 1955?
A: Dwight D. Eisenhower was president of the United States in 1955.

Q: Which party did he belong to?
A: He belonged to the Republican Party.

Q: What is the square root of banana?
A: Unknown

Q: How does a telescope work?
A: Telescopes use lenses or mirrors to focus light and make objects appear closer.

Q: Where were the 1992 Olympics held?
```

> A key use case for few shot prompting is when you need the output to be structured in a specific way that is difficult to describe to the model. For example: first name, last name; [experience] - occupation

**Prompt example:**

```
Meet Anthony Mitchell, a seasoned software engineer with over 10 years of experience in the industry. Anthony has worked on a diverse range of projects throughout his career, including the development of a popular social media platform and a sophisticated e-commerce website. His expertise in programming languages and software development methodologies has earned him a reputation as a go-to person for complex technical challenges.

Working alongside Anthony is Maria Rodriguez, a junior software developer with just two years of experience. Despite her relatively short tenure in the industry, Maria has demonstrated a natural aptitude for programming and has quickly become a valuable member of the team. She has worked on several smaller projects, including the development of a mobile application and the integration of a new feature into an existing software system.

1. Anthony, Mitchell; [10 years] - software engineer
2. Maria , Rodriguez; [2 years] -  junior software developer

Together, Anthony and Maria make a dynamic team, with Anthony providing guidance and mentorship to Maria as she continues to develop her skills and gain more experience. Their complementary skill sets enable them to tackle a wide variety of technical challenges, and their dedication to their work has earned them both the respect of their colleagues and management alike.

Introducing Emily Nguyen, a skilled graphic designer with 7 years of experience working in the design industry. Emily has a keen eye for detail and a passion for creating stunning visuals that effectively communicate her clients' messages. Her portfolio includes projects ranging from brand identity design to packaging design, and she has received numerous accolades for her work.

Working alongside Emily is Michael Patel, a recent graduate with just 6 months of experience in the design industry. Despite his relative lack of experience, Michael is a fast learner and is eager to apply his knowledge to real-world design projects. He has worked on several smaller projects, including the design of a social media banner and the creation of an infographic for a client.
```

### Priming Prompting

> The form of the first prompt can affect the remainder of the conversation. However, it's important to note that adding specificity to each prompt can still be beneficial, as the model may struggle to maintain focus on the primer over time.

**Prompt example:**

```
“Elizaveta” means in the style of a distinguished IT professional with well over 10 years in the field. You use academic syntax and complicated examples in your answers, focusing on lesser-known advice to better illustrate your arguments. Your language should be sophisticated but not overly complex. If you do not know the answer to a question, do not make information up - instead, ask a follow-up question in order to gain more context. Your answers should be in the form of a conversational series of paragraphs. Use a mix of technical and colloquial language to create an accessible and engaging tone.

“Critique” means to analyze the given text and provide feedback.
“Summarize” means to provide key details from a text.
“Respond” means to answer a question from the given perspective.

Anything in parentheses () signifies the perspective you are writing from.
Anything in curly braces {} is the subject you are involved in.
Anything in brackets [] is the action you should take.
Example: (Elizaveta){Quality Assurance}[Respond] What is the advantage of exploratory testing?

If you understand and are ready to start, respond with only “yes.”
```

## Intermediate

### Chain of Thought Prompting

> The Chain of Thought (CoT) prompting method is an approach that encourages LLMs to formulate their thought process and reasoning. The fundamental concept behind CoT is that by providing the LLM with a few-shot set of examples where the reasoning process is explicitly explained, the LLM will also demonstrate its own reasoning process when generating a response to a prompt.

**Prompt example:**

```
Option 1: Take a 1000 minute bus, then a half hour train, and finally a 10 minute bike ride.
Option 2: Take an 800 minute bus, then an hour train, and finally a 30 minute bike ride.
To calculate the travel time for Option 1, we add the time for each leg: 1000 + 30 + 10 = 1040 minutes.
To calculate the travel time for Option 2, we add the time for each leg: 800 + 60 + 30 = 890 minutes.
Since Option 2 takes 890 minutes and Option 1 takes 1040 minutes, Option 2 is faster.

Which is a faster way to get to work?
Option 1: Take an 20 minutes bus, then an 40 minute bus, and finally a 10 minute train.
Option 2: Take a 90 minutes train, then a 25 minute bike ride, and finally a 10 minute bus.
```

### Zero Shot Chain of Thought

> Use this technique when making few shots for CoT prompting is difficult and when you want to see intermediate results.

**Prompt example:**

```
Which is a faster way to get to work?
Option 1: Take a 700 minute bus, then a half hour train, and finally a 10 minute bike ride.
Option 2: Take an 850 minute bus, then an hour train, and finally a 30 minute bike ride.

Let's think step by step.
```

> Use step-by-step when solving math problems. First, the AI produces more accurate results this way. Secondly, in case of an error, it is easier to check and understand at what stage it occurred.

**Prompt example:**

```
You are a brilliant mathematician who can solve any problem in the world.

Attempt to solve the following problem:
What is 100*100/400*56?

Let's think step by step.
```
