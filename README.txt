Para ejecurtar los algoritmos, se debe descargar la base de datos
del siguiente link: https://data.cityofnewyork.us/Public-Safety/NYPD-Complaint-Data-Historic/qgea-i56i
Subirla a drive, y luegoabrir los archivos con google colab, vincular drive con 
las siguientes lineas de codigo: 

from google.colab import drive
drive.mount('/content/drive')

y ultimamente ajustar la ruta en la que se subio la base en la siguiente linea de codigo:
df = pd.read_csv('/content/drive/MyDrive/Colab Notebooks/NYPD_Complaint_Data_Historic.csv', skiprows=lambda x: x % 2 != 0)