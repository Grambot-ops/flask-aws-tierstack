# Image we are going to use for running the Application

FROM python:3.13.3-slim-bookworm

# we now say to docker what is the working directory of the application
WORKDIR /app

# Now we copy the application file to the /app location
COPY ./Simple_Flask_app/ .

# Now we install what is need
RUN pip install --no-cache-dir -r requirements.txt

# Set environment variables
ENV FLASK_APP=crudapp.py
ENV FLASK_ENV=development

# now we expose the port of the application
EXPOSE 5000

# Now we define the application we going to run
CMD ["flask", "run", "--host=0.0.0.0"]