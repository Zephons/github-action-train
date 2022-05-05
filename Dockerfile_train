FROM python:3.8-slim-buster
LABEL maintainer="Hetic"

RUN pip install pipenv
COPY Pipfile .
RUN pipenv install

COPY train.py /train.py

CMD ["pipenv", "run", "python", "train.py"]