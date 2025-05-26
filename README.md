# Patates Sağlık Analiz Sistemi

Bu proje, patates bitkilerinin sağlık durumunu yapay zeka kullanarak analiz eden bir web uygulamasıdır. Sistem, patates yapraklarının fotoğraflarını analiz ederek erken yanıklık (Early Blight), geç yanıklık (Late Blight) ve sağlıklı durumları tespit edebilmektedir.

## Proje Mimarisi

Proje üç ana bileşenden oluşmaktadır:

### 1. Backend (API)
- FastAPI framework'ü kullanılarak geliştirilmiştir
- TensorFlow modeli entegre edilmiştir
- RESTful API endpoints:
  - `/ping`: API'nin çalışır durumda olduğunu kontrol etmek için
  - `/predict`: Patates yaprağı fotoğrafını analiz etmek için
- CORS desteği ile frontend ile güvenli iletişim sağlanmıştır

### 2. Frontend
- React.js ile geliştirilmiştir
- Material-UI kullanılarak modern bir arayüz tasarlanmıştır
- Özellikler:
  - Sürükle-bırak dosya yükleme
  - Gerçek zamanlı görüntü analizi
  - Kullanıcı dostu arayüz
  - Responsive tasarım

### 3. Model
- TensorFlow/Keras ile geliştirilmiş derin öğrenme modeli
- Üç sınıf sınıflandırması:
  - Early Blight (Erken Yanıklık)
  - Late Blight (Geç Yanıklık)
  - Healthy (Sağlıklı)
- Model dosyaları:
  - `models/4.keras`: Ana model dosyası
  - Diğer model versiyonları farklı eğitim aşamalarını temsil etmektedir

## Teknik Detaylar

### Backend Gereksinimleri
- Python 3.x
- FastAPI
- TensorFlow
- Uvicorn
- NumPy
- Pillow

### Frontend Gereksinimleri
- Node.js
- React 17.0.2
- Material-UI 4.11.4
- Axios
- Material-UI-Dropzone

## Geliştirme Süreci

1. Model Geliştirme:
   - Patates yaprağı görüntüleri ile eğitilmiş derin öğrenme modeli
   - Transfer learning teknikleri kullanılmıştır
   - Model performansı optimize edilmiştir

2. API Geliştirme:
   - FastAPI ile RESTful API tasarımı
   - Asenkron işlem desteği
   - Güvenli dosya işleme
   - CORS yapılandırması

3. Frontend Geliştirme:
   - Modern React uygulaması
   - Material-UI ile kullanıcı arayüzü
   - Sürükle-bırak dosya yükleme
   - API entegrasyonu

## Güvenlik Özellikleri
- CORS koruması
- Güvenli dosya işleme
- API rate limiting
- Input validasyonu

## Performans Optimizasyonları
- Asenkron API işlemleri
- Optimize edilmiş model yükleme
- Frontend bundle optimizasyonu
- Lazy loading implementasyonu 



# Potato Health Analysis System

This project is a web application that analyzes the health status of potato plants using artificial intelligence. The system can detect early blight, late blight, and healthy conditions by analyzing photos of potato leaves.

## Project Architecture

The project consists of three main components:

### 1. Backend (API)
- Developed using FastAPI framework
- Integrated TensorFlow model
- RESTful API endpoints:
  - `/ping`: To check if the API is operational
  - `/predict`: To analyze potato leaf photos
- Secure communication with frontend through CORS support

### 2. Frontend
- Developed with React.js
- Modern interface designed using Material-UI
- Features:
  - Drag-and-drop file upload
  - Real-time image analysis
  - User-friendly interface
  - Responsive design

### 3. Model
- Deep learning model developed with TensorFlow/Keras
- Three-class classification:
  - Early Blight
  - Late Blight
  - Healthy
- Model files:
  - `models/4.keras`: Main model file
  - Other model versions represent different training stages

## Technical Details

### Backend Requirements
- Python 3.x
- FastAPI
- TensorFlow
- Uvicorn
- NumPy
- Pillow

### Frontend Requirements
- Node.js
- React 17.0.2
- Material-UI 4.11.4
- Axios
- Material-UI-Dropzone

## Development Process

1. Model Development:
   - Deep learning model trained with potato leaf images
   - Transfer learning techniques used
   - Model performance optimized

2. API Development:
   - RESTful API design with FastAPI
   - Asynchronous operation support
   - Secure file handling
   - CORS configuration

3. Frontend Development:
   - Modern React application
   - User interface with Material-UI
   - Drag-and-drop file upload
   - API integration

## Security Features
- CORS protection
- Secure file handling
- API rate limiting
- Input validation

## Performance Optimizations
- Asynchronous API operations
- Optimized model loading
- Frontend bundle optimization
- Lazy loading implementation 