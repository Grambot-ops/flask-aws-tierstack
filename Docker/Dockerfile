# Image we are going to use for running the Application

FROM python:3.13.3-slim-bookworm

# we now say to docker what is the working directory of the application

WORKDIR /app

# Now we copy the application file to the /app location

COPY ../Simple_Flusk_app/ .

# Now we install what is need

RUN pip install --no-cache-dir -r requirements.txt

# now we expose the port of the application

EXPOSE 5000

# Now we define the application we going to run

CMD [ "python", "crudapp.py" ]