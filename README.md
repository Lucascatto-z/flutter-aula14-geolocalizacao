# 📍 Check-in & GPS — Geolocalização com Flutter

Aplicativo desenvolvido na disciplina de **Programação para Dispositivos Móveis I** (Aula 14). O projeto demonstra a integração com os sensores físicos de localização do smartphone utilizando o pacote oficial `geolocator`.

---

## 🚀 Funcionalidades

* **Validação de Serviço e Permissões:** Verifica se o GPS do dispositivo está ativo e gerencia permissões nativas (`ACCESS_FINE_LOCATION` e `ACCESS_COARSE_LOCATION`) de forma defensiva.
* **Captura Única de Coordenadas:** Obtém Latitude, Longitude, Precisão (em metros) e Altitude sob demanda (`getCurrentPosition`).
* **Rastreamento Contínuo:** Monitora atualizações de localização em tempo real conforme o deslocamento do usuário (`getPositionStream` com filtro de 10 metros).

---

## 🛠️ Tecnologias Utilizadas

* **Flutter & Dart SDK**
* **Pacote:** [`geolocator: ^11.0.0`](https://pub.dev/packages/geolocator)

---

## 📁 Estrutura do Projeto

```text
lib/
├── screens/
│   └── geolocalizacao_screen.dart  # Interface gráfica e controle de estado do GPS
├── services/
│   └── location_service.dart       # Camada de serviço e validação de permissões
└── main.dart                       # Ponto de entrada da aplicação
