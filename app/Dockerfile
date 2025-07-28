FROM python:3.11-slim
LABEL maintainer="seniv.05@gmail.com"

ENV PYTHOUNNBUFFERED=1
WORKDIR app/

COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt

COPY . .

CMD ["python", "main.py", "runserver", "0.0.0.0:8000"]