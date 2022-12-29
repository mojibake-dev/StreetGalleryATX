#our image
FROM python:3.8-slim-buster

#opens port
EXPOSE 8000
#names our working dir
WORKDIR /app
#brings requirements.txt into container
COPY requirements.txt /app
#install dependencies
RUN pip3 install -r requirements.txt --no-cache-dir
#brings source code into container
COPY . /app 

ENTRYPOINT ["python3"] 
CMD ["manage.py", "runserver", "0.0.0.0:8000"]