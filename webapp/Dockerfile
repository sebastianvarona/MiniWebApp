FROM python:3.6

EXPOSE 5000
ENV FLASK_APP=run.py

WORKDIR /app
COPY . /app

COPY requirements.txt /app
RUN pip install -r requirements.txt

COPY run.py /app

CMD ["python3", "-m", "flask", "run", "--host=0.0.0.0"]
