# Samsung Innovation Campus 2023-2024  
## Proyecto: Análisis de Factores Influyentes en el Suicidio  

**Equipo:** QWERTY  

### Integrantes y Roles  
- **Karol Urbina**: Investigación temática, búsqueda de datasets y desarrollo  
- **Kevin Durán**: Búsqueda, desarrollo, procesamiento y estructuración de los datos  
- **Andrés Bueno**: Análisis y visualización  
- **Cristian Molina**: Limpieza y procesamiento de datos  
- **Jesús Moreno**: Análisis y visualización  

---

### Descripción del Proyecto  
Este proyecto busca **entender, analizar e interpretar datos globales** obtenidos de fuentes verificadas sobre el suicidio, una emergencia sanitaria de gran relevancia en los últimos 60 años debido al impacto del desarrollo industrial, político y tecnológico.  

El objetivo principal es analizar patrones por **edad (generacionales)** y **regiones (continentes)**, vinculándolos a sucesos históricos para identificar raíces contextuales que permitan comprender este problema con mayor precisión.  

---

### Estructura del Repositorio  

#### Ramas del Proyecto  
- **Branch - Desarrollo:**  
  Contiene notebooks preliminares y datos iniciales.  
  - `Dataset`: Datasets originales utilizados  
  - `Datasets limpios`: Datos tras el proceso de limpieza  
  - `Notebooks Datos limpios`: Código sobre la limpieza  
  - `Notebook Pre-análisis`: Exploración inicial de los datos  

- **Branch - Proyecto:**  
  Contiene resultados finales y análisis formateados.  
  - `Datasets`: Archivos limpios y procesados  
  - `json`: Archivo `.json` para mapas de calor  
  - **Notebooks:**  
    - `Procesamiento-data`: Procesamiento analítico de los datos  
    - **Análisis:** Notebooks por grupos etarios:  
      - `Analisis_Niñez`: [5-9] y [10-14 años]  
      - `Analisis_Adolescencia`: [15-19] y [20-24 años]  
      - `Analisis_Adultez`: [25-29] y [30-34 años]  
      - `Analisis_Madurez`: [35-39], [40-44], [45-49], [50-54], [55-59 años]  
      - `Analisis_Vejez`: [60-64] y [65-69 años]  

---

### Datasets  
1. **[Suicide Rates Overview 1985-2021 (Kaggle)](https://www.kaggle.com/datasets/omkargowda/suicide-rates-overview-1985-to-2021):**  
   - Datos obtenidos de:  
     - United Nations Development Program (2018)  
     - World Bank (2018)  
     - WHO (2018)  
     - Szamil (2017)  

2. **[WHO Suicide Statistics](https://www.kaggle.com/datasets/szamil/who-suicide-statistics/data):**  
   Dataset complementario con mayor detalle estadístico.  

3. **[WHO Suicide Data 1950-2021](https://www.kaggle.com/datasets/kumaranand05/who-suicide-data-1950-2021):**  
   Datos de amplio rango histórico y análisis comparativo.  

---

### Estructura de Análisis  

#### División del Dataset  
1. **Por Región:**  
   - América  
   - Europa  
   - Asia  
   - Oceanía  
   - África  

2. **Por Edad:**  
   - Niñez y Pre-adolescencia: [5-9], [10-14 años]  
   - Adolescencia y Juventud: [15-19], [20-24 años]  
   - Adultez: [25-29], [30-34 años]  
   - Madurez: [35-39], [40-44], [45-49], [50-54], [55-59 años]  
   - Vejez: [60-64], [65-69 años]  

3. **Por Generación:**  
   - **Grandiosa:** 1900-1927  
   - **Silenciosa:** 1928-1945  
   - **Boomers:** 1946-1964  
   - **Generación X:** 1965-1981  
   - **Generación Y:** 1982-1996  
   - **Generación Z:** 1997-2012  
   - **Generación Alfa:** 2013-2020  

#### Cálculos Generacionales  
Se usaron los años registrados desde **1969 hasta 2020**, con una alta densidad de datos.  

**Ejemplo:**  
- Registro de **1980** en el rango de edad **[5-9 años]:**  
  - Año de nacimiento estimado: `1980 - 5 = 1975`.  
  - Generación asignada: **Generación X.**  
- Si un rango abarca dos generaciones, se clasifica como "Generación de Transición" (e.g., **Generación X/Generación Y**).  

Y también:
### Regla para el Conteo de Suicidios  
El conteo de suicidios se define como:  

```plaintext
Conteo de suicidios = Conteo de Suicidios por edad (Rango de edad 1) + Conteo de Suicidios por edad (Rango de edad 2)

### Entonces  
Con aproximadamente **10,000 registros**, se descartaron filas con:  
- Datos nulos.  
- Conteo de suicidios igual a cero.  

### Visualización y conclusiones 

#### 1. Análisis Etario: Suicidios por Edad  
![](https://github.com/Andres-cymk/QWERTY/blob/Proyecto/imagenes/1.jpg) 
**Descripción:** Gráfica que compara el conteo de suicidios por rangos etarios, permitiendo identificar tendencias en generaciones específicas.  

#### 2. Evolución Histórica de Suicidios  
![][(https://github.com/Andres-cymk/QWERTY/blob/Proyecto/imagenes/2.jpg)]
**Descripción:** Representación temporal de los datos, enfocándose en los cambios y picos a lo largo de las últimas décadas.  

#### 3. Relación entre Suicidio y Etapas de vida  
**[](https://www.github.com/Andres-cymk/QWERTY/blob/Proyecto/imagenes/3.jpg)**

#### 4. Mapa de Calor por Continentes  
https://github.com/Andres-cymk/QWERTY/blob/9f7e77137b3aa12a4e1227e6b7d8742763c8776f/imagenes/4.jpg
**Descripción:** Este mapa muestra la densidad de suicidios por región, destacando áreas con mayor impacto durante el periodo analizado.  

