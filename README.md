# raspberry-lab-hardware
Repozytorium raspberry-hardware-lab to platforma testowa dla modułów sprzętowych kompatybilnych z Raspberry Pi, zawierająca kod źródłowy, narzędzia kalibracyjne, testy i dokumentację dla różnych komponentów. Skupia się na modularności, automatyzacji testów i łatwości integracji nowych elementów.


## Template:
```bash
raspberry-hardware-lab/
├── README.md                # Ogólny opis projektu
├── requirements.txt         # Lista zależności Pythona
├── .gitignore               # Ignorowanie wyników i środowiska wirtualnego
├── tools/                   # Narzędzia wspólne dla modułów
│   ├── utils.py             # Funkcje pomocnicze (np. parsowanie JSON)
│   ├── logging.py           # Narzędzia do logowania
│   └── calibration_utils.py # Funkcje wspólne do kalibracji
├── modules/                 # Moduły sprzętowe
│   ├── gps/                 # Moduł GPS
│   │   ├── docs/            # Dokumentacja specyficzna dla GPS
│   │   │   ├── usage.md     # Jak używać modułu GPS
│   │   │   └── setup.md     # Jak podłączyć i skonfigurować GPS
│   │   ├── results/         # Wyniki generowane przez moduł GPS
│   │   │   ├── gps_test_results.json
│   │   │   └── gps_logs.txt
│   │   ├── src/
│   │   │   ├── gps_module.py         # Klasa obsługująca GPS
│   │   │   ├── gps_calibration.py    # Klasa do kalibracji GPS
│   │   │   └── __init__.py
│   │   ├── tests/
│   │   │   ├── test_gps_module.py    # Testy jednostkowe modułu GPS
│   │   │   └── test_gps_calibration.py
│   │   └── data/
│   │       ├── calibration_data.json # Dane kalibracyjne GPS
│   │       └── sample_gps_data.txt   # Przykładowe dane GPS
│   ├── imu/                 # Moduł IMU
│   │   ├── docs/            # Dokumentacja specyficzna dla IMU
│   │   │   ├── usage.md
│   │   │   └── setup.md
│   │   ├── results/
│   │   │   ├── imu_test_results.csv
│   │   │   └── imu_logs.txt
│   │   ├── src/
│   │   │   ├── imu_module.py
│   │   │   ├── imu_calibration.py
│   │   │   └── __init__.py
│   │   ├── tests/
│   │   │   ├── test_imu_module.py
│   │   │   └── test_imu_calibration.py
│   │   └── data/
│   │       ├── calibration_data.json
│   │       └── sample_imu_data.txt
│   └── ...                 # Dodaj kolejne moduły w podobnej strukturze
├── scripts/                 # Skrypty pomocnicze
│   ├── test_all.py          # Skrypt uruchamiający wszystkie testy
│   ├── generate_report.py   # Skrypt generujący raporty z testów
│   └── start_hardware.py    # Główny skrypt startowy dla modułów
└── tests/                   # Testy integracyjne
    ├── test_integration.py  # Testy komunikacji między modułami
    └── test_system.py       # Testy całego systemu
```
