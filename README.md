
## 😄 Introduction
Hi, I'm Minjun. Most of my time goes into making LLM serving faster and more reliable. I fix bugs and performance issues in open-source projects like LMCache and AIBrix, and I'm also building [pygrpc-native](https://github.com/pygrpc/pygrpc-native), a Python gRPC server backed by Rust. On the side, I make things with friends and write about them on my [blog](https://minjun.blog/).


## 🌐 Open Source
[LMCache/LMCache](https://github.com/LMCache/LMCache) · KV cache layer for vLLM/SGLang · [14 merged PRs](https://github.com/LMCache/LMCache/pulls?q=is%3Apr+is%3Amerged+author%3Atheminjunchoi)
* Added a native gRPC server mode in Rust, outside the GIL, with 1.2x ZMQ's throughput ([#6031](https://github.com/LMCache/LMCache/pull/6031))
* Raised gRPC throughput 1.9x via an asyncio server with bounded stream read-ahead ([#5799](https://github.com/LMCache/LMCache/pull/5799), [#5858](https://github.com/LMCache/LMCache/pull/5858))
* Cut gRPC p99 latency from ~9 ms to 1.8 ms by fixing a metrics flush stall ([#5760](https://github.com/LMCache/LMCache/pull/5760))
* Cut gRPC recovery after a server restart from 36 s to 0.4 s by bounding reconnect backoff ([#5825](https://github.com/LMCache/LMCache/pull/5825))
* Sped up the gRPC codec for up to 2x lookup and 1.7x stream throughput ([#5935](https://github.com/LMCache/LMCache/pull/5935), [#5906](https://github.com/LMCache/LMCache/pull/5906))

[vllm-project/aibrix](https://github.com/vllm-project/aibrix) · vLLM's Kubernetes control plane for LLM serving · [11 merged PRs](https://github.com/vllm-project/aibrix/pulls?q=is%3Apr+is%3Amerged+author%3Atheminjunchoi)
* Built an encode stage for multimodal requests in PD and E+PD disaggregated routing ([#3069](https://github.com/vllm-project/aibrix/pull/3069), [#3153](https://github.com/vllm-project/aibrix/pull/3153), [#3200](https://github.com/vllm-project/aibrix/pull/3200))
* Cut prefix-cache routing latency by 42% and fixed tokenizer pool failures ([#3035](https://github.com/vllm-project/aibrix/pull/3035))
* Fixed LoRA prefix-cache routing by indexing KV cache blocks per adapter ([#3097](https://github.com/vllm-project/aibrix/pull/3097))

[vllm-project/semantic-router](https://github.com/vllm-project/semantic-router) · vLLM's intelligent router for mixture-of-models serving
* Cut JSON validation time by up to 44% for requests and 64% for responses ([#5204](https://github.com/vllm-project/semantic-router/pull/5204))

[vllm-project/guidellm](https://github.com/vllm-project/guidellm) · Benchmarking tool for LLM inference deployments · [2 merged PRs](https://github.com/vllm-project/guidellm/pulls?q=is%3Apr+is%3Amerged+author%3Atheminjunchoi)
* Added collectors that scrape server metrics from Prometheus while a benchmark runs ([#1250](https://github.com/vllm-project/guidellm/pull/1250))
* Fixed streaming requests bypassing the mock server's concurrency limit ([#1262](https://github.com/vllm-project/guidellm/pull/1262))

[vllm-project/production-stack](https://github.com/vllm-project/production-stack) · vLLM's reference stack for Kubernetes deployment
* Kept prefill/decode model labels when a dynamic config reload rebuilds the router ([#1129](https://github.com/vllm-project/production-stack/pull/1129))

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
* [pygrpc-native](https://github.com/pygrpc/pygrpc-native) - A Rust-backed gRPC server for Python, used by LMCache. (2026.10. ~ )
* [GAMSS](https://github.com/Nexters/GAMSS-Server) - An emotional trash can for things you can't tell anyone. (2026.07. ~ )
* [ZZOL](https://github.com/woowacourse-teams/2025-zzol) - A luck-based game that even clumsy players can enjoy! (2025.07. ~ )

