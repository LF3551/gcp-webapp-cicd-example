FROM python:3.8-slim
WORKDIR /app
RUN ls -la 
RUN ls -la /app/
RUN cd .. && ls -la
COPY requirements.txt .
RUN pip install -r requirements.txt
COPY . /app
CMD ["python", "/app/app.py"]
