ARG PYTHON_IMAGE_VERSION
FROM python:${PYTHON_IMAGE_VERSION}
ENV PYTHONUNBUFFERED=1
COPY . /app
WORKDIR /app
RUN pip3 install -r requirements.txt
CMD gunicorn app:app -b 0.0.0.0:8000