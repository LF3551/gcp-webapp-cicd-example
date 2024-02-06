FROM python:3.8-slim
WORKDIR /app
RUN ls -la /app/
COPY requirements.txt ./
RUN ls -la /app/
RUN pip install -r requirements.txt
COPY . /app
CMD ["python", "app.py"]