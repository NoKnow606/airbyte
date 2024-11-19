FROM noknow606/source-file-rowland:0.0.3

WORKDIR /airbyte/integration_code
COPY source_file_secure ./source_file_secure
COPY main.py ./
COPY setup.py ./
RUN pip install .
RUN pip install numpy==1.26.4

ENV AIRBYTE_ENTRYPOINT "python /airbyte/integration_code/main.py"
ENTRYPOINT ["python", "/airbyte/integration_code/main.py"]

LABEL io.airbyte.version=0.2.31
LABEL io.airbyte.name=airbyte/source-file-secure
