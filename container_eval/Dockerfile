FROM python:3.9 
WORKDIR /app
COPY . .
RUN pip install --upgrade pip && \
    pip install --no-cache-dir streamlit psycopg2-binary

EXPOSE 8501
CMD ["streamlit", "run", "stream.py", "--server.port=8501", "--server.address=0.0.0.0"]