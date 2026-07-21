# 🎵 MusicToolsHub Pro

**Advanced Music Device Manager with AI Orchestration**

MusicToolsHub to zaawansowany system do zarządzania urządzeniami muzycznymi na Windows 11 z wbudowanym AI do aranżacji, automatycznym wykrywaniem urządzeń, pobieraniem sterowników i wyszukiwaniem bibliotek muzycznych.

## 🎯 Główne Funkcje

### 1. **Automatyczne Wykrywanie Urządzeń**
- Detekcja podłączonych urządzeń muzycznych w rzeczywistym czasie
- Obsługiwane urządzenia:
  - Native Instruments Maschine MK2
  - M-Audio SMC-Pad
  - Akai MPK mini

### 2. **Zarządzanie Sterownikami**
- Automatyczne pobieranie najnowszych sterowników
- Weryfikacja bezpieczeństwa plików (VirusTotal API)
- Instalacja i aktualizacja sterowników
- Okresowe sprawdzanie aktualizacji

### 3. **Wyszukiwarka Muzyczna Pro**
- Samples, MIDI, Loops, Presets
- Filtry zaawansowane
- Integracja z:
  - Freesound.org API
  - Zenodo
  - Własna baza danych

### 4. **AI Orchestration**
- Lokalne AI (Ollama + open-source modele)
- Wsparcie OpenAI API (ChatGPT)
- Pomoc w aranżacji w czasie rzeczywistym
- Analiza przykładów, tekstu i mowy

### 5. **Interfejs Graficzny**
- Główne okno z przeglądem wszystkich urządzeń
- Oddzielne zakładki dla każdego urządzenia
- Wizualizacja funkcji i opcji
- Skróty klawiaturowe
- Drzewo wyszukiwania instrukcji i rozwiązań

### 6. **Bezpieczeństwo**
- Weryfikacja plików przez VirusTotal
- Skanowanie w tle
- Bezpieczne pobieranie z zaufanych źródeł

## 📦 Wymagania

- Windows 11
- Python 3.10+
- Internet connection
- (Opcjonalnie) API keys: OpenAI, Freesound.org

## 🚀 Instalacja

```bash
# Klonowanie repozytorium
git clone https://github.com/lukaszkowalsky0/MusicToolsHub.git
cd MusicToolsHub

# Instalacja zależności
pip install -r requirements.txt

# Uruchomienie
python -m src.main
```

## 📂 Struktura Projektu

```
MusicToolsHub/
├── src/
│   ├── core/
│   │   ├── device_detector.py      # Wykrywanie urządzeń
│   │   ├── driver_manager.py       # Zarządzanie sterownikami
│   │   ├── virus_scanner.py        # Weryfikacja bezpieczeństwa
│   │   ├── ai_orchestrator.py      # AI w czase rzeczywistym
│   │   └── config_manager.py       # Konfiguracja
│   ├── ui/
│   │   ├── main_window.py          # Główne okno aplikacji
│   │   ├── device_tabs.py          # Zakładki urządzeń
│   │   ├── search_interface.py     # Wyszukiwarka muzyczna
│   │   └── ai_panel.py             # Panel AI
│   ├── plugins/
│   │   ├── native_instruments_maschine.py
│   │   ├── m_audio_smc_pad.py
│   │   ├── akai_mpk_mini.py
│   │   └── base_device.py
│   ├── services/
│   │   ├── downloader.py           # Pobieranie plików
│   │   ├── freesound_api.py        # Integracja Freesound
│   │   ├── zenodo_api.py           # Integracja Zenodo
│   │   └── local_db_manager.py     # Baza danych lokalna
│   ├── utils/
│   │   ├── logger.py               # Logowanie
│   │   ├── validators.py           # Walidacja
│   │   └── helpers.py              # Funkcje pomocnicze
│   ├── resources/
│   │   ├── icons/
│   │   ├── styles/
│   │   └── instructions/
│   └── main.py                     # Punkt wejścia
├── data/
│   ├── device_profiles/            # Profile urządzeń
│   ├── instructions/               # Instrukcje urządzeń
│   ├── samples/                    # Cache samples
│   └── midi/                       # Cache MIDI
├── config/
│   ├── config.yaml                 # Konfiguracja główna
│   ├── devices.yaml                # Konfiguracja urządzeń
│   └── api_keys.example            # Szablon API keys
├── tests/
│   ├── test_device_detector.py
│   ├── test_driver_manager.py
│   └── test_virus_scanner.py
├── requirements.txt                # Zależności
├── setup.py                        # Skrypt instalacyjny
├── build_exe.py                    # Budowanie .exe
└── .gitignore                      # Git ignore

```

## 🔧 Obsługiwane Urządzenia

| Urządzenie | Producent | Status |
|-----------|----------|--------|
| Maschine MK2 | Native Instruments | ✅ Planowane |
| SMC-Pad | M-Audio | ✅ Planowane |
| MPK mini | Akai | ✅ Planowane |

## 🤖 AI Features

- **Ollama Local**: Open-source LLM na komputerze
- **OpenAI API**: ChatGPT dla zaawansowanych funkcji
- **Rzeczywisty czas**: Analiza i sugestie na żywo
- **Aranżacja**: Pomoc w tworzeniu muzyki

## 🔐 Bezpieczeństwo

- VirusTotal API dla weryfikacji plików
- Skanowanie w tle
- Sandboxing pobieranych sterowników
- Logi wszystkich operacji

## 📝 Licencja

MIT License - Otwarte oprogramowanie

## 🤝 Wspólny Rozwój

Chętnie przyjmujemy:
- Bug reports
- Feature requests
- Pull requests
- Dokumentację

## 📞 Kontakt

- GitHub Issues: [Issues](https://github.com/lukaszkowalsky0/MusicToolsHub/issues)
- Dyskusje: [Discussions](https://github.com/lukaszkowalsky0/MusicToolsHub/discussions)

---

**Status**: 🔨 W Rozwoju | Ostatnia aktualizacja: 2026-07-21
