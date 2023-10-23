# ParcialDomiciliario Parte 1


## 🧑‍🎓Estudiante
- Joaquín N. Vicente

## Proyecto: Contador de 0 a 99
![parcial_domiciliario_1](https://github.com/JoacoVic/ParcialDomiciliario1/assets/133211768/0439fcaa-f1b0-4a4a-bfa5-1a292e0bb46b)


## Descripción
El proyecto sirve como un contador de 0 a 99 en donde se pueden subir o bajar los valores en unidades. Utiliza 2 displays de 7 segmentos y la técnica de multiplexación.

# Función principal
Esta función se encarga de reconocer el botón que se presionó para cambiar el contador.

```C
int presionarBoton(void)
{
 botonSubir = digitalRead(SUBIR);
 botonBajar = digitalRead(BAJAR);
 botonResetear = digitalRead(RESETEAR);
 if (botonSubir)
   botonSubirPrevio = 1;
 if(botonBajar)
   botonBajarPrevio = 1;
 if(botonResetear)
   botonResetearPrevio = 1;
 
 if (botonSubir == 0 && botonSubir != botonSubirPrevio)
  {
   botonSubirPrevio = botonSubir;
   return SUBIR;
  }
 if (botonBajar == 0 && botonBajar != botonBajarPrevio)
  {
   botonBajarPrevio = botonBajar;
   return BAJAR;
  }
 if (botonResetear == 0 && botonResetear != botonResetearPrevio)
  {
   botonResetearPrevio = botonResetear;
   return RESETEAR;
  }
 return 0;
}
```

## 🤖 Link al proyecto
- [proyecto](https://www.tinkercad.com/things/6vzLoPOFNS7-parcial-domiciliario-spd-joaquin-vicente/editel?sharecode=amWLb_-UNT1qJ1Hg_kgoauOPl_ppTlKQK9IMiE71BLw)

 # ParcialDomiciliario Parte 2


## 🧑‍🎓Estudiantes
- Joaquín N. Vicente
- Alejandro Voutsina Labrin
- Giuliano Sohrobigarat
- Franco Postulka

## Proyecto: Contador de 0 a 99, contador de primos, motor de CC y sensor de temperatura
![parcial_domiciliario_2](https://github.com/JoacoVic/ParcialSPD/assets/133211768/d620e3de-f196-413b-9ff5-3818b6bbd493)



## Descripción
Utiliza un contador de 0 a 99, y con un switch cambia a un contador de números primos con los mismos valores. Además, contiene un sensor de temperatura conectado a un motor de CC.

Motor de  CC: Es un dispositivo de salida analógica con valores del 0 al 255. En el proyecto funciona como un ventilador que recibe los valores en grados del sensor de temperatura, y trabaja a las RPM acordes a los grados.

Sensor de temperatura: es un dispositivo de entrada y salida analógica.

# Función principal
Esta función se encarga de reconocer el botón que se presionó para cambiar el contador.

```C
int presionarBoton(void)
{
 botonSubir = digitalRead(SUBIR);
 botonBajar = digitalRead(BAJAR);
 botonResetear = digitalRead(RESETEAR);
 if (botonSubir)
   botonSubirPrevio = 1;
 if(botonBajar)
   botonBajarPrevio = 1;
 if(botonResetear)
   botonResetearPrevio = 1;
 
 if (botonSubir == 0 && botonSubir != botonSubirPrevio)
  {
   botonSubirPrevio = botonSubir;
   return SUBIR;
  }
 if (botonBajar == 0 && botonBajar != botonBajarPrevio)
  {
   botonBajarPrevio = botonBajar;
   return BAJAR;
  }
 if (botonResetear == 0 && botonResetear != botonResetearPrevio)
  {
   botonResetearPrevio = botonResetear;
   return RESETEAR;
  }
 return 0;
}
```

## 🤖 Link al proyecto
- [proyecto](https://www.tinkercad.com/things/6vzLoPOFNS7-parcial-domiciliario-spd-joaquin-vicente/editel?sharecode=amWLb_-UNT1qJ1Hg_kgoauOPl_ppTlKQK9IMiE71BLw)


