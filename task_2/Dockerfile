FROM python:3.10-alpine
WORKDIR /usr/src/app
COPY ./stocks_products/requirements.txt .
RUN pip install -r requirements.txt
COPY ./stocks_products .
RUN python3 manage.py migrate
EXPOSE 8000
CMD ["python3", "manage.py", "runserver", "0.0.0.0:8000"]
