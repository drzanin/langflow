# Use a imagem oficial do Langflow como base
FROM langflow-ai/langflow:latest

# Defina diretório de trabalho
WORKDIR /app

RUN uv pip install reportlab

CMD ["python", "-m", "langflow", "run", "--host", "0.0.0.0", "--port", "7860"]
