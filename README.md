# ▀▄▀ █▄ █▄ █▚▞▌ docker-compose

Run Llama-3.2-11B-Vision-Instruct with 4-bit quantization using vLLM and Open WebUI.

## Prerequisites
- NVIDIA GPU with CUDA support
- Docker and Docker Compose
- Hugging Face token
- Cloudflare tunnel token (optional, for remote access)

## Setup
1. Copy `env-example` to `.env` and fill in:
   - `HF_TOKEN`: Your Hugging Face token
   - `VLLM_API_KEY`: Generate a random API key
   - `CLOUDFLARE_TUNNEL_TOKEN`: Your Cloudflare tunnel token (optional)

2. Start the services:
   ```bash
   # Start all services
   docker compose up -d

   # View logs
   docker compose logs -f
   ```

3. Access the UI:
   - Local: http://localhost:3000
   - Remote: If using Cloudflare tunnel, access via your configured domain
