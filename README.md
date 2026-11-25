# SimClips (beta)

**Reels automáticos de tus carreras de iRacing y Le Mans Ultimate.** Corrés con OBS grabando y, al terminar,
SimClips ya tiene los mejores momentos cortados (sobrepasos, peleas, trompos, la largada, la bandera), con tu
cámara, repeticiones desde otras cámaras, widgets, portada y el texto para el posteo. Verticales para Reels,
TikTok y Shorts, y la carrera editada para YouTube.

Todo corre en tu PC: no hay cuentas ni servidores. La interfaz está en español e inglés. Acá se publican los
instaladores; el código está en un repo privado aparte.

> **Primera vez:** leé la [guía para testers (PDF)](Guia_testers_SimClips.pdf): modo de uso paso a paso, cómo
> preparar OBS, qué mirar, problemas comunes y los avisos importantes de la beta.

## Descargar

Todas las versiones, están en [Releases](../../releases).

## Qué necesitás

- **Windows 10 u 11 (64 bits).** No hay versión para Mac ni Linux.
- **iRacing y/o Le Mans Ultimate** (los únicos sims soportados). Con Le Mans Ultimate no hay que instalar ningún plugin.
- **[OBS Studio](https://obsproject.com/) 28 o más nuevo.** Con OBS 30 o más nuevo, SimClips también puede cambiar la
  carpeta de grabación; con 28 o 29 la cambiás vos en OBS (Configuración > Salida).
- **Recomendado:** placa de video NVIDIA (graba y arma los videos mucho más rápido con NVENC).
- **Espacio en disco:** una carrera de 40 minutos en 1080p60 pesa entre 8 y 15 GB. Conviene un disco con 100 GB libres
  o más (mejor si no es el de Windows).
- Opcional: micrófono (para detectar tus reacciones) y cámara web (sale arriba en los reels).

## Instalar

1. Bajá el instalador de [Releases](../../releases): `SimClips-Setup-X.Y.Z.exe`
   de la versión más nueva; las de la beta aparecen como "Pre-release").
2. Ejecutalo. No pide permisos de administrador. Te pregunta si querés un acceso directo en el escritorio y si querés
   que SimClips se abra con Windows (las dos son opcionales).
3. Si Windows muestra "Windows protegió tu PC": **Más información > Ejecutar de todas formas** (la beta todavía
   no tiene firma digital; el instalador no lleva el código fuente).
4. **Abrí OBS y después SimClips.** La bienvenida encuentra sola la conexión con OBS (y su contraseña), te deja poner tu @,
   elegir un color y las opciones, y revisa que esté todo listo. El botón "Dejar OBS listo para SimClips" ajusta OBS por vos
   (1080p60, formato mkv, pistas de audio, escena de replays).
   Si dice "OBS no responde": en OBS, **Herramientas > Configuración del servidor WebSocket > Habilitar**.

## Cómo se usa

1. Abrí **OBS y SimClips** (los dos, antes de largar) y corré como siempre: SimClips graba solo cuando larga la carrera
   y marca los momentos leyendo la telemetría. Suenan avisos cortos (empezó a grabar, cortó, reels listos).
2. **iRacing: si querés las repeticiones con otras cámaras, tenés que esperar un rato después de la bandera.** Salí del auto al
   garage **sin salir de la sesión** (tenés 5 minutos) y esperá los pitidos: SimClips maneja el replay y graba cada momento
   desde otras cámaras (de 1 a 3 minutos, sin tocar iRacing) y recién después arma los reels y te avisa. Si no querés
   esperar, el botón "Cortar los replays" arma los reels ya, con la cámara de tu auto.
   En Le Mans Ultimate no hay replays: arma los reels al terminar la carrera, sin que hagas nada.
3. En **Carreras** abrí la carrera y tocá un reel para editarlo (cortar, textos, sonidos, música, cámaras) y "Rehacer".
4. **Publicar** te abre TikTok o Instagram con el texto copiado (arrastrás el video y pegás) o te lo manda al celular con
   un QR. La subida directa todavía no está.

**Dónde queda todo:** los reels, en una carpeta `Reels` al lado de la grabación de OBS, con una subcarpeta por carrera
(fecha, hora y pista). Por defecto la grabación entera se guarda 3 días y después quedan solo los momentos (se cambia en
Ajustes > Reels). Tus ajustes y datos están en `%LOCALAPPDATA%\SimClips`.

**Coach, spotter y widgets:** el coach analiza tus vueltas (en iRacing, prendé la telemetría con Alt+L en pista) y te habla
en práctica; el spotter (iRacing) avisa combustible y cuándo parar; los widgets (Diseño > Widgets) van en los reels, en el
stream y, si iRacing está en ventana sin bordes, encima del juego (no quedan en lo que graba OBS en carrera). En
Ajustes > General > Qué usás prendés o apagás cada función; el "Modo liviano" deja solo los reels.

