FROM python:3.8-slim
WORKDIR /app
COPY requirements.txt /app/
RUN ls -la /app/
RUN pip install -r requirements.txt
COPY app.py /app/
CMD ["python", "/app/app.py"]
