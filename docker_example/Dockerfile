# Use a imagem oficial do Langflow como base
FROM langflowai/langflow:latest

# Defina diretório de trabalho
WORKDIR /app

# Copie o pyproject.toml para instalar dependências personalizadas (caso precise)
COPY pyproject.toml /app/pyproject.toml

# Instale dependências adicionais que você adicionou no pyproject.toml
RUN uv pip install reportlab

# Ou, caso queira instalar todas as dependências (caso tenha adicionado mais):
# RUN uv pip install . 

# Execute o Langflow normalmente
CMD ["python", "-m", "langflow", "run", "--host", "0.0.0.0", "--port", "7860"]
