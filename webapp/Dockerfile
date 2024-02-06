FROM python:3.8-slim
RUN ls -la /app/
WORKDIR /app
RUN ls -la /app/
COPY requirements.txt .
RUN pip install -r requirements.txt
COPY . /app
CMD ["python", "/app/app.py"]
