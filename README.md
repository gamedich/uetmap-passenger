# УЭТ Карты — Android Passenger App 🚋📱

> Официальное мобильное приложение для пассажиров городского электротранспорта города Ульяновска.

[![Android Release](https://img.shields.io/badge/release-v1.0.2--beta-blue.svg)](https://github.com/gamedich/uetmap-passenger/releases/tag/v1.0.2-beta)
[![Platform](https://img.shields.io/badge/platform-Android%208.0%2B-green.svg)](https://github.com/gamedich/uetmap-passenger)
[![Web Version](https://img.shields.io/badge/web-uet--map.ru-orange.svg)](https://uet-map.ru/)

---

## 📌 Overview

**UETMap Passenger App** — нативное Android-приложение для удобного и быстрого доступа к интерактивной карте трамваев и троллейбусов Ульяновска непосредственно с экрана смартфона. Позволяет оперативно проверять местоположение транспорта, отслеживать схемы объездов и находить ближайшие остановочные пункты без необходимости открывать браузер.

* **Скачать APK:** [GitHub Release v1.0.2-beta](https://github.com/gamedich/uetmap-passenger/releases/tag/v1.0.2-beta)
* **Веб-версия карты:** [https://uet-map.ru/](https://uet-map.ru/)
* **Канал новостей и обновлений:** [t.me/uet_maps](https://t.me/uet_maps)

---

## 🚀 Key Features

* **⚡ Мгновенный запуск:** предварительно упакованные ассеты интерфейса ускоряют холодный старт карты на мобильном устройстве.
* **📍 Пассажирская навигация:** просмотр остановок, трассировки маршрутов, времени работы и статуса движения по графику.
* **🚧 Оповещения об изменениях:** оперативные предупреждения о ремонтах путей, перекрытиях и временных схемах движения.
* **📱 Мобильная эргономика:** оптимизированное жестовое управление нижними карточками (bottom sheet) и поддержка мобильных экранов с разной плотностью пикселей.

---

## 🏛️ Architecture & Relationship with Web

Приложение построено по архитектуре гибридного легковесного клиента:
* **Native Shell (Java / Android SDK):** отвечает за жизненный цикл активности, управление аппаратными кнопками, безопасное взаимодействие с сетевыми протоколами и работу с полноэкранным режимом.
* **Bundled Web Engine:** встроенный оптимизированный клиент карты на базе Leaflet GIS, использующий те же проверенные алгоритмы, что и [UETMap Web Client](https://github.com/gamedich/uetmap-web-client).
* **Сетевая синхронизация:** данные о положении транспорта и активных объездах подгружаются по защищенному протоколу с основного сервера `uet-map.ru`.

---

## 🛠️ Technology Stack

* **Язык разработки:** Java 17 / Android SDK.
* **Сборка:** Gradle (Android Application Plugin).
* **Минимальная версия:** Android 8.0 (API Level 26) и выше.
* **Внутренний UI:** Leaflet GIS, HTML5, CSS3, ES6 JavaScript.

---

## 📦 Installation

Готовый установочный пакет APK доступен в разделе релизов репозитория:
1. Перейдите на страницу релиза: [v1.0.2-beta Release](https://github.com/gamedich/uetmap-passenger/releases/tag/v1.0.2-beta).
2. Загрузите файл `uet_tram_passenger_beta.apk`.
3. Установите на устройство Android (при необходимости разрешите установку из доверенных источников).

---

## 🚦 Project Status

Приложение находится в стадии активного открытого бета-тестирования (**Public Beta**). Замечания и предложения принимаются в официальном канале [@uet_maps](https://t.me/uet_maps).
