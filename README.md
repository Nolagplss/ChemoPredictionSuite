# 🔬 Chemical Prediction App

![Platform](https://img.shields.io/badge/platform-Windows-blue.svg)
![Status](https://img.shields.io/badge/status-en%20desarrollo%20%7C%20Linux%20y%20macOS%20pronto-orange)
![Tech](https://img.shields.io/badge/made_with-WPF%20%7C%20C%23%20%7C%20XAML%20%7C%20Python-blueviolet)
![Status](https://img.shields.io/badge/status-en%20desarrollo-orange)

Aplicación de escritorio desarrollada en **WPF con C# y XAML** que permite realizar predicciones químicas utilizando una API REST.  
Durante el proyecto también fue necesario crear y modificar funcionalidades de la API para que funcionara.

---

## 🚀 Características

- Interfaz de usuario desarrollada en WPF.
- Conexión con una API REST interna para predicciones químicas.
- Soporte para **8 modelos distintos**, cada uno con su propio formulario.
- Entrada de datos mediante **SMILES**, **CAS**, o **dibujando la molécula**.
- Visualización clara y estructurada de los resultados.

---

## 🔧 Ajustes realizados en la API

Durante el desarrollo de la aplicación fue necesario adaptar algunos aspectos de la API(desarrollada en Python) para asegurar una integración fluida y consistente. Esto incluyó tareas como:

- Estandarización del formato de las respuestas JSON.
- Validación adicional de los datos de entrada.
- Mejora en el manejo de errores y códigos de estado HTTP.
- Ajustes menores en algunos endpoints para un funcionamiento más predecible desde la app.

Estas modificaciones permitieron que la aplicación interactúe correctamente con los distintos modelos de predicción y maneje los resultados de forma clara para el usuario.

## 🧪 Modelos Implementados

Cada modelo cuenta con su propio formulario y lógica de procesamiento, aunque comparten una estructura común en la interfaz. Esto permitió reutilizar componentes y mantener un diseño coherente:

1. **DPPPredIV**
2. **G4mtQSAR**
3. **Paint4IRAS**
4. **SulfaTOX**
5. **MicotoXilico**
6. **ProtoAquaTox**
7. **EskaPred**
8. **DockTox** *(en desarrollo)*

---

## 🧱 Arquitectura y Tecnologías

- Backend en Python (Django) utilizado para las predicciones químicas y consumido desde la app.
- **Arquitectura MVVM** (Model-View-ViewModel), con separación clara entre lógica de presentación, negocio y datos.
- **Validación de entradas químicas** mediante expresiones regulares para **SMILES** y **CAS**, y soporte para entrada visual con **dibujado molecular**.
- **ClosedXML** para generación de informes Excel.
- Uso de librerías como **RDKit** (química computacional).
- Validaciones adicionales para asegurar que las entradas (SMILES, CAS, estructuras moleculares) fueran químicamente correctas.
- Reutilización de funciones comunes para evitar duplicación de código.
- Uso de principios de diseño como **SOLID**, **DRY** (Don't Repeat Yourself) y separación de responsabilidades.
- Organización modular por tipo de modelo químico.
- Mejoras en control de errores HTTP y serialización de respuestas.

---

## 🖼️ Capturas de Pantalla

### 🏠 Pantalla de Inicio

![Home](assets/Home.png)

---

### 🔐 Pantallas de Acceso

#### Acceso módulo DPPred  
![Acceso Dppred](assets/AccesDppred.png)

#### Acceso módulo G4MTQSAR  
![Acceso G4MTQSAR](assets/AccesG4mtqsar.png)

---

### 🔑 Login

#### Login en DPPred  
![Login Dppred](assets/LoginDppred.png)

#### Login en SulfaTOX  
![Login SulfaTOX](assets/LoginSulfaTOX.png)

---

### 📝 Registro

![Registro](assets/Registro.png)

---

### 🧪 Formulario y Resultado – Módulo DPPred

#### Formulario  
![Load File](assets/LoadFile.png)

#### Calculando
![Formulario Dppred](assets/Calculando.png)

#### Resultado  
![Resultado Dppred](assets/ResultadosDpppred.png)

---

### 🧬 Formulario y Resultado – Módulo G4MTQSAR

#### Formulario  
![Formulario G4MTQSAR](assets/FormularioG4mtqsar.png)

#### Descarga de Resultados  
![Descarga Resultados G4](assets/DescargaResultadosG4.png)

#### Resultados  
![Resultados G4MTQSAR](assets/ResultadosG4mtqsar.png)

---

### 🔬 Otros Formularios

#### Eskapred  
![Formulario Eskapred](assets/FormularioEskapred.png)

#### Paint4IRAS  
![Formulario Paint4IRAS](assets/FormularioPaint4IRAS.png)

#### Dibujar molécula 
![Dibujar molécula](assets/DibujarMolecula.png)

---

### ☣️ Formulario Especial – DockTox

#### Formulario DockTox  
![Formulario DockTox](assets/FormularioDocktox.png)
![Formulario DockTox](assets/CheckDockTox.png)

#### Selección del modelo  
![Modelo DockTox](assets/ModeloSeleccionadoDockTox.png)

#### Resultados DockTox  
![Resultado DockTox 1](assets/ResultadoDocTox.png)  
![Resultado DockTox 2](assets/ResultadoDockTox2.png)

---

### 📊 Módulo Micotoxilico

#### Selección específica  
![Micotoxilico](assets/Micotoxilico.png)

#### Vista general  
![Micotoxilico General](assets/MicotoxilicoGeneral.png)  
![Micotoxilico General 2](assets/MicotoxilicoGeneral2.png)

#### Base de datos  
![Micotoxilico Database](assets/MicotoxilicoDatabase.png)



---

## 👨‍💻 Autoría

Esta aplicación fue desarrollada íntegramente por mí durante mis prácticas profesionales, incluyendo:

- El diseño y desarrollo completo del cliente de escritorio (WPF + C#).
- La integración y adaptación con la API REST.
- Las mejoras técnicas necesarias en la API para su correcto funcionamiento con la app.

---

## 📦 Instalador

Cuando se publique la versión estable de la aplicación, se incluirá un instalador (.exe) en este repositorio para que pueda ser descargada y probada fácilmente.
