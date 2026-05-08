# weather-station
weather station based on a pi zero w2, software developed with Claude
weather_station_v2/
│
├── main.py                  ← 100 lines — the only file you need to read daily
├── config.py                ← all settings in one place (unchanged)
├── mqtt_publisher.py        ← all MQTT and Home Assistant logic
├── requirements.txt
├── weather_station.service
│
└── sensors/
    ├── __init__.py
    ├── bme280.py            ← BME280Sensor
    ├── anemometer.py        ← Anemometer + SimulatedAnemometer
    ├── wind_vane.py         ← ADS1115ADC + WindVane + SimulatedWindVane
    └── rain_gauge.py        ← RainGauge + SimulatedRainGauge
