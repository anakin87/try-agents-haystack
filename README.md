# try-agents-haystack
Trying the Agents 🕵️ --> new feature introduced in [Haystack](https://github.com/deepset-ai/haystack) 1.15.0 to make Large Language Models resolve complex queries and tasks.

---
As of release 1.15, Haystack implements Agents 🕵️!

Put simply, an Agent is a Large Language Model with a specific prompt.

Based on that prompt, the Agent can answer complex questions, by performing a sequence of steps.

At each step, the Agent (our brain 🧠) can select a Tool from its toolbox 🧰 and use it to accomplish a task.

Some examples of Tools: Web Search, calculator, several pipelines/nodes (available in Haystack)...

## Demo
https://user-images.githubusercontent.com/44616784/229845195-c2d6f5a5-8354-4816-aa21-6e29c06b149f.mp4


In the video, you see the Agent in action with the task of answering questions about books on my reading list.

* I uploaded a CSV containing a minimal reading list 📚
* I initialized two Tools ⚒️:
    * A Question Answering component to answer questions about my reading list
    * A Search tool 🔎🌐, which can browse the web and find information
* I defined an Agent, based on Davinci model and equipped with the Tools defined above.
* Now I can ask complex questions, such as "Can you provide me with information on the shortest book on my reading list, including author and price on Amazon?""

🚀

Currently, Agents work great with OpenAI Davinci model.
Soon, open-source models will also be supported, so you can have the power of LLM at your disposal without giving up your data!

## More information
### Agents in Haystack
- [Introducing Agents in Haystack: Make LLMs resolve complex tasks](https://haystack.deepset.ai/blog/introducing-haystack-agents) by Tuana Çelik
- [Tutorial: Answering Multihop Questions with Agents](https://haystack.deepset.ai/tutorials/23_answering_multihop_questions_with_agents)
- [Haystack documentation: the Agent](https://docs.haystack.deepset.ai/docs/agent)

### Papers
- [ReAct: Synergizing Reasoning and Acting in Language Models](https://arxiv.org/abs/2210.03629)
- [MRKL Systems: A modular, neuro-symbolic architecture that combines large language models, external knowledge sources and discrete reasoning](https://arxiv.org/abs/2205.00445)
