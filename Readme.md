# Análisis Visual con IA

**Plataforma inteligente de análisis de imágenes utilizando Machine Learning y redes neuronales**

## Sobre el Proyecto

**Análisis Visual con IA** es una aplicación web full-stack que permite analizar imágenes utilizando modelos de **Machine Learning**. El sistema puede detectar objetos, clasificar imágenes y extraer texto mediante OCR, todo procesado con redes neuronales pre-entrenadas.

## Tecnologías

### Backend
- **Node.js** - Entorno de ejecución JavaScript
- **MongoDB Atlas** - Base de datos NoSQL en la nube para almacenamiento de imágenes
- **TensorFlow.js** - Machine Learning en JavaScript
- **COCO-SSD** - Detección de objetos (90 categorías)
- **MobileNet** - Clasificación de imágenes (1000 categorías)
- **Tesseract.js** - OCR (Reconocimiento óptico de caracteres)
- **Jimp** - Procesamiento de imágenes
- **Firebase Authentication** - Autenticación de usuarios

### Herramientas de Desarrollo
- **[dotenv](https://github.com/motdotla/dotenv)** - Variables de entorno
- **[CORS](https://github.com/expressjs/cors)** - Políticas de origen cruzado
- **[Nodemon](https://nodemon.io/)** - Auto-reload en desarrollo

---

## Características

### Análisis con Machine Learning
- **Detección de objetos** - Identifica hasta 90 tipos de objetos usando COCO-SSD
- **Clasificación de imágenes** - Clasifica imágenes en 1000 categorías con MobileNet
- **OCR (Reconocimiento de texto)** - Extrae texto visible en español con Tesseract.js
- **Análisis en paralelo** - Ejecuta los 3 modelos simultáneamente para mayor velocidad

### Interfaz de Usuario
- **Drag & Drop** - Arrastra imágenes directamente
- **Preview en tiempo real** - Visualiza la imagen antes de analizar
- **Resultados detallados** - Descripción, objetos, etiquetas y texto detectado
- **Diseño responsivo** - Funciona en desktop, tablet y móvil
- **Animaciones fluidas** - Transiciones y estados de carga elegantes

### Seguridad & Autenticación
- **Firebase Authentication** - Login seguro con Google y email
- **JWT Tokens** - Autenticación mediante tokens
- **Sesiones persistentes** - Mantiene la sesión del usuario
- **Protección de rutas** - Solo usuarios autenticados pueden analizar

### Flujo de Datos
1. Usuario sube imagen → Frontend la convierte a Base64
2. Frontend envía petición con token JWT → Servidor valida autenticación
3. Servidor guarda imagen en MongoDB → Retorna ID de imagen
4. Servidor procesa con ML Service:
   - **COCO-SSD**: Detecta objetos
   - **MobileNet**: Clasifica imagen
   - **Tesseract**: Extrae texto
5. Resultados se guardan en MongoDB
6. Servidor retorna análisis completo al cliente
7. Frontend muestra resultados visualizados

## Contacto

**Yessetk Rodriguez**

- GitHub: [@yessetkr21](https://github.com/yessetkr21)
- Email: yessetkr2190@gmail.com
