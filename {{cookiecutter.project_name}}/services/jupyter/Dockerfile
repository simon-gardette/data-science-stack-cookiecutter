FROM jupyter/scipy-notebook

USER root

RUN pip install --proxy=${http_proxy}\
    psycopg2-binary\
    SQLAlchemy\
    minio

RUN jupyter labextension install @jupyterlab/celltags

USER {{cookiecutter.owner_name}}
