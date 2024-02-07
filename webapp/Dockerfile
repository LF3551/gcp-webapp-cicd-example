FROM python:3.11-slim
WORKDIR /app
COPY requirements.txt /app/
RUN pip install -r requirements.txt
COPY app.py /app/
COPY templates /app/templates
CMD ["python", "/app/app.py"]
