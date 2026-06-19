#Conexión con la API
import requests
import pandas as pd
import re
import matplotlib.pyplot as plt

url = "https://rickandmortyapi.com/api/character"

respuesta = requests.get(url)

print("URL consultada:", respuesta.url)
print("Status code:", respuesta.status_code)
print("Content-Type:", respuesta.headers.get("Content-Type"))
