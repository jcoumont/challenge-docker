# Create an image based on python 3.7
FROM python:3.7
# Create a directory "app"
RUN mkdir /app
# Copy all source code to the app folder
COPY pipeline/ /app/pipeline/
# Copy requirement.txt to app folder
COPY requirements.txt /app/requirements.txt
# Select the work directory
WORKDIR /app
# Install required packages
RUN pip install -r requirements.txt
# Launch the python command
CMD ["python", "pipeline/model/model.py"]