FROM python:3.10
#Crear un directorio de trabajo
WORKDIR /servidor
COPY servidor.py .

#instala las depedencias necesarias
RUN pip install flask

#Ejecutar 1 aplicacion

CMD [ "python","servidor.py" ]

EXPOSE 5002