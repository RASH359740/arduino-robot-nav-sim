# Arduino Differential Drive Robot

## О проекте

Мобильный робот с **дифференциальным приводом** на Arduino.  
В проекте работают три инженера:

- **Robotics Platform Engineer** — Arduino, моторы, энкодеры, IMU, Serial
- **Navigation Engineer** — одометрия, PID, фильтрация, wall-following, Bug-алгоритмы
- **Simulation & Infrastructure Engineer** — структура проекта, веб-интерфейс, калибровка, визуализация, ручной режим, запись видео

## Структура проекта

```bash
arduino-robot-nav-sim/
├── arduino/                    ← код для Arduino
├── python/
│   ├── serial_interface.py     ← главный скрипт (Serial)
│   ├── calibration/            ← калибровка колёс и IMU
│   ├── navigation/             ← одометрия и навигация
│   └── visualization/          ← построение карты и траектории
├── interface/
│   ├── web/                    ← Streamlit-приложение (статус робота)
│   └── manual/                 ← ручной режим
├── simulation/
├── docs/
├── data/                       ← логи, карты, видео
├── requirements.txt
└── README.md
```
