# Use a imagem oficial do Langflow como base
FROM langflowai/langflow:latest

# Defina diretório de trabalho
WORKDIR /app

# Instale dependências adicionais que você adicionou no pyproject.toml
RUN uv pip install reportlab

CMD ["python", "-m", "langflow", "run", "--host", "0.0.0.0", "--port", "7860"]
