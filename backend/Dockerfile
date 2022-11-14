FROM python:3.8
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1
COPY . /app
WORKDIR /app
RUN pip3 install -r requirements.txt
# RUN python manage.py migrate
# RUN python manage.py runserver 0.0.0.0:8000
# RUN curl -L https://raw.githubusercontent.com/vishnubob/wait-for-it/master/wait-for-it.sh -o wait-for-it.sh && \
#   chmod 755 wait-for-it.sh && \
#   mv wait-for-it.sh /usr/local/bin
# CMD ["/usr/local/bin/wait-for-it.sh", "db:5432", "--timeout=30", "gunicorn -b 0.0.0.0:8000 --worker-class=gevent --worker-connections=1000 --workers=5 backend.wsgi","python manage.py makemigrations","python manage.py migrate"]
# CMD gunicorn -b 0.0.0.0:8000 --worker-class=gevent --worker-connections=1000 --workers=5 backend.wsgi

