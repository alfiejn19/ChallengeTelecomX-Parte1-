# ChallengeTelecomX-Parte1-
ChallengeTelecomX(Parte1) Esta es la solución.
Challenge Telecom X - Análisis de Datos
Este proyecto aborda el análisis de datos para Telecom X, enfocado en predecir el fenómeno de "Churn" (abandono de clientes). El proceso se divide en tres etapas principales: extracción, transformación y estandarización de datos.

🔍 Pasos Realizados

1. Extracción de Datos
+ Carga inicial del dataset desde un archivo JSON remoto.
+ Normalización de datos anidados en las columnas:
  + customer
  + phone
  + internet
+ Renombramiento de columnas para eliminar prefijos redundantes.

2. Transformación de Datos
+ Limpieza de datos:
  + Eliminación de valores vacíos en Churn (224 registros) y Charges.Total (11 registros).
  + Tipificación correcta de Charges.Total como float64.
+ Renombramiento de columnas en español para mejor comprensión.

3. Estandarización de Datos
   + Variables binarias.
   + Variables categóricas con dummies.

4. Análisis y creación de gráficas.

📈 Análisis Exploratorio (Hallazgos Clave)  

**1. Patrones Críticos de Abandono** 
- **Servicios Digitales:**  
  - Clientes **sin seguridad online**: 10x más churn (3,443 vs 295)  
  - Clientes **sin streaming**: 85% más probabilidad de abandono  
- **Factores Contractuales:**  
  - Contratos **mensuales**: 45% de abandonos vs **12%** en contratos de 2 años  
  - Facturas **< $50**: 3.2x más riesgo  

**2. Perfil Demográfico de Riesgo**
+riesgo)  
| Segmento | Tasa Churn |  
|----------|------------|  
| Hombres solteros <45 años | 38.7% |  
| Jubilados | 12.1% |  
| Usuarios sin internet | 42.3% |  

**3. Servicios que Retienen**  
Seguridad Online:    ↓91.4% churn  
Fibra Óptica:        ↓67% churn vs DSL  
Contratos 2 años:    ↓73% churn vs mensual  
