FROM python:3.7.3-stretch
WORKDIR 
/app
## Step 2:
# Copy source code to working directory
COPY . app.py /app

## Step 3:
RUN pip install --upgrade pip &&\
    pip install --trusted-host pypi.python.org -r requirements.txt
# Install packages from requirements.txt
# hadolint ignore=DL3013

## Step 4:
Expose port 80

## Step 5:
CMD ["python","app.py"]