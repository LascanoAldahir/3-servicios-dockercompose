app1.py: <br>
from flask import Flask
app1 = Flask(_name_)
@app1.route('/')
def hola ():
    return "Hola desde el servidor soy aldahir"

if _name_ == '_main_':
    app1.run(host='0.0.0.0', port=5003)

<br><br><br>
dockerfile <br><br>
bash '''
FROM python:3.10
#Crear un directorio de trabajo...
WORKDIR /servidor
COPY app1.py .

#instala las depedencias necesarias
RUN pip install flask

#Ejecutar 1 aplicacion

CMD [ "python","app1.py" ]

EXPOSE 5002
