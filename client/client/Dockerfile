FROM python:slim
WORKDIR /app
COPY ./client/app.py /app/app.py
COPY ./pyproject.toml /app/pyproject.toml
RUN pip3 install poetry
RUN poetry config virtualenvs.create false
RUN poetry install
CMD [ "poetry", "run", "python", "app.py" ]