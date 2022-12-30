#our image
FROM python:3

#opens port
EXPOSE 8000

#names our working dir
WORKDIR /StreetGalleryATX

#brings source code into container
COPY . /StreetGalleryATX

# # Create a virtual environment in /opt
# RUN python3 -m venv /opt/venv

#install dependencies
RUN pip install -r requirements.txt --no-cache-dir

#lanuch 
ENTRYPOINT ["python3"] 
CMD ["manage.py", "runserver", "0.0.0.0:8000"]