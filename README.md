# SimClips (beta)

**Reels automáticos de tus carreras de iRacing y Le Mans Ultimate.** Corrés con OBS grabando y, al terminar,
SimClips ya tiene los mejores momentos cortados (sobrepasos, peleas, trompos, la largada, la bandera), con tu
cámara, repeticiones desde otras cámaras, widgets, portada y el texto para el posteo. Verticales para Reels,
TikTok y Shorts, y la carrera editada para YouTube.

Todo corre en tu PC: no hay cuentas ni servidores. La interfaz está en español e inglés. Acá se publican los
instaladores; el código está en un repo privado aparte.

## Instalar

> **Primera vez:** leé la [guía para testers (PDF)](Guia_testers_SimClips.pdf): cómo probar, qué mirar y los avisos
> importantes de la beta.

1. Entrá a [Releases](../../releases) y bajá `SimClips-Setup-X.Y.Z.exe` de la versión más nueva
   (las de la beta aparecen como "Pre-release").
2. Ejecutalo. No pide permisos de administrador.
3. Si Windows muestra "Windows protegió tu PC": **Más información > Ejecutar de todas formas** (la beta todavía
   no tiene firma digital).
4. Abrí OBS y después SimClips: la bienvenida encuentra sola la conexión con OBS, te deja elegir un diseño y
   revisa que esté todo listo.

**Necesitás:** Windows 10 u 11 (64 bits), iRacing o Le Mans Ultimate y [OBS Studio](https://obsproject.com/) 28 o
más nuevo (con OBS 30 o más nuevo, SimClips también puede elegir la carpeta de grabación). Recomendado: placa NVIDIA (graba y arma los videos mucho más rápido).

## Cómo se usa

Abrí OBS y SimClips y corré como siempre: graba solo cuando larga la carrera. **En iRacing, si querés las
repeticiones con otras cámaras, tenés que esperar un rato después de la bandera:** salí del auto al garage **sin salir de la sesión** y
esperá los pitidos; SimClips maneja el replay y graba cada momento (de 1 a 3 minutos, sin tocar iRacing) y recién después arma los reels y te avisa. Si no querés
esperar, el botón "Cortar los replays" arma los reels ya, con la cámara de tu auto. En Le Mans Ultimate no hay replays: arma los reels al terminar.
El paso a paso completo está en la guía.

## Contanos qué anda y qué no

Desde la app: **Inicio > Enviar feedback**: un solo cuadro con las áreas ya escritas; completás las que quieras (o pegás todo junto) y lo vacío no se manda. Se manda directo, con unos datos técnicos para entender el problema (sin
contraseñas); si no puede, abre el [formulario](https://docs.google.com/forms/d/e/1FAIpQLSfraF8IBol4JW6nWH5HaUnpEQeUHKiINNZQDuPwzSDG2S8N4w/viewform) con tu texto ya copiado. Además guarda en tu escritorio un
paquete de diagnóstico (.zip) con tiempos y fallas, **sin datos personales y sin mandarse solo**: si querés, pasáselo a
quien te dio SimClips. Una captura o un video corto ayuda un montón.

## Actualizaciones

SimClips revisa este repo al abrirse y cada 12 horas (solo las instalaciones hechas con el instalador de acá). Cuando hay una versión nueva te avisa y se instala con un
clic; antes de instalarla verifica que el archivo sea idéntico al publicado acá (SHA-256).

---

### English

SimClips automatically turns your iRacing and Le Mans Ultimate races into short videos: it records with OBS, reads
the telemetry and cuts the best moments (overtakes, battles, spins, start and finish) with your webcam, replays
from other cameras, widgets, a cover and the post text. Everything runs on your PC.

The interface is available in Spanish and English. The tester guide ([PDF](Guia_testers_SimClips.pdf)) is in Spanish. Download `SimClips-Setup-X.Y.Z.exe` from
[Releases](../../releases) and run it (no admin rights needed). If Windows SmartScreen warns you: **More info > Run
anyway** (the beta isn't code-signed yet). Requires Windows 10/11 64-bit, iRacing or Le Mans Ultimate and
[OBS Studio](https://obsproject.com/) 28 or newer (with OBS 30+, SimClips can also set the recording folder).
Recommended: an NVIDIA GPU.

How to use it: open OBS and SimClips and race as usual; it records on its own. **On iRacing, if you want the replays from other cameras, you have to wait a while after the flag:** leave the car to the garage **without leaving the session** and wait for the beeps; SimClips drives the replay and records each moment (1 to 3 minutes, don't touch iRacing) and only then builds the reels and tells you. If you don't want to wait, the "Stop the replays" button builds the reels right away with your car's camera. Le Mans Ultimate has no replays: it builds the reels when the race ends.

Feedback: **Home > Send feedback** in the app: a single box with the areas already written; fill in the ones you want (or paste everything together) and empty ones aren't sent. It's sent directly, with some technical details to understand the
problem (no passwords); if it can't, it opens the [form](https://docs.google.com/forms/d/e/1FAIpQLSfraF8IBol4JW6nWH5HaUnpEQeUHKiINNZQDuPwzSDG2S8N4w/viewform) with your text already copied. It also saves a
diagnostic package (.zip) with timings and failures on your desktop, **with no personal data and never sent by
itself**: if you want, give it to whoever gave you SimClips. A screenshot or a short video helps a lot.

Updates: SimClips checks this repo when it opens and every 12 hours (installer builds only). When there is a new
version it tells you and installs with one click, after checking the file matches the published SHA-256.

<!-- Este repo tiene que ser público: la app consulta los releases sin iniciar sesión. -->
