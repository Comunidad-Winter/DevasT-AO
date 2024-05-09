# DesvasT-AO

## Implementaciones

### Programación

- Nicks Siempre Visibles
- MiniMapa
- Nicks De Gms Verde
- Letra Se Cambió a "Comic Sanz MS"
- Link De La Página Del AO En El FrmConnect
- IP Y Puerto Ocultos En El Cliente
- Estado Del Servidor En El FrmConnect
- Cliente Propio

### Graficación

- Se Graficaron Más De 30 Objetos Totalmente Propios
- Se Graficaron Nuevas Interfaces
- Se Graficaron Árboles Nuevos
- Se Graficaron Estatuas Propias
- Se Graficaron Nuevas Paredes
- Se Graficaron Puertas Dobles Propias
- Se Graficaron En Total Más De 100 Graficos

### Mapeo

- Edicion de algunos mapas
- Se Mapearon Aproximadamente 25 Mapas Para Eventos
- Sala De Teleport's

### Dateo

- Se Datearon 120 Objetos Aproximadamente

### Indexación

- Se Indexarón Nuevas Armaduras, Cascos, Escudos y Armas.

## Instrucciones

**Para los que no saben configurar la ip:**

Entran al VB 6.0 (puede ser el portable tambien pero el portable que compile, si no compila, NO sirve) bueno, como iva diciendo, Entran Al VB 6.0 Habren La Carpeta Contenedora Del AO, Van A La Carpeta Del Cliente Abren El "Client.vbp" (Client.Visual Basic Proyect) y Se Le Van A Habrir Todos Los Archivos de .FRM Del Codigo. Van A "FrmConnect.frm" Le Hacen Doble Click Y Se Les Va A Habrir Una Pantalla Que Es Como Si Estuviesen Por Loguear Al AO Vean Bien Y Hacen Click Donde Iria La IP (Que Creo Que En Todos Esta Configurada Como "localhost"), Bueno Una Vez Que Clickiaron Ahí, Vean Abajo A La Izq. Que Dice "IPTxt.txt", Van Mas Abajo Hasta Que Va A Decir "Text= localhost", Eso Que Dice localhost Lo Borran Y Lo Reemplazan Por Su IP. Exactamente Lo Mismo Es Para Cambiar El Puerto (Igual Les Recomiendo Que Dejen De Puerto "7666"). Esa IP Y Puerto Que Configuraron Desde Donde Les Dije, También Ponganlo En El Server.ini (Ubicado En La Carpeta Del Servidor).

Despues De Eso Hacen Click Derecho En FrmConnect Y Ponen "Ver Codigo", Apretan Control+F Y Se Les Va A Abrir Un Buscador Ponen "Proyecto Actual" Y Buscan:

```
     'Server IP
    PortTxt.Text = "7666"
    IPTxt.Text = "devastao.no-ip.info"
    IPTxt.Visible = True
    'Label5.Visible = True
```

Y Lo Cambian Por Su IP Y Puerto

Despues buscan:

```
Public Function CurServerIp() As String
 
        CurServerIp = "devastao.no-ip.info" '<---- Acá ponen la IP
 
End Function
```

Despues De Configurar Su IP A Travez De Visual Basic, Generen El .exe.
Luego, Van A La Carpeta Del Cliente, Buscan La Carpeta "Init", Van A Sinfo.dat Y Les Va A Aparecer Esto

```
[INIT]
Cant =1

[S1]
Desc=DevasT AO - Online <-- Cambian Por El Nombre De Su AO.
IP=devastao.no-ip.info <-- Cambian Por Su IP.
P2= 7667 <-- Cambian Por Su Puerto (Pero Recomiendo Que Esto Lo Dejen Así)
PJ= 7666 <-- Cambian Por Su Puerto (Pero Recomiendo Que Esto Lo Dejen Así)
```

## Fuente

https://www.gs-zone.org/temas/liberacion-devast-ao-v1-0-0.28491/
