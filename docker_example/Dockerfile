FROM langflowai/langflow:latest

# Copia os arquivos de dependências
COPY pyproject.toml poetry.lock* requirements.txt* ./

# Instala as dependências adicionais
RUN pip install --upgrade pip \
    && pip install .

# Executa o Langflow
CMD ["python", "-m", "langflow", "run", "--host", "0.0.0.0", "--port", "7860"]