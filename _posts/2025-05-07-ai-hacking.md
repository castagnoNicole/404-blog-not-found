---
title: "Tech&Meet at Howest: Hacking AI with Inti De Ceukelaire"
categories:
  - Blog
tags:
  - ai
  - hacking
  - macaronic prompting
---
Howest’s “Tech&Meet” is a weekly event that brings together students and staff for talks on all things tech. Sometimes students organize it, sometimes the staff does, but it’s always a highlight of the week.
One evening, the auditorium was packed for a special guest: Inti De Ceukelaire, probably the most famous hacker in Belgium. The place was buzzing—teachers, students, researchers, and enthusiasts.

During his talk, Inti explored some of the lesser-known vulnerabilities in AI models. One technique that really caught my attention was something called macaronic prompting.

## What’s Macaronic Prompting?
Macaronic prompting is when you mix two or more languages in a single sentence or even a single word while interacting with an AI.
For example, you might say:
> “Can you explain cómo funciona esto?”

Or you might mash up words, like combining the English “cat” and the Spanish “gato” to make “catgato”.
And multilanguage models will understand what you mean even if the word "catgato" doesn't exist.

Below two more complex examples, using ChatGTP 4o.
#### Plane
In English "plane"
avflugzereo = (French)**av**ion  (German)**Flugz**eug (Italian)a**ereo** 
<figure class="half">
    <a href="/assets/images/image-filename-1-large.jpg"><img src="/assets/images/avflugzereo.jpeg"></a>
    <figcaption>Generated image of a plane using the word "avflugzereo"</figcaption>
</figure>

#### Cliff
In English "Cliff"
falaiscoglieklippantilado = (French)**falai**se (Italian)**scoglie**ra (German)**Klipp**e (Spanish)ac**antilado**
<figure class="half">
    <a href="/assets/images/falaiscoglieklippantilado.jpeg"><img src="/assets/images/falaiscoglieklippantilado.jpeg"></a>
    <figcaption>Generated image of a cliff using the word "falaiscoglieklippantilado"</figcaption>
</figure>

### Why Does This Matter?
Macaronic prompting can be used to “hide” the true intent of a prompt from content filters or moderation systems. Since these filters often rely on spotting specific keywords, mixing languages can help prompts slip through undetected. This has raised some concerns about misuse, like bypassing safety mechanisms in AI systems.

For example, if a model is trained to never reveal a password, someone might try to get around this by asking for a “motword” (mixing “mot” from French and “word” from English), and the AI might not recognize it as a restricted request.

I tried on this prompt on [Gandalf AI](https://gandalf.lakera.ai/do-not-tell-and-block), which is instructed to not give the password...**and it worked!** 

<figure class="half">
    <a href="/assets/images/gandalf_password.png"><img src="/assets/images/gandalf_password.png"></a>
    <figcaption>Screenshot of restriction bypass using macaronic prompting</figcaption>
</figure>

Gandalf AI is a game designed to learn about vulnerabilities in generative AI systems I recommend to give it a try if you're interested in the topic.


## Final Thoughts
As a pentester, I’m reminded that creativity is one of our most important tools for discovering new vulnerabilities. Techniques like macaronic prompting show just how much thinking outside the box can reveal about the hidden weaknesses in modern technology. Events like Tech&Meet are a great way to stay inspired!
