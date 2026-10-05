# Disease-detection-for-pumpkin

Flutter mobile app → FastAPI backend → EfficientNetB0 model → prediction → JSON response → Flutter result screen


disease-detection-for-pumpkin/
│
├── backend/
│   │
│   ├── app/
│   │   ├── __init__.py
│   │   ├── main.py
│   │   │
│   │   ├── api/
│   │   │   ├── __init__.py
│   │   │   └── disease_routes.py
│   │   │
│   │   ├── services/
│   │   │   ├── __init__.py
│   │   │   ├── model_service.py
│   │   │   └── prediction_service.py
│   │   │
│   │   ├── schemas/
│   │   │   ├── __init__.py
│   │   │   └── disease_schema.py
│   │   │
│   │   └── utils/
│   │       ├── __init__.py
│   │       └── image_utils.py
│   │
│   ├── models/
│   │   ├── best_pumpkin_disease_efficientnetb0.keras
│   │   └── class_names.txt
│   │
│   ├── uploads/
│   │
│   ├── requirements.txt
│   ├── .env
│   └── run.py
│
├── mobile/
│   └── pumpkin_disease_app/
│       │
│       ├── android/
│       ├── ios/
│       ├── lib/
│       │   ├── main.dart
│       │   │
│       │   ├── core/
│       │   │   ├── constants/
│       │   │   │   ├── api_constants.dart
│       │   │   │   └── app_colors.dart
│       │   │   │
│       │   │   └── theme/
│       │   │       └── app_theme.dart
│       │   │
│       │   ├── models/
│       │   │   └── disease_result.dart
│       │   │
│       │   ├── services/
│       │   │   ├── api_service.dart
│       │   │   └── image_service.dart
│       │   │
│       │   ├── screens/
│       │   │   ├── home_screen.dart
│       │   │   ├── camera_screen.dart
│       │   │   ├── result_screen.dart
│       │   │   └── history_screen.dart
│       │   │
│       │   ├── widgets/
│       │   │   ├── disease_card.dart
│       │   │   ├── confidence_bar.dart
│       │   │   └── image_preview.dart
│       │   │
│       │   └── routes/
│       │       └── app_routes.dart
│       │
│       ├── assets/
│       │   └── images/
│       │
│       └── pubspec.yaml
│
├── README.md
└── .gitignore
