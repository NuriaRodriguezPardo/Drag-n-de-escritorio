# 🐉 Dragón de Escritorio · Ember

Ember es un dragón adulto de fantasía que vive en tu escritorio de Windows. Camina por encima de la barra de tareas, vuela por la pantalla, se posa sobre tus ventanas, duerme, juega, escupe fuego y tiene su propio carácter. No es un GIF pegado en la pantalla: es un personaje animado con esqueleto que decide por sí mismo qué hacer.

- **Versión:** 1.0.0
- **Sistema:** Windows 10 / 11 (64 bits)
- **Tamaño:** instalador de unos 2 MB · unos 4 MB instalado
- **Conexión a Internet:** no la necesita

---

## Índice

1. [Instalación](#1-instalación)
2. [Actualizar a una versión nueva](#2-actualizar-a-una-versión-nueva)
3. [Desinstalar](#3-desinstalar)
4. [Abrir y cerrar el dragón](#4-abrir-y-cerrar-el-dragón)
5. [El menú de la bandeja](#5-el-menú-de-la-bandeja)
6. [Cómo interactuar con él](#6-cómo-interactuar-con-él)
7. [Personalidad y estados de ánimo](#7-personalidad-y-estados-de-ánimo)
8. [Repertorio de animaciones](#8-repertorio-de-animaciones)
9. [Interacción con Windows](#9-interacción-con-windows)
10. [Seguridad y privacidad](#10-seguridad-y-privacidad)
11. [Rendimiento](#11-rendimiento)
12. [Solución de problemas](#12-solución-de-problemas)
13. [Preguntas frecuentes](#13-preguntas-frecuentes)
14. [Archivos incluidos](#14-archivos-incluidos)
15. [Para desarrolladores](#15-para-desarrolladores)
16. [Limitaciones conocidas](#16-limitaciones-conocidas)

---

## 1. Instalación

### Con instalador (recomendado)

1. Haz doble clic en **`DragonEscritorio-Instalador-1.0.0.exe`**.
2. Si aparece el aviso azul de **Windows SmartScreen** ("Windows protegió su PC"), pulsa **Más información** y luego **Ejecutar de todas formas**. El aviso sale porque el programa no tiene una firma digital de pago; no significa que sea peligroso.
3. Elige qué quieres instalar:
   - **Dragón de Escritorio** (obligatorio).
   - **Acceso directo en el escritorio** (marcado por defecto).
   - **Iniciar con Windows** (desmarcado por defecto).
4. Pulsa **Instalar** y, al final, deja marcada la casilla **Despertar al dragón ahora**.

No hacen falta permisos de administrador. El programa se instala solo para tu usuario, en:

```
C:\Users\<tu usuario>\AppData\Local\Programs\DragonEscritorio\
```

### Versión portable (sin instalar)

1. Descomprime **`DragonEscritorio-Portable-1.0.0.zip`** en la carpeta que quieras.
2. Mantén juntos los archivos `DragonEscritorio.exe` y `WebView2Loader.dll`.
3. Ejecuta `DragonEscritorio.exe`.

### Requisito: WebView2

El dragón usa **Microsoft Edge WebView2 Runtime** para dibujarse.

- **Windows 11:** ya lo trae.
- **Windows 10:** lo trae si está actualizado.

Si falta, el instalador lo detecta y te ofrece abrir la página oficial de descarga de Microsoft. Instálalo y vuelve a ejecutar el instalador del dragón.

---

## 2. Actualizar a una versión nueva

**No hace falta desinstalar.** Ejecuta el instalador nuevo encima del anterior:

- Se instala en la misma carpeta y sustituye cada archivo por su versión nueva, así que no quedan restos de la versión antigua ocupando espacio.
- Si el dragón está abierto, el instalador lo cierra automáticamente.
- Tus ajustes (volumen, tamaño, frecuencia…) se conservan.
- Los accesos directos y la entrada en "Aplicaciones" se actualizan en lugar de duplicarse.

**Versión portable:** cierra el dragón desde la bandeja, descomprime el zip nuevo en la misma carpeta y acepta reemplazar los archivos.

Cuando termines, puedes borrar el archivo del instalador si no lo quieres guardar.

---

## 3. Desinstalar

Tienes dos formas:

- **Configuración › Aplicaciones › Aplicaciones instaladas › Dragón de Escritorio › Desinstalar**
- **Menú Inicio › Dragón de Escritorio › Desinstalar**

El desinstalador cierra el dragón y borra el programa, los accesos directos y el inicio automático con Windows.

Tus ajustes se guardan en un archivo pequeño (menos de 1 KB) que no se borra. Si quieres eliminarlo también, borra esta carpeta:

```
%APPDATA%\com.claude.dragonescritorio\
```

---

## 4. Abrir y cerrar el dragón

**Para abrirlo:** busca **"Dragón de Escritorio"** en el menú Inicio o usa el acceso directo del escritorio. Al arrancar, Ember entra volando desde un lado de la pantalla y aterriza.

Junto al reloj, en la bandeja del sistema, aparece un icono con su cabeza. Si no lo ves, pulsa la flecha **^** que hay al lado del reloj; puedes arrastrar el icono fuera de ese menú para que siempre esté visible.

- **Clic izquierdo en el icono:** muestra u oculta al dragón.
- **Clic derecho en el icono:** abre el menú completo de ajustes.

**Para cerrarlo**, elige cualquiera de estas opciones:

- Icono de la bandeja › **Cerrar la aplicación**.
- Clic derecho sobre el dragón › **Cerrar la aplicación**.

Si intentas abrir el programa cuando ya está en marcha, no se abre una segunda copia: el dragón que ya existe vuelve a la pantalla.

---

## 5. El menú de la bandeja

| Opción | Qué hace |
|---|---|
| **Mostrar dragón** | Lo muestra u oculta. Oculto no consume casi nada. |
| **Llamar al dragón ahora** | Si se ha ido de paseo, vuelve volando. Si ya está, viene a buscarte. |
| **Pausar animaciones** | Lo congela en su postura actual y deja de consumir recursos. |
| **Autonomía (vida propia)** | Activada: decide solo qué hacer y cuándo irse y volver. Desactivada: se queda tranquilo en su sitio y solo reacciona cuando interactúas con él. |
| **Frecuencia de aparición** | Cuánto tiempo pasa en pantalla y cuánto fuera (ver tabla de abajo). |
| **Volumen** | Silencio, 25 %, 50 %, 75 % o 100 %. |
| **Tamaño** | Pequeño, Mediano o Grande. |
| **Interacción con Windows ›** | **Posarse sobre ventanas** y **Permitir empujar ventanas reales** (ver [sección 9](#9-interacción-con-windows)). |
| **Iniciar con Windows** | Aparece automáticamente al encender el ordenador. |
| **Instrucciones** | Muestra un resumen de los controles en pantalla. |
| **Cerrar la aplicación** | Cierra el programa por completo. |

### Frecuencia de aparición (valores aproximados)

| Modo | Tiempo en pantalla | Tiempo fuera |
|---|---|---|
| **Baja** | 2–4 minutos | 15–30 minutos |
| **Normal** | 3–7 minutos | 4–10 minutos |
| **Alta** | 5–10 minutos | 1–3 minutos |
| **Siempre presente** | Siempre | Nunca se va |

Los tiempos varían a propósito para que no resulte predecible. Mientras está fuera, a veces cruza la pantalla volando sin detenerse.

---

## 6. Cómo interactuar con él

| Acción | Reacción |
|---|---|
| **Clic** | Te mira con curiosidad o da un saltito de alegría, según su humor. |
| **Varios clics seguidos** | Se va irritando… y puede acabar escupiendo fuego hacia el cursor. |
| **Doble clic** | Echa a volar por la pantalla. |
| **Arrastrar** | Lo coges en brazos: patalea y mueve las alas. Al soltarlo cae al suelo o, si estaba alto, sale volando. |
| **Pasar el ratón despacio por encima** | Lo acaricias: ronronea y se pone contento. |
| **Clic si está dormido** | Se despierta de mal humor. |
| **Clic derecho sobre él** | Menú rápido (ver abajo). |
| **Soltar un archivo encima** | Aparece un papel con el nombre del archivo y el dragón lo coge con la boca. Es solo visual: el archivo real no se toca. |

### Menú rápido (clic derecho sobre el dragón)

Volar · Dar vueltas · Perseguir el cursor · Jugar con el orbe · Escupir fuego · Dormir · Que se vaya un rato · Pausar · Ocultar · Instrucciones · Cerrar la aplicación

Cuando el cursor no está encima del dragón, los clics pasan a lo que haya debajo (tus ventanas, el escritorio, la barra de tareas) como si el dragón no existiera.

---

## 7. Personalidad y estados de ánimo

Ember tiene seis estados de ánimo, que cambian con el tiempo y según cómo lo trates:

| Estado | Señal | Qué le apetece |
|---|---|---|
| 😊 **Contento** | ♥ | Pasear, sentarse, posarse en ventanas, volar un poco. |
| 🔎 **Curioso** | ? | Mirar alrededor, acercarse al cursor, investigar ventanas. |
| 🎾 **Juguetón** | ♪ | Perseguir el cursor, jugar con el orbe, dar vueltas en el aire, correr. |
| 😴 **Perezoso** | … | Sentarse, tumbarse, echarse siestas. Lleva los ojos entornados. |
| 😠 **Enfadado** | 💢 | Rugir, escupir fuego, mover la cola nervioso. Le brillan los ojos. |
| 🥱 **Somnoliento** | z | Bostezar y dormir. |

Además de los estados de ánimo, lleva la cuenta de tres cosas:

- **Energía:** baja poco a poco mientras está activo y se recupera durmiendo. Con poca energía se vuelve somnoliento.
- **Irritación:** sube con los clics repetidos y con los despertares, y baja sola con el tiempo. Si es alta, se enfada.
- **Felicidad:** sube cuando juegas con él o lo acaricias, y le hace más juguetón.

Para que no resulte repetitivo, evita repetir lo que acaba de hacer.

---

## 8. Repertorio de animaciones

Todas las animaciones se generan en tiempo real a partir de un esqueleto de 34 huesos que deforma la ilustración original. Por eso los movimientos son fluidos y las transiciones entre unos y otros son suaves.

**Vida cotidiana:** respirar · parpadear · mirar alrededor · caminar (con las patas bien apoyadas en el suelo) · correr · sentarse · tumbarse · dormir · despertarse · estirarse · bostezar · mover la cola · sacudir las alas · plegar y desplegar las alas.

**Vuelo:** despegar · volar en horizontal y en diagonal · planear · quedarse suspendido en el aire · girar · dar vueltas · aterrizar (levanta polvo) · desaparecer volando · cruzar la pantalla.

**Interacciones:** perseguir el cursor · saltar para atraparlo · reaccionar a los clics · escupir fuego (con humo y chispas) · rugir · jugar con un orbe mágico · empujar ventanas · llevar en la boca los archivos que le sueltes · colgar de tu cursor cuando lo arrastras · mostrar enfado, curiosidad o alegría.

Los sonidos (aleteo, fuego, rugido, gruñido, ronroneo, ronquido, golpe al aterrizar) se sintetizan al momento, sin archivos de audio.

---

## 9. Interacción con Windows

### Posarse sobre ventanas (activado por defecto)

El dragón puede aterrizar sobre la barra de título de tus ventanas, sentarse allí y pasear por encima:

- Si mueves la ventana, **viaja con ella**.
- Si la cierras, la minimizas o la tapas con otra, **cae** al suelo.

Para hacer esto solo **mira** dónde están las ventanas; no las modifica.

### Empujar ventanas reales (desactivado por defecto)

Al activarlo, Windows te pide confirmación. A partir de ahí, el dragón puede volar hasta el lateral de una ventana y empujarla unos centímetros. Tiene estos límites:

- Nunca mueve ventanas maximizadas ni minimizadas.
- Nunca saca una ventana de la pantalla.
- Solo desplaza la ventana: **nunca la cierra, ni la redimensiona, ni cambia su contenido**.

Con esta opción desactivada, el dragón lo intenta, ve que la ventana no se mueve y se va a hacer otra cosa.

### Otros comportamientos automáticos

- **Pantalla completa:** si estás en un juego, un vídeo o una presentación a pantalla completa, el dragón se esconde y se detiene solo. Vuelve cuando sales.
- **Barra de tareas:** camina justo por encima de ella, sin taparla.

---

## 10. Seguridad y privacidad

- ❌ No borra, cierra, renombra ni modifica ningún archivo ni ventana.
- ❌ Los archivos que le sueltas encima nunca se abren, se mueven ni se copian: solo se muestra su nombre en un papel dibujado.
- ❌ No se conecta a Internet ni envía datos a ningún sitio.
- ❌ No necesita permisos de administrador.
- ✅ La única acción real sobre otras ventanas (empujarlas) viene desactivada y pide confirmación.
- ✅ Solo guarda un archivo de ajustes en `%APPDATA%\com.claude.dragonescritorio\ajustes.json`.
- ✅ "Iniciar con Windows" usa la clave de registro estándar de tu usuario (`HKCU\...\Run`), que el desinstalador elimina.

---

## 11. Rendimiento

| Situación | Consumo |
|---|---|
| En movimiento (volando, caminando) | Hasta 60 fps |
| Quieto (de pie, sentado) | 30 fps |
| Dormido | 15 fps |
| Fuera de la pantalla, oculto, en pausa o con un programa a pantalla completa | Animación detenida por completo |

- **Memoria:** el uso esperado en reposo está en torno a 50–150 MB, la mayor parte del componente WebView2 de Windows.
- **Almacenamiento:** unos 4 MB.

Si quieres que consuma lo mínimo:

- Usa **Pausar animaciones** u **Ocultar** cuando no quieras verlo.
- Pon la **Frecuencia** en **Baja**.
- Elige el **Tamaño Pequeño**.

---

## 12. Solución de problemas

**Windows muestra "Windows protegió su PC".**
Pulsa **Más información › Ejecutar de todas formas**. Ocurre con programas sin firma digital comercial.

**No pasa nada al abrirlo.**
- El dragón tarda un segundo en entrar volando desde un lado. Mira también si está en pausa u oculto: busca el icono junto al reloj.
- Si estaba "de paseo", usa **Llamar al dragón ahora**.
- Comprueba que WebView2 está instalado (ver [sección 1](#requisito-webview2)).

**Aparece un error sobre WebView2Loader.dll.**
En la versión portable, `WebView2Loader.dll` tiene que estar en la misma carpeta que `DragonEscritorio.exe`. Con el instalador no debería pasar; reinstala si ocurre.

**No veo el icono de la bandeja.**
Pulsa la flecha **^** junto al reloj. Para fijarlo, arrástralo a la barra de tareas.

**No puedo hacer clic en lo que hay detrás del dragón.**
Es normal mientras el cursor está encima de él. Aparta el cursor un poco, o arrastra al dragón a otro sitio.

**No suena nada.**
Revisa **Volumen** en el menú de la bandeja y el volumen de Windows. Algunos sonidos solo se activan después del primer clic sobre el dragón.

**Se ve borroso en tamaño Grande.**
La ilustración original tiene una resolución limitada. Usa **Mediano** para que se vea nítido.

**Desapareció mientras jugaba o veía un vídeo.**
Se esconde a propósito con los programas a pantalla completa. Vuelve al salir de ellos.

**Tengo varios monitores.**
De momento el dragón vive solo en el monitor principal.

---

## 13. Preguntas frecuentes

**¿Puedo cambiarle el nombre o el aspecto?**
El aspecto procede de la ficha de diseño original. Cambiarlo requiere regenerar los recursos (ver [sección 15](#15-para-desarrolladores)).

**¿Gasta batería en un portátil?**
Poco, pero algo gasta mientras se mueve. Con **Pausar** u **Ocultar** el consumo es prácticamente nulo.

**¿Puede ponerse por debajo de las ventanas?**
No. Siempre se mantiene por encima, salvo con los programas a pantalla completa, donde se esconde.

**¿Por qué a veces se va y no vuelve en un rato?**
Es parte de su autonomía. Ajusta la **Frecuencia de aparición** o elige **Siempre presente**.

**¿Puedo dejarlo quieto en un sitio?**
Sí: desactiva **Autonomía**. Se quedará tranquilo y solo reaccionará cuando interactúes con él.

---

## 14. Archivos incluidos

| Archivo | Contenido |
|---|---|
| `DragonEscritorio-Instalador-1.0.0.exe` | Instalador para Windows. |
| `DragonEscritorio-Portable-1.0.0.zip` | Versión sin instalación. |
| `LEEME.txt` | Instrucciones breves. |
| `README.md` | Este documento. |
| `codigo_fuente.zip` | Código fuente completo y guía para recompilar (`COMPILAR.txt`). |
| `recursos_graficos.zip` | El dragón definitivo, las texturas, el rig y 19 animaciones en GIF con una hoja de contacto. |
| `fase1/` | El recorte del diseño definitivo aprobado. |

---

## 15. Para desarrolladores

### Tecnología

- **[Tauri 2](https://tauri.app)** (Rust): ventana nativa transparente, sin bordes y siempre encima, con icono en la bandeja y acceso a la API de Windows para el cursor, las ventanas, el área de trabajo y la detección de pantalla completa.
- **[PixiJS 8](https://pixijs.com)** (WebGL): renderizado del dragón.
- **Motor de esqueleto propio:** cinemática directa, IK de dos huesos para apoyar las patas y *skinning* lineal de mallas en la CPU.
- **WebAudio:** síntesis de todos los sonidos.

### Estructura del código

```
app/
├─ src/
│  ├─ rig.js          Esqueleto 2D y skinning de mallas
│  ├─ anim.js         Todas las poses y animaciones procedurales
│  ├─ dragonview.js   Rig + párpados + brillo de ojos
│  ├─ game.js         Cerebro autónomo, ánimos, vuelo, física, interacción
│  ├─ fx.js           Fuego, humo, chispas, Zzz, polvo, orbe, papeles
│  ├─ sound.js        Sonidos sintetizados
│  ├─ platform.js     Puente con Windows (y simulación para navegador)
│  ├─ ui.js           Menú contextual y panel de ayuda
│  ├─ index.js        Arranque de la app
│  └─ preview.js      Vista previa con escritorio simulado
├─ src-tauri/src/lib.rs   Backend nativo: ventana, bandeja, ajustes, API Win32
├─ public/assets/         Texturas y rig generados
└─ preview/               Vista previa para el navegador
tools/
├─ build_rig.py       Genera el rig a partir de la ficha de diseño
├─ shot.py, play.py   Pruebas visuales automáticas
installer/
└─ installer.nsi      Script del instalador NSIS
```

### Recompilar en Windows

1. Instala **Node.js 20+**, **Rust** (https://rustup.rs) y, si quieres generar el instalador NSIS, **NSIS**.
2. Ejecuta:

   ```
   cd app
   npm install
   npx tauri build
   ```

3. El ejecutable queda en `src-tauri/target/release/` y el instalador en `src-tauri/target/release/bundle/`.

### Regenerar el dragón desde la ficha de diseño

Requiere Python 3 con `opencv-python` y `numpy`:

```
python tools/build_rig.py "Ficha de diseño_ Dragón de escritorio animado.png" app/public/assets
```

Después convierte `body.png` y `wing.png` a `.webp` y vuelve a compilar.

### Probar sin compilar

Sirve la carpeta `app/` con cualquier servidor web y abre `preview/index.html`:

```
python -m http.server 8123
```

---

## 16. Limitaciones conocidas

- Solo funciona en el **monitor principal**.
- El arte procede de una única ilustración, así que en tamaño **Grande** puede verse algo suave. Algunas posturas extremas (dormir o volar) deforman ligeramente la imagen original.
- El ejecutable **no está firmado digitalmente**, por lo que SmartScreen avisa la primera vez.
- Esta versión se compiló y se probó a fondo en un escritorio simulado, pero no en todos los equipos con Windows. Si algo no funciona, guarda una descripción de lo que pasa para poder corregirlo.

---

*Ember · Dragón de Escritorio 1.0.0 — un dragón con vida propia en tu escritorio.*
# Drag-n-de-escritorio
