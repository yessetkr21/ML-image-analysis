# AI Visual Analysis

**Intelligent image analysis platform using Machine Learning and neural networks**

### Project Link  

---

## About the Project

**AI Visual Analysis** is a full-stack web application that allows users to analyze images using **Machine Learning** models. The system can detect objects, classify images, and extract text using OCR, all processed with pre-trained neural networks.

---

## Technologies

### Backend
- **Node.js** - JavaScript runtime environment  
- **MongoDB Atlas** - Cloud-based NoSQL database for image storage  
- **TensorFlow.js** - Machine Learning in JavaScript  
- **COCO-SSD** - Object detection (90 categories)  
- **MobileNet** - Image classification (1000 categories)  
- **Tesseract.js** - OCR (Optical Character Recognition)  
- **Jimp** - Image processing  
- **Firebase Authentication** - User authentication  

### Development Tools
- **dotenv** - Environment variables  
- **CORS** - Cross-origin resource policies  
- **Nodemon** - Auto-reload in development  

---

## Features

### Machine Learning Analysis
- **Object detection** - Identifies up to 90 object types using COCO-SSD  
- **Image classification** - Classifies images into 1000 categories with MobileNet  
- **OCR (Text Recognition)** - Extracts visible Spanish text using Tesseract.js  
- **Parallel processing** - Runs all 3 models simultaneously for higher speed  

### User Interface
- **Drag & Drop** - Drag images directly  
- **Real-time preview** - View the image before analyzing  
- **Detailed results** - Description, objects, labels, and detected text  
- **Responsive design** - Works on desktop, tablet, and mobile  
- **Smooth animations** - Elegant transitions and loading states  

### Security & Authentication
- **Firebase Authentication** - Secure login with Google and email  
- **JWT Tokens** - Token-based authentication  
- **Persistent sessions** - Maintains user sessions  
- **Route protection** - Only authenticated users can analyze  

---

## Data Flow
1. User uploads image → Frontend converts it to Base64  
2. Frontend sends request with JWT token → Server validates authentication  
3. Server stores image in MongoDB → Returns image ID  
4. Server processes with ML Service:
   - **COCO-SSD**: Detects objects  
   - **MobileNet**: Classifies image  
   - **Tesseract**: Extracts text  
5. Results are stored in MongoDB  
6. Server returns full analysis to the client  
7. Frontend displays visualized results  

---

## Contact

**Yessetk Rodriguez**

- GitHub: https://github.com/yessetkr21  
- Email: yessetkr2190@gmail.com
