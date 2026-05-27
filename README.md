# SimpleXAI

SimpleXAI is an unrestricted AI assistant.

## Deploy

1. Download a GGUF model and place it in `./model/model.gguf`
2. Install dependencies: `pip install -r requirements.txt`
3. Run: `python app.py`

## Deploy to Hugging Face Spaces

Choose Docker SDK: `docker run -p 8080:8080 -e MODEL_PATH=/app/model/model.gguf -v ./model:/app/model your-image`

## API

- `POST /chat` - Send chat message
- `POST /run` - Execute code
- `GET /health` - Health check
