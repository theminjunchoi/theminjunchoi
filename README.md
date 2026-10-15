
## 😄 Introduction
Hi, I'm Minjun, a backend developer. Lately I've been spending most of my time on LLM serving infrastructure, mostly fixing bugs and slow paths in projects like AIBrix, LMCache and KAI-Scheduler. I also build side projects with friends and write about them on my [blog](https://minjun.blog/).


## 🌐 Open Source
[LMCache/LMCache](https://github.com/LMCache/LMCache) · KV cache layer for vLLM/SGLang
* Made the ZMQ server work through queued requests in batches instead of one per poll ([#5614](https://github.com/LMCache/LMCache/pull/5614))
* Added `--concurrency` to `lmcache bench server` to compare ZMQ and gRPC ([#5735](https://github.com/LMCache/LMCache/pull/5735))
* Found a gRPC server stall under load and cut its p99 latency from ~9 ms to 1.8 ms ([#5760](https://github.com/LMCache/LMCache/pull/5760))

[vllm-project/aibrix](https://github.com/vllm-project/aibrix) · vLLM's Kubernetes control plane for LLM serving
* Cut prefix-cache routing time by 42% and fixed tokenizer pool failures ([#3035](https://github.com/vllm-project/aibrix/pull/3035))
* Kept model HTTPRoutes in sync with their workloads ([#3017](https://github.com/vllm-project/aibrix/pull/3017))
* Added gateway routing for vLLM `/classify` and `/v1/messages/count_tokens` ([#3015](https://github.com/vllm-project/aibrix/pull/3015), [#3012](https://github.com/vllm-project/aibrix/pull/3012))
* Fixed token metering for streamed `/v1/messages` ([#3009](https://github.com/vllm-project/aibrix/pull/3009))

[kai-scheduler/KAI-Scheduler](https://github.com/kai-scheduler/KAI-Scheduler) · NVIDIA's Kubernetes GPU scheduler
* Cut reclaim time by up to 48% and allocations by up to 75% for many small jobs ([#2420](https://github.com/kai-scheduler/KAI-Scheduler/pull/2420))
* Cut allocations in node scoring by up to 23% ([#2410](https://github.com/kai-scheduler/KAI-Scheduler/pull/2410))
* Kept operator-managed objects from being garbage-collected when kai-config is recreated ([#2372](https://github.com/kai-scheduler/KAI-Scheduler/pull/2372))
* Made a flaky pod affinity e2e test stable ([#2370](https://github.com/kai-scheduler/KAI-Scheduler/pull/2370))


## ✏️ Education 
* [Software (Computer Science & Engineering)](https://cse.cau.ac.kr/main.php), Chung-Ang University (2021.03. ~ )
  
  
## 💻 Activity
* Nexters 29th BE Member (2026.07. ~ 2026.08.)
* GDGoC CAU 5th Organizer (2025.09. ~ )
* Woowacourse 7th BE (2025.02. ~ 2025.11.)
* GDGoC CAU 4th Core Member (2024.09. ~ 2025.08.)
* CECOM Member (2024.09. ~ )
* Undergraduate researcher at [HCSLAB of Chung-Ang Univ.](https://sites.google.com/view/hcslab-cau/home?authuser=0) (2024.09. ~ 2025.01.)
* CAU ZeroPage 32nd vice-President (2022.03. ~ 2023.02.)
* GDSC CAU 1st Member (2021.06. ~ 2022.07.)
* CAU ZeroPage 31st Regular Member (2021.03. ~ )


## 🚀 Projects
* [GAMSS](https://github.com/Nexters/GAMSS-Server) - An emotional trash can for things you can't tell anyone. (2026.07. ~ )
* [ZZOL](https://github.com/woowacourse-teams/2025-zzol) - A luck-based game that even clumsy players can enjoy! (2025.07. ~ )

