# **EtaWatch**

![Docker Image EtaWatch](https://github.com/VK/EtaWatch/workflows/Docker%20Image%20EtaWatch/badge.svg?branch=master)

A docker setup to track all measured values ​​of an [eta pellet heating unit](https://www.eta.co.at/) with an influx database.

```
docker build -t vikru/etawatch .
```

## Some Values

    Temperaturen
    -------------------------------------------------------------------
    * Sys>>System>>Außentemperatur
    * Solar>>Zustand>>Kollektor
    * Kessel>>Kessel>>Kessel
    * Puffer>>Puffer>>PufferUntenSolar
    * Puffer>>Puffer>>PufferUnten
    * Puffer>>Puffer>>PufferOben
    * Puffer>>Warmwasserspeicher>>Warmwasserspeicher

    Pumpen
    -------------------------------------------------------------------
    * Solar>>Zustand>>Kollektorpumpe
    * Kessel>>Kessel>>Vorlauf>>Kesselpumpe
    * Hk>>Heizkreis>>Heizkreispumpe


    Lager
    -------------------------------------------------------------------
    * Lager>>Vorrat
    * Kessel>>Kessel>>Pelletsbehälter>>InhaltPelletsbehälter


    Verbrauch
    -------------------------------------------------------------------
    * Kessel>>Kessel>>Entaschung>>VerbrauchSeitAscheboxLeeren
    * Kessel>>Kessel>>Entaschung>>VerbrauchSeitWartung
