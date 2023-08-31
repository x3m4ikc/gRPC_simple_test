FROM python:slim
WORKDIR /app
COPY . .
RUN pip3 install poetry
RUN poetry config virtualenvs.create false
RUN poetry install
RUN cd server
CMD ["poetry", "run", "python", "app.py" ]