# 🦜️🔗 LangChain

⚡ Building applications with LLMs through composability ⚡

In autogpt's agent.py, the lastest replies got append to both `memory` and `full_message_history`, so when we retrieve memory, we often got the same messages in message history, which is inefficient.

I modified it so that only when message history exceed 1000 words, the oldest messages will be pop and appended to memory.
