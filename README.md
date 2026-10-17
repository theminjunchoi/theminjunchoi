
## 😄 Introduction
Hi, I'm Minjun. Lately I've been spending most of my time on LLM serving infrastructure, mostly fixing bugs and performance bottlenecks in projects like LMCache, AIBrix, guidellm and KAI-Scheduler. I also build side projects with friends and write about them on my [blog](https://minjun.blog/).


## 🌐 Open Source
[LMCache/LMCache](https://github.com/LMCache/LMCache) · KV cache layer for vLLM/SGLang · [6 merged PRs](https://github.com/LMCache/LMCache/pulls?q=is%3Apr+is%3Amerged+author%3Atheminjunchoi)
* Cut gRPC transport p99 latency from ~9 ms to 1.8 ms by fixing a metrics flush stall ([#5760](https://github.com/LMCache/LMCache/pull/5760))
* Added a concurrent-client mode to `lmcache bench server` to compare ZMQ and gRPC ([#5735](https://github.com/LMCache/LMCache/pull/5735))
* Raised ZMQ server throughput by up to 37% under concurrent load by batching requests ([#5614](https://github.com/LMCache/LMCache/pull/5614))
* Fixed L1 cache filling up to 100% in buffer-only mode by retrying blocked deletions ([#5802](https://github.com/LMCache/LMCache/pull/5802))

[vllm-project/aibrix](https://github.com/vllm-project/aibrix) · vLLM's Kubernetes control plane for LLM serving · [8 merged PRs](https://github.com/vllm-project/aibrix/pulls?q=is%3Apr+is%3Amerged+author%3Atheminjunchoi)
* Built an encode stage for multimodal requests in prefill/decode disaggregated routing ([#3069](https://github.com/vllm-project/aibrix/pull/3069))
* Cut prefix-cache routing latency by 42% and fixed tokenizer pool failures ([#3035](https://github.com/vllm-project/aibrix/pull/3035))
* Fixed LoRA prefix-cache routing by indexing KV cache blocks per adapter ([#3097](https://github.com/vllm-project/aibrix/pull/3097))

[vllm-project/guidellm](https://github.com/vllm-project/guidellm) · Benchmarking tool for LLM inference deployments
* Fixed streaming requests bypassing the mock server's concurrency limit ([#1262](https://github.com/vllm-project/guidellm/pull/1262))

[kai-scheduler/KAI-Scheduler](https://github.com/kai-scheduler/KAI-Scheduler) · NVIDIA's Kubernetes GPU scheduler · [5 merged PRs](https://github.com/kai-scheduler/KAI-Scheduler/pulls?q=is%3Apr+is%3Amerged+author%3Atheminjunchoi)
* Cut reclaim time by up to 48% and allocations by up to 75% for many small jobs ([#2420](https://github.com/kai-scheduler/KAI-Scheduler/pull/2420))
* Cut memory use by 53% in reclaim scenario search by reusing cloned victim jobs ([#2400](https://github.com/kai-scheduler/KAI-Scheduler/pull/2400))
* Cut allocations in GPU node scoring by up to 23% ([#2410](https://github.com/kai-scheduler/KAI-Scheduler/pull/2410))


## ✏️ Education 
* [Software (Computer Science & Engineering)](https://cse.cau.ac.kr/main.php), Chung-Ang University (2021.03. ~ )
  
  
## 💻 Activity
* Nexters 29th BE Member (2026.07. ~ 2026.08.)
* GDGoC CAU 4th Core Member, 5th Organizer, 6th Team Member (2024.09. ~ )
* Woowacourse 7th BE (2025.02. ~ 2025.11.)
* CECOM Member (2024.09. ~ 2026.02.)
* Undergraduate researcher at [HCSLAB of Chung-Ang Univ.](https://sites.google.com/view/hcslab-cau/home?authuser=0) (2024.09. ~ 2025.01.)
* GDSC CAU 1st Member (2021.06. ~ 2022.07.)
* CAU ZeroPage 31st Member, 32nd Vice-President (2021.03. ~ )


## 🚀 Projects
* [GAMSS](https://github.com/Nexters/GAMSS-Server) - An emotional trash can for things you can't tell anyone. (2026.07. ~ )
* [ZZOL](https://github.com/woowacourse-teams/2025-zzol) - A luck-based game that even clumsy players can enjoy! (2025.07. ~ )

