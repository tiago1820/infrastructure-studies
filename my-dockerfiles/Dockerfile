FROM debian

# Instala Node.js y npm
RUN apt-get update && \
    apt-get install -y nodejs npm

# Crea un directorio de trabajo dentro del contenedor
WORKDIR /app

# Copia los archivos de tu aplicación al contenedor
COPY . .

# Instala las dependencias de tu aplicación
RUN npm install

# Expone el puerto en el que tu aplicación escucha (si es necesario)
EXPOSE 3001

# Comando para iniciar tu aplicación (ajusta según tu configuración)
CMD ["npm", "start"]