## Si algo no anda

| Problema | Qué hacer |
|---|---|
| No grabó la carrera | OBS tiene que estar abierto antes de largar y con el servidor WebSocket habilitado. |
| El reel quedó mudo | OBS tiene que capturar el "Audio del escritorio" sin silenciar. No se puede arreglar después. |
| No salieron las otras cámaras | No saliste al garage a tiempo, saliste de la sesión o tocaste iRacing mientras grababa. |
| Tarda mucho en armar | Normal sin placa NVIDIA, o si corriste otra carrera (se pausa mientras estás en pista). Probá el Modo liviano. |
| Se ve la pantalla entera | Tu escena de OBS captura la pantalla: cambiala a "Captura de juego". |
| Se llenó el disco | Pasá las grabaciones a otro disco (la bienvenida y Ajustes te lo proponen). |

## Avisos de la beta

- Es una beta: no borres grabaciones importantes hasta ver que los reels salieron bien.
- No está pensado para usarse mientras transmitís en vivo: el armado se pausa mientras estás en pista o en vivo.
- Solo iRacing y Le Mans Ultimate. Las repeticiones con otras cámaras, las banderas de rivales en los widgets y el spotter
  de combustible son solo de iRacing.
- La subida directa a YouTube, TikTok e Instagram todavía no está ("Próximamente").
- Las diferencias de tiempo y la ganancia de iRating son estimadas.

## Contanos qué anda y qué no

