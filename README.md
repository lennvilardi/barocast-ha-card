# Barocast HA Card (HACS Dashboard)

Custom Lovelace card for the **Barocast HA** integration.

## Breaking change (sensor IDs)
- Default entity IDs are now in the `sensor.barocast_forecast*` namespace.
- Update existing card configs if they still reference `sensor.local_forecast*`.

## Features
- Clear 3-block layout: now / next slot / later slot
- Forecast text, pressure trend and rain probabilities
- Defensive rendering when entities are unavailable at startup
- Language labels derived from integration language index
- Polished visual style (gradients + card sections)

## Requirements
- Home Assistant
- Integration sensors:
  - `sensor.barocast_forecast`
  - `sensor.barocast_forecast_zambretti_detail`
  - `sensor.barocast_forecast_pressure_change`

## Installation with HACS
1. HACS → menu (⋮) → **Custom repositories**.
2. Add this repository URL.
3. Category: **Dashboard** (backend HACS: plugin).
4. Install **Barocast HA Card**.
5. Reload browser cache.

## Card configuration

```yaml
type: custom:barocast-ha-card
entity: sensor.barocast_forecast
detail_entity: sensor.barocast_forecast_zambretti_detail
pressure_change_entity: sensor.barocast_forecast_pressure_change
```

## Optional configuration

```yaml
type: custom:barocast-ha-card
entity: sensor.barocast_forecast
detail_entity: sensor.barocast_forecast_zambretti_detail
pressure_change_entity: sensor.barocast_forecast_pressure_change
icon_now: mdi:weather-cloudy-clock
```

## Notes
- This card is read-only and displays values produced by the integration.
- Missing values are rendered as `-` until sensors are available.

---

# Version Française

Carte Lovelace custom pour l’intégration **Barocast HA**.

## Changement majeur (IDs capteurs)
- Les IDs d’entités par défaut sont désormais dans l’espace `sensor.barocast_forecast*`.
- Mets à jour les configurations de carte existantes si elles référencent encore `sensor.local_forecast*`.

## Fonctionnalités
- Mise en page claire en 3 blocs : maintenant / prochain créneau / créneau suivant
- Texte de prévision, tendance de pression et probabilités de pluie
- Rendu robuste quand les entités sont indisponibles au démarrage
- Libellés de langue basés sur l’index de langue de l’intégration
- Style visuel amélioré (dégradés + sections de carte)

## Prérequis
- Home Assistant
- Capteurs de l’intégration :
  - `sensor.barocast_forecast`
  - `sensor.barocast_forecast_zambretti_detail`
  - `sensor.barocast_forecast_pressure_change`

## Installation via HACS
1. HACS → menu (⋮) → **Dépôts personnalisés**.
2. Ajoutez l’URL de ce dépôt.
3. Catégorie : **Dashboard** (backend HACS : plugin).
4. Installez **Barocast HA Card**.
5. Rechargez le cache du navigateur.

## Configuration de la carte

```yaml
type: custom:barocast-ha-card
entity: sensor.barocast_forecast
detail_entity: sensor.barocast_forecast_zambretti_detail
pressure_change_entity: sensor.barocast_forecast_pressure_change
```

## Configuration optionnelle

```yaml
type: custom:barocast-ha-card
entity: sensor.barocast_forecast
detail_entity: sensor.barocast_forecast_zambretti_detail
pressure_change_entity: sensor.barocast_forecast_pressure_change
icon_now: mdi:weather-cloudy-clock
```

## Notes
- Cette carte est en lecture seule et affiche les valeurs produites par l’intégration.
- Les valeurs manquantes sont affichées par `-` tant que les capteurs ne sont pas disponibles.
