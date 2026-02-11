# RTAverse AI (Cloud Version)

This is the cloud-hosted version of the RTAverse Traffic Forecasting System. It runs on Google Colab using a Tesla T4 GPU and serves a web interface via Ngrok.

## How to Run
1. Open the notebook in Google Colab.
2. Add your API tokens to the Colab Secrets manager (Key icon on the left):
   - Name: `HF_TOKEN` (Your Hugging Face Read Token)
   - Name: `NGROK_TOKEN` (Your Ngrok Authtoken)
3. Run all cells.
4. Click the public `ngrok-free.app` link generated in the final cell output to access the interface.

## Tech Stack
- **Model:** Llama 3 (8B Instruct) via Hugging Face
- **Backend:** Flask & LangChain
- **Frontend:** HTML/CSS (Rendered via Flask)
- **Infrastructure:** Google Colab (GPU) & Ngrok (Tunneling)
