FROM python:2.7
LABEL maintainer="marcondol"

COPY . /app
WORKDIR /app
RUN pip install -r requirements.txt
RUN python init_db.py
EXPOSE 3111/tcp

CMD [ "python", "app.py" ]