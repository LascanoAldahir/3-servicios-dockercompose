FROM python:3.10
#Crear un directorio de trabajo
WORKDIR /servidor
COPY app1.py .

#instala las depedencias necesarias
RUN pip install flask

#Ejecutar 1 aplicacion

CMD [ "python","app1.py" ]

EXPOSE 5002