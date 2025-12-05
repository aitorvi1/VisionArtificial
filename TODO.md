# Plan de práctica en Visión Artificial (versión mejorada)

## Bloque 0: Entorno y herramientas
- [x] Configurar entorno (Python 3.11+, `pip`, `venv`, Git, VS Code/PyCharm).
- [x] Instalar dependencias base (`opencv-python`, `numpy`, `matplotlib`, `scikit-image`, `jupyter`).
- [x] Crear estructura de carpetas (src/, notebooks/, data/raw–processed/, outputs/).
- [ ] Preparar dataset de prueba pequeño (imágenes + vídeos).

## Bloque 0.5: Gestión de datos y etiquetado
- [ ] Organización de datasets (train/val/test, evitar leakage).
- [ ] Herramientas de etiquetado (LabelImg, CVAT, Roboflow).
- [ ] Data augmentation clásica y para DL (flips, brillo, blur, crops, rotaciones).
- [ ] Práctica: etiquetar un mini dataset propio.

## Bloque 1: Fundamentos de imagen
- [ ] Cargar/mostrar imágenes (BGR↔RGB, guardado).
- [ ] Canales y formatos (grises, binaria, HSV/Lab; resize, crop, padding).
- [ ] Ajustes de intensidad (brillo/contraste, gamma, histogramas, CLAHE).
- [ ] Filtros (blur, Gaussian, median, bilateral) y análisis del ruido.
- [ ] Bordes y gradientes (Sobel, Scharr, Canny).

**Mini proyecto**
- [ ] Detector de bordes interactivo (sliders para thresholds).

## Bloque 2: Geometría y transformaciones
- [ ] Transformaciones geométricas (rotación, escalado, traslación, affine, perspectiva).
- [ ] Interpolaciones (nearest, bilinear, bicubic).
- [ ] Detección de formas y líneas (Hough líneas/círculos, contornos, bounding boxes rotadas).
- [ ] Estimación geométrica: calibración de cámara, distorsión, pose con PnP, triangulación básica.

## Bloque 3: Primer contacto con modelos preentrenados
- [ ] Inferencia con YOLO preentrenado (detección en imágenes/vídeo).
- [ ] MediaPipe: manos, rostro, pose.
- [ ] OCR con easyocr + preprocesado clásico.
- [ ] Comparación de pipelines clásicos vs DL.

## Bloque 4: Morfología y segmentación clásica
- [ ] Operaciones morfológicas (erode, dilate, open, close, gradiente, top-hat).
- [ ] Segmentación clásica (umbralizado global/adaptativo/Otsu, watershed).
- [ ] Connected components y filtrado por área/perímetro.

**Mini proyecto**
- [ ] Contador de objetos en cinta transportadora.

## Bloque 5: Características y emparejamiento
- [ ] Detectores y descriptores (Harris, FAST, SIFT/SURF/ORB).
- [ ] Matching (Brute Force, FLANN).
- [ ] Homografía con RANSAC.
- [ ] Stitching panorámico simple.

## Bloque 6: Movimiento y seguimiento clásico
- [ ] Flujo óptico (Lucas-Kanade sparse, Farnebäck dense).
- [ ] Trackers clásicos (CSRT, KCF).
- [ ] Multi-objeto básico (detección + tracking; métricas MOT).

**Mini proyecto**
- [ ] Seguimiento de balón o marcador de color en vídeo.

## Bloque 7A: Detección y análisis clásico de objetos
- [ ] Detección de rostros/personas con Haar Cascades.
- [ ] HOG + SVM para personas u objetos.
- [ ] Detección de formas específicas (placas simples, balones, marcadores de color).

## Bloque 7B: Modelos preentrenados avanzados
- [ ] Keypoints humanos con MediaPipe/OpenPose-lite (métricas PCK).
- [ ] OCR avanzado con easyocr (pipeline mejorado).
- [ ] Reconocimiento facial práctico (InsightFace/ArcFace en modo inferencia).
- [ ] Comparación clásico vs DL por tareas.

**Mini proyecto**
- [ ] Detector de placas + OCR (preprocesado + easyocr).

## Bloque 8: Deep Learning práctico
- [ ] DataLoaders, batching, shuffle, transformaciones.
- [ ] Training loop + validación.
- [ ] Logging con TensorBoard.
- [ ] Checkpoints, early stopping.
- [ ] Regularización (dropout, weight decay).
- [ ] Configs reproducibles (semillas, YAML).

## Bloque 9: Deep Learning para visión
- [ ] Transfer learning/Fine-tuning (MobileNet/EfficientNet).
- [ ] Entrenamiento de detectores (YOLO/SSD) en dataset pequeño.
- [ ] Segmentación (U-Net, DeepLab, Mask R-CNN).
- [ ] Restauración: denoise, deblur, super-res (PSNR/SSIM).

**Mini proyectos**
- [ ] Clasificador de gestos con webcam.
- [ ] Segmentación de personas + recorte de fondo.

## Bloque 10: Rendimiento y despliegue
- [ ] Optimización en tiempo real (profiling, reducción de resolución, cuantización).
- [ ] Exportación a ONNX/TFLite.
- [ ] API REST (FastAPI/Flask).
- [ ] Interfaz visual (Gradio/Streamlit).
- [ ] Consideraciones para edge (CPU vs GPU, latencia, memoria).

## Bloque 11: Proyectos integradores
- [ ] Sistema de conteo en cinta (detección + tracking + API + dashboard).
- [ ] Control de acceso (detección/identificación de persona o matrícula).
- [ ] Segmentación de persona con fondo dinámico.
- [ ] Pipeline propio: captura → etiquetado → entrenamiento → despliegue.

## Bloque 12: Documentación y métricas
- [ ] Métricas: PSNR/SSIM, accuracy/F1, precision–recall, mAP, curvas PR/ROC.
- [ ] Matrices de confusión.
- [ ] Reportes de experimentos (logs y comparaciones).
- [ ] Notas y aprendizajes por módulo.

