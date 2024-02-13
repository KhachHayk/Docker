FROM python

WORKDIR /django

COPY ./django /django

RUN pip install -r /django/requirements.txt

ENV SECRET_KEY wqevrbntjykliyuktyjrthr

ENV DEBUG True

RUN python3 manage.py migrate

EXPOSE 8000

CMD gunicorn stocks_products.wsgi -b 0.0.0.0:8000