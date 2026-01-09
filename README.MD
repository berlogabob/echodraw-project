```
EchoDraw/
├── .github/                # CI/CD и шаблоны
│   └── workflows/          # GitHub Actions YAML для тестов
│       └── ci.yml          # Пример: build для Flutter, lint для p5.js
├── docs/                   # Модуль документации и отчётов
│   ├── README.md           # Обзор docs: как генерировать отчёты
│   ├── mkdocs.yml          # Конфиг для MkDocs (сайт из Markdown)
│   ├── reports/            # Отчёты: progress logs, specs
│   │   └── stage1-report.md # Пример: Отчёт по этапу 1
│   ├── bom/                # Bill of Materials (CSV/Excel для компонентов)
│   │   └── hardware-bom.csv
│   └── images/             # Скриншоты, диаграммы для docs
├── hardware/               # Модуль 1: Аппаратная часть
│   ├── README.md           # Инструкции: сборка, pinout NEJE
│   ├── configs/            # YAML для FluidNC
│   │   └── config.yaml     # Базовый config для TMC2209
│   ├── designs/            # 3D-модели (STL, CAD из Fusion360/Tinkercad)
│   │   └── pen-holder.stl  # Держатель для single-pen
│   ├── firmware/           # Прошивки (если кастом)
│   └── tests/              # G-code примеры для тестов
│       └── test-line.gcode
├── generative-core/        # Модуль 2: p5.js + ml5.js
│   ├── README.md           # Как запустить: npm install, etc.
│   ├── src/                # Код: sketches, libraries
│   │   ├── index.html      # Базовый p5.js canvas
│   │   ├── sketch.js       # Генератор паттернов (этап 1)
│   │   └── ml-integration.js # ml5.js для handpose
│   ├── examples/           # Примеры паттернов (SVG/G-code)
│   └── package.json        # Зависимости (p5, ml5)
├── flutter-app/            # Модуль 3: Flutter обёртка
│   ├── README.md           # Flutter setup: flutter pub get
│   ├── lib/                # Код: main.dart, screens
│   │   └── main.dart       # Базовое app (этап 1)
│   ├── assets/             # Иконки, изображения
│   └── pubspec.yaml        # Зависимости Flutter
├── .gitignore              # Игнор: build/, .DS_Store, etc.
├── LICENSE                 # MIT текст
├── README.md               # Главный: Обзор проекта, структура, как запустить
└── CONTRIBUTING.md         # Правила вклада (для группы)
```
