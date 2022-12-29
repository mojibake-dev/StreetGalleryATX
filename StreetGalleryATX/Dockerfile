#our image
FROM python:3.8-slim-buster

#opens port
EXPOSE 8000
#names our working dir
WORKDIR /StreetGalleryATX
#brings requirements.txt into container
COPY requirements.txt /StreetGalleryATX
#install dependencies
RUN pip3 install -r requirements.txt --no-cache-dir
#brings source code into container
COPY . /StreetGalleryATX

ENTRYPOINT ["python3"] 
CMD ["manage.py", "runserver", "0.0.0.0:8000"]