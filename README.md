<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/vllm-project/vllm/main/docs/source/assets/logos/vllm-logo-text-dark.png">
    <img alt="vLLM" src="https://raw.githubusercontent.com/vllm-project/vllm/main/docs/source/assets/logos/vllm-logo-text-light.png" width=55%>
  </picture>
</p>

<h3 align="center">
Easy, fast, and cheap LLM serving for everyone
</h3>

<p align="center">
| <a href="https://docs.vllm.ai"><b>Documentation</b></a> | <a href="https://vllm.ai"><b>Blog</b></a> | <a href="https://arxiv.org/abs/2309.06180"><b>Paper</b></a> | <a href="https://discord.gg/jz7wjKhh6g"><b>Discord</b></a> |

</p>

## Changes
In this project, we implemented request parallel reasoning. By setting the degree of request parallelism, multiple schedulers can simultaneously schedule different requests to different workers to realize asynchronous execution reasoning, thus improving the computing throughput.You only need to set the num_parallel_requests parameter during LLM instantiation.

## Design frame drawing
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/yaoc6620/vllm_requests/requestPallel/vllm1.png?token=GHSAT0AAAAAACUMMYI7XVHGF2J336IO5X6MZVJ37HA">
    <img alt="vLLM" src="https://raw.githubusercontent.com/yaoc6620/vllm_requests/requestPallel/vllm1.png?token=GHSAT0AAAAAACUMMYI7XVHGF2J336IO5X6MZVJ37HA" width=70%>
  </picture>
  <div style="height: 40px;"></div>
</p>
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/yaoc6620/vllm_requests/requestPallel/vllm2.png?token=GHSAT0AAAAAACUMMYI62VZSCTU2INSMKFNSZVJ4AGQ">
    <img alt="vLLM" src="https://raw.githubusercontent.com/yaoc6620/vllm_requests/requestPallel/vllm2.png?token=GHSAT0AAAAAACUMMYI62VZSCTU2INSMKFNSZVJ4AGQ" width=70%>
  </picture>
  <div style="height: 20px;"></div>
</p>
