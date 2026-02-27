# AI Agent Operating System Papers Summary

## 1. AIOS: LLM Agent Operating System

**标题**: AIOS: LLM Agent Operating System

**作者**: Kai Mei, Wujiang Xu, Zelong Li, Shuyuan Xu, Ruosong Ye, Yingqiang Ge, Yongfeng Zhang

**年份**: 2024

**摘要**: 
LLM-based intelligent agents face significant deployment challenges, particularly related to resource management. Allowing unrestricted access to LLM or tool resources can lead to inefficient or even potentially harmful resource allocation and utilization for agents. Furthermore, the absence of proper scheduling and resource management mechanisms in current agent designs hinders concurrent processing and limits overall system efficiency. To address these challenges, this paper proposes the architecture of AIOS (LLM-based AI Agent Operating System) under the context of managing LLM-based agents. It introduces a novel architecture for serving LLM-based agents by isolating resources and LLM-specific services from agent applications into an AIOS kernel. This AIOS kernel provides fundamental services (e.g., scheduling, context management, memory management, storage management, access control) for runtime agents. To enhance usability, AIOS also includes an AIOS SDK, a comprehensive suite of APIs designed for utilizing functionalities provided by the AIOS kernel. Experimental results demonstrate that using AIOS can achieve up to 2.1x faster execution for serving agents built by various agent frameworks.

---

## 2. Eliza: A Web3 friendly AI Agent Operating System

**标题**: Eliza: A Web3 friendly AI Agent Operating System

**作者**: S. Walters, Sam Gao, Shakker Nerd, Feng Da, Warren Williams, Ting-Chien Meng, A. Chow, Hunter Han, Frank S. He, Allen Zhang, Mingyu Wu, Tim Shen, Maxwell Hu, Jerry C. Yan

**年份**: 2025

**摘要**: 
AI Agent, powered by large language models (LLMs) as its cognitive core, is an intelligent agentic system capable of autonomously controlling and determining the execution paths under user's instructions. With the burst of capabilities of LLMs and various plugins, such as RAG, text-to-image/video/3D, etc., the potential of AI Agents has been vastly expanded, with their capabilities growing stronger by the day. However, at the intersection between AI and web3, there is currently no ideal agentic framework that can seamlessly integrate web3 applications into AI agent functionalities. In this paper, we propose Eliza, the first open-source web3-friendly Agentic framework that makes the deployment of web3 applications effortless. We emphasize that every aspect of Eliza is a regular Typescript program under the full control of its user, and it seamlessly integrates with web3 (i.e., reading and writing blockchain data, interacting with smart contracts, etc.). Furthermore, we show how stable performance is achieved through the pragmatic implementation of the key components of Eliza's runtime.

---

## 3. Memory OS of AI Agent

**标题**: Memory OS of AI Agent

**作者**: Jiazheng Kang, Mingming Ji, Zhe Zhao, Ting Bai

**年份**: 2025

**摘要**: 
Large Language Models (LLMs) face a crucial challenge from fixed context windows and inadequate memory management, leading to a severe shortage of long-term memory capabilities and limited personalization in the interactive experience with AI agents. To overcome this challenge, we innovatively propose a Memory Operating System, i.e., MemoryOS, to achieve comprehensive and efficient memory management for AI agents. Inspired by the memory management principles in operating systems, MemoryOS designs a hierarchical storage architecture and consists of four key modules: Memory Storage, Updating, Retrieval, and Generation. Specifically, the architecture comprises three levels of storage units: short-term memory, mid-term memory, and long-term personal memory. Key operations within MemoryOS include dynamic updates between storage units: short-term to mid-term updates follow a dialogue-chain-based FIFO principle, while mid-term to long-term updates use a segmented page organization strategy. Our pioneering MemoryOS enables hierarchical memory integration and dynamic updating. Extensive experiments on the LoCoMo benchmark show an average improvement of 49.11% on F1 and 46.18% on BLEU-1 over the baselines on GPT-4o-mini, showing contextual coherence and personalized memory retention in long conversations.
