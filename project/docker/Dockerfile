FROM python:3.7
ENV PYTHONUNBUFFERED 1

RUN mkdir /code
WORKDIR /code

# RUN apt-get update && apt-get install -y --no-install-recommends \
#     gcc \
#     libpq-dev \
#     && apt-get clean \
#     && rm -rf /var/lib/apt/lists/*

COPY requirements.txt /code/
RUN pip install --upgrade pip && pip install --no-cache-dir -r requirements.txt

COPY . /code/