Desde la app: **Inicio > Enviar feedback**: un solo cuadro con las áreas ya escritas; completás las que quieras (o pegás todo
junto) y lo vacío no se manda. Se manda directo, con unos datos técnicos para entender el problema (sin contraseñas); si no
puede, abre el [formulario](https://docs.google.com/forms/d/e/1FAIpQLSfraF8IBol4JW6nWH5HaUnpEQeUHKiINNZQDuPwzSDG2S8N4w/viewform) con tu texto ya copiado. Además guarda en tu escritorio un paquete de diagnóstico (.zip)
con tiempos y fallas, **sin datos personales y sin mandarse solo**: si querés, pasáselo a quien te dio SimClips. Una
captura o un video corto ayuda un montón.
También podés escribirle directo a Marco (Instagram: [@marcograffi_racing](https://instagram.com/marcograffi_racing)): un
bug, una idea, una duda o un audio, todo sirve.

## Actualizaciones

SimClips revisa este repo al abrirse y cada 12 horas (solo las instalaciones hechas con el instalador de acá). Cuando hay
una versión nueva te avisa y se instala con un clic; antes de instalarla verifica que el archivo sea idéntico al publicado
acá (SHA-256).

## Privacidad y desinstalar

Todo queda en tu PC. Lo único que sale es lo que mandás vos con "Enviar feedback" y la consulta a GitHub de si hay una versión
nueva. Para desinstalar: Configuración de Windows > Aplicaciones > SimClips. Te pregunta si querés borrar también tus ajustes y
registros; tus grabaciones y reels no se borran nunca.

---

### English


All versions are in [Releases](../../releases).

SimClips automatically turns your iRacing and Le Mans Ultimate races into short videos: it records with OBS, reads the
telemetry and cuts the best moments (overtakes, battles, spins, start and finish) with your webcam, replays from other
cameras, widgets, a cover and the post text. Everything runs on your PC — no accounts, no servers. The interface is
available in Spanish and English. The tester guide ([PDF](Guia_testers_SimClips.pdf)) is in Spanish: step-by-step usage, how to
set up OBS, what to look at, common problems and the important beta warnings.

**What you need**

- Windows 10/11 (64-bit). No Mac or Linux version.
- iRacing and/or Le Mans Ultimate (the only supported sims). Le Mans Ultimate needs no plugin.
- [OBS Studio](https://obsproject.com/) 28 or newer. With OBS 30+, SimClips can also change the recording folder; with 28 or 29
  you change it yourself in OBS (Settings > Output).
- Recommended: an NVIDIA GPU (recording and building videos is much faster with NVENC).
- Disk space: a 40-minute race at 1080p60 takes 8 to 15 GB. A disk with 100 GB free or more is best (preferably not the Windows one).
- Optional: a microphone (to detect your reactions) and a webcam (shown on top of the reels).

**Install**

1. Download `SimClips-Setup-X.Y.Z.exe` from [Releases](../../releases) (beta versions are marked "Pre-release") and run it. No
   admin rights needed. It asks if you want a desktop shortcut and if SimClips should start with Windows (both optional).
2. If Windows SmartScreen warns you: **More info > Run anyway** (the beta isn't code-signed yet; the installer doesn't contain the source code).
3. **Open OBS, then SimClips.** The welcome screen finds the OBS connection (and its password) by itself, lets you set your @, pick a
   color and the options, and checks everything is ready. The "Get OBS ready for SimClips" button sets OBS up
   for you (1080p60, mkv format, audio tracks, replay scene). If it says OBS isn't responding: in OBS, **Tools > WebSocket Server
   Settings > Enable**.

**How to use it**

1. Open **OBS and SimClips** (both, before the race starts) and race as usual: SimClips records on its own when the race starts and marks
   the moments from the telemetry. Short sounds tell you it started recording, stopped, and the reels are ready.
2. **iRacing: if you want the replays from other cameras, you have to wait a while after the flag.** Leave the car to the garage **without
   leaving the session** (you have 5 minutes) and wait for the beeps: SimClips drives the replay and records each moment from other
   cameras (1 to 3 minutes, don't touch iRacing) and only then builds the reels and tells you. If you don't want to wait, the "Stop the
   replays" button builds the reels right away with your car's camera. Le Mans Ultimate has no replays: it builds the reels when the race ends, with nothing for you to do.
3. In **Races** open the race and tap a reel to edit it (cuts, texts, sounds, music, cameras) and "Redo".
4. **Publish** opens TikTok or Instagram with the text already copied (you drag the video and paste) or sends it to your phone with a QR.
   Direct upload isn't available yet.

**Where everything is:** reels go in a `Reels` folder next to the OBS recording, with a subfolder per race (date, time and track). By default the
full recording is kept for 3 days and then only the moments remain (change it in Settings > Reels). Your settings and data are in `%LOCALAPPDATA%\SimClips`.

**Coach, spotter and widgets:** the coach analyzes your laps (on iRacing, turn telemetry on with Alt+L on track) and talks to you in practice; the
spotter (iRacing) warns about fuel and when to pit; the widgets (Layout > Widgets) go in the reels, on the stream and, if iRacing is borderless windowed, on top of the game (they are
not part of what OBS records during the race). In Settings > General > "What you use" you turn each feature on or off; "Light mode" keeps only the reels.

**If something doesn't work**

| Problem | What to do |
|---|---|
| It didn't record the race | OBS must be open before the race starts, with the WebSocket server enabled. |
| The reel has no sound | OBS must capture "Desktop Audio", unmuted. It can't be fixed afterwards. |
| No other-camera shots | You didn't reach the garage in time, left the session or touched iRacing while it was recording. |
| Building takes long | Normal without an NVIDIA GPU, or if you raced again (it pauses while you're on track). Try Light mode. |
| You see the whole screen | Your OBS scene captures the screen: switch it to "Game Capture". |
| The disk is full | Move recordings to another disk (the welcome screen and Settings suggest it). |

**Beta warnings:** it's a beta, don't delete important recordings until the reels look right · not meant to be used while live-streaming (building pauses while you're on track or live) ·
iRacing and Le Mans Ultimate only; other-camera replays, rivals' flags in the widgets and the fuel spotter are iRacing only · direct upload to
YouTube, TikTok and Instagram isn't available yet · time gaps and iRating gain are estimates.

Feedback: **Home > Send feedback** in the app: a single box with the areas already written; fill in the ones you want (or paste everything together) and empty ones aren't sent. It's sent
directly, with some technical details to understand the problem (no passwords); if it can't, it opens the [form](https://docs.google.com/forms/d/e/1FAIpQLSfraF8IBol4JW6nWH5HaUnpEQeUHKiINNZQDuPwzSDG2S8N4w/viewform) with your text already copied. It also saves a diagnostic package (.zip) with timings and
failures on your desktop, **with no personal data and never sent by itself**: if you want, give it to whoever gave you SimClips. A screenshot or a short video helps a lot. You can also message Marco directly
(Instagram: [@marcograffi_racing](https://instagram.com/marcograffi_racing)): a bug, an idea, a question or a voice note, anything helps.

Updates: SimClips checks this repo when it opens and every 12 hours (installer builds only). When there is a new version it tells you and installs with one click, after checking the file matches the published
SHA-256. Privacy: everything stays on your PC; the only things that leave it are what you send with "Send feedback" and the check for new versions. To uninstall: Windows Settings > Apps > SimClips; it asks if you also want to delete
your settings and logs; your recordings and reels are never deleted.

<!-- Este repo tiene que ser público: la app consulta los releases sin iniciar sesión. -->
