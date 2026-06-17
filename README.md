# Retinal Vessel Segmentation - ResU-Net Implementation

Proyek ini adalah pipeline lengkap untuk melakukan segmentasi pembuluh darah pada retina mata menggunakan **STARE Dataset**. Di sini, saya mengombinasikan arsitektur **ResNet50** (sebagai Encoder/Feature Extractor) dan **U-Net** (sebagai Decoder) yang biasa disebut dengan **ResU-Net**.

Proyek ini mencakup seluruh alur pengerjaan data, mulai dari pembacaan file medis mentah, teknik augmentasi data manual, hingga proses training model di Google Colab. Proyek ini dikembangkan untuk mendukung penelitian dosen di Program Studi Teknik Elektro Universitas Mulawarman (Unmul).

---

## Struktur Folder
pure-numpy-deep-learning/
├── README.md                  # Dokumentasi proyek
├── requirements.txt           # Library yang dibutuhkan (TensorFlow, OpenCV, dll)
│
├── preprocessing/
│   └── resize_and_clean.py    # Ekstrak .ppm.gz, normalisasi, & resize ke 224x224 px
│
├── data_augmentation/
│   └── image_augmentation.py  # Script augmentasi manual (Flip, Rotate, Brightness)
│
└── training_pipelines/
    └── training_resunet.ipynb # Notebook training model ResU-Net di Google Colab
