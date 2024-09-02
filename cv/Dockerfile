FROM python:3.7

WORKDIR /usr/src/app

COPY requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt



COPY . .

RUN  pip install --upgrade pip
RUN pip install -U fastai
run apt-get update -y &&  apt-get install graphviz -y
CMD [ "python", "app.py" ]
