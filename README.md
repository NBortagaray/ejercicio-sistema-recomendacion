# Ejercicio Sistema Recomendación
Grupo 4

## Descripción

El objetivo de este proyecto es crear un sistema de recomendación capaz de generar 20 recomendaciones personalizadas para cada usuario, incluyendo aquellos usuarios que no tienen interacciones previas en el conjunto de entrenamiento (cold start).
El sistema de recomendación se basa en un modelo de factorización de matrices implementado utilizando la biblioteca LightFM. Además, para los usuarios sin interacciones en el conjunto de entrenamiento, se recomienda una lista de los 20 contenidos más populares.

## Uso
1. Clona el repositorio:

    ```bash
    gh repo clone NBortagaray/ejercicio-sistema-recomendacion
    ```
    
2. Crea y activa un entorno virtual:
    ```bash
    python -m venv .venv
    source .venv/bin/activate
    ```
3. Instala las dependencias:
    ```bash
    pip install -r requirements.txt
    ```
    
4. Abre el notebook de Jupyter
5. Descarga los archivos train.csv y metadata.csv desde el siguiente link: https://drive.google.com/drive/folders/1rEu1e5EImJZBDvPNysZdEwP4hDU9u4aX?usp=sharing
6. Ejecuta las celdas del notebook para entrenar el modelo y generar las recomendaciones.
7. Las recomendaciones generadas se guardarán en un archivo CSV llamado recomms.csv (Tambien se puede descargar desde el link del punto 5).

## Métricas
El sistema de recomendación ha sido evaluado utilizando la métrica Mean Average Precision (MAP). El resultado obtenido es:
```bash
Mean Average Precision = 0.065
```
