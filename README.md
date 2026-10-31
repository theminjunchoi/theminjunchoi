
## 😄 Introduction
Hi, I'm Minjun. Most of my time goes into making LLM serving faster and more reliable. I fix bugs and performance issues in open-source projects like LMCache and AIBrix, and I'm also building [pygrpc-native](https://github.com/pygrpc/pygrpc-native), a Python gRPC server backed by Rust. On the side, I make things with friends and write about them on my [blog](https://minjun.blog/).


## 🌐 Open Source
[pygrpc/pygrpc-native](https://github.com/pygrpc/pygrpc-native) · Drop-in Python gRPC server with its HTTP/2 layer in Rust · used by LMCache
* Runs LMCache's native gRPC mode and ships in its Docker images ([#6031](https://github.com/LMCache/LMCache/pull/6031), [#6048](https://github.com/LMCache/LMCache/pull/6048))
* Made LMCache's gRPC transport 21% faster than ZMQ, where grpcio was 36% slower
* Replaces `grpc.server()` in one line, with existing servicers and interceptors unchanged
* 1.5x grpcio's calls per second from a single client thread, 5x from 32

[LMCache/LMCache](https://github.com/LMCache/LMCache) · KV cache layer for vLLM/SGLang · [22 merged PRs](https://github.com/LMCache/LMCache/pulls?q=is%3Apr+is%3Amerged+author%3Atheminjunchoi)
* Added a native gRPC server mode in Rust, outside the GIL, with 1.2x ZMQ's throughput ([#6031](https://github.com/LMCache/LMCache/pull/6031))
* Raised gRPC throughput 1.9x via an asyncio server with bounded stream read-ahead ([#5799](https://github.com/LMCache/LMCache/pull/5799), [#5858](https://github.com/LMCache/LMCache/pull/5858))
* Cut gRPC p99 latency from ~9 ms to 1.8 ms by fixing a metrics flush stall ([#5760](https://github.com/LMCache/LMCache/pull/5760))
* Cut gRPC recovery after a server restart from 36 s to 0.4 s by bounding reconnect backoff ([#5825](https://github.com/LMCache/LMCache/pull/5825))

[vllm-project/aibrix](https://github.com/vllm-project/aibrix) · vLLM's Kubernetes control plane for LLM serving · [11 merged PRs](https://github.com/vllm-project/aibrix/pulls?q=is%3Apr+is%3Amerged+author%3Atheminjunchoi)
* Built an encode stage for multimodal requests in PD and E+PD disaggregated routing ([#3069](https://github.com/vllm-project/aibrix/pull/3069), [#3153](https://github.com/vllm-project/aibrix/pull/3153), [#3200](https://github.com/vllm-project/aibrix/pull/3200))
* Cut prefix-cache routing latency by 42% and fixed tokenizer pool failures ([#3035](https://github.com/vllm-project/aibrix/pull/3035))
* Fixed LoRA prefix-cache routing by indexing KV cache blocks per adapter ([#3097](https://github.com/vllm-project/aibrix/pull/3097))

Also contributed to [KAI-Scheduler](https://github.com/kai-scheduler/KAI-Scheduler/pulls?q=is%3Apr+is%3Amerged+author%3Atheminjunchoi) (5 PRs, up to 48% faster reclaim) · [guidellm](https://github.com/vllm-project/guidellm/pulls?q=is%3Apr+is%3Amerged+author%3Atheminjunchoi) (2 PRs) · [semantic-router](https://github.com/vllm-project/semantic-router/pull/5204) · [production-stack](https://github.com/vllm-project/production-stack/pull/1129)


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

