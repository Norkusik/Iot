FROM python:3.6

WORKDIR /usr/src/app

COPY requirements.txt ./

RUN pip install --no-cache-dir -r requirements.txt

COPY . .

ENV FLASK_APP main.py
ENV FLASK_DEBUG=1
CMD ["python", "-m", "flask", "run", "--host=0.0.0.0", "--port=8090"]
