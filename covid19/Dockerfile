FROM python:3.7

ADD . /usr/src/app
WORKDIR /usr/src/app

COPY requirements.txt ./
RUN pip install --upgrade pip
RUN pip install -r requirements.txt
EXPOSE 3000

COPY . .
RUN ls
CMD ["python", "./manage.py", "runserver", "0.0.0.0:3000"]