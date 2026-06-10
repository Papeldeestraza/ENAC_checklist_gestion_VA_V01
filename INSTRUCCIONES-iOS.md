# Implantación del Checklist VA en iPhone / iPad

Tienes **dos vías**. La **Opción A (recomendada)** convierte el checklist en una app real: icono propio, pantalla completa y funcionamiento **sin conexión** (imprescindible en piscinas, parques o instalaciones sin cobertura). La **Opción B** es un acceso rápido sin necesidad de servidor, pero con limitaciones.

En ambos casos, **los datos se guardan automáticamente en el dispositivo** mientras no borres el historial del navegador ni pulses "Reiniciar".

---

## Archivos entregados

Todos van juntos en la carpeta `va-app-ios` (o en el ZIP `VA-ENAC-iOS.zip`):

- `index.html` — el checklist
- `manifest.json` — define la app (nombre, icono, color)
- `sw.js` — permite el uso sin conexión
- `icon-180.png`, `icon-192.png`, `icon-512.png`, `icon-512-maskable.png` — iconos

> Importante: estos archivos deben permanecer **juntos en la misma carpeta** y conservar sus nombres.

---

## OPCIÓN A — App completa con icono y sin conexión (recomendada)

Requiere publicar la carpeta en una dirección web (HTTPS). La forma gratuita más sencilla es **GitHub Pages**. Solo se hace una vez.

### Paso 1 · Crear el repositorio (desde un ordenador)
1. Entra en https://github.com y crea una cuenta (si no la tienes).
2. Pulsa **New repository**. Ponle un nombre, p. ej. `va-enac`. Márcalo como **Public**. Crea el repositorio.
3. En la página del repositorio, pulsa **Add file → Upload files**.
4. Arrastra **todos** los archivos de la carpeta `va-app-ios` (no la carpeta, sino su contenido). Pulsa **Commit changes**.

### Paso 2 · Activar GitHub Pages
1. En el repositorio, ve a **Settings → Pages**.
2. En "Source", elige la rama **main** y carpeta **/ (root)**. Pulsa **Save**.
3. Espera 1–2 minutos. Aparecerá la dirección, del tipo:
   `https://TU-USUARIO.github.io/va-enac/`

### Paso 3 · Instalar en el iPhone/iPad
1. Abre esa dirección en **Safari** (debe ser Safari, no Chrome).
2. Pulsa el botón **Compartir** (cuadrado con flecha hacia arriba).
3. Desliza y pulsa **Añadir a pantalla de inicio**.
4. Confirma el nombre ("VA ENAC") y pulsa **Añadir**.
5. Aparecerá el icono en la pantalla de inicio. Ábrelo **una vez con conexión** para que se descargue y quede disponible sin internet.

A partir de ahí funciona como una app: a pantalla completa, con icono y **sin necesidad de conexión** en campo.

---

## OPCIÓN B — Sin servidor (acceso rápido)

Más simple, pero el icono no será personalizado y conviene tener el archivo a mano.

1. Pásate el archivo `index.html` al iPhone/iPad (por **AirDrop**, correo o guardándolo en **Archivos / iCloud Drive**).
2. Abre la app **Archivos**, localiza `index.html` y tócalo. Si no se abre con todas las funciones, mantén pulsado → **Compartir → Safari**, o usa una app gratuita tipo visor HTML.
3. Una vez abierto en Safari, puedes usar **Compartir → Añadir a pantalla de inicio** para crear un acceso directo.

> Nota: por seguridad, iOS limita algunas funciones cuando un archivo se abre directamente desde Archivos. Para una experiencia completa y sin conexión, usa la Opción A.

---

## Uso diario

- **Marcar ítems**: toca cada línea. Se tacha y suma al progreso.
- **Cronómetro**: toca el reloj de la barra superior para iniciar/pausar la duración de la VA.
- **Hallazgos**: en la fase "Observación", botón **+ Añadir hallazgo** para registrar desviaciones con su referencia normativa y tipo.
- **Notas**: cada fase tiene su cuadro de observaciones.
- **Guardado**: automático. El indicador 💾 Auto recuerda que no hay que guardar a mano.
- **Exportar informe**: botón **⬇ Exportar informe** → genera el informe completo en texto → **Copiar al portapapeles** para pegarlo en correo, Notas o tu documento de informe.
- **Imprimir / PDF**: botón **🖨 Imprimir / PDF** → en el diálogo de impresión de iOS, pellizca para "Guardar en Archivos" como PDF.
- **Reiniciar**: borra todo lo introducido en el dispositivo (pide confirmación). Úsalo al empezar una VA nueva, **después** de haber exportado la anterior.

---

## Recomendación

Para trabajo de campo recurrente, la **Opción A** es claramente superior: una sola configuración inicial y después funciona como cualquier app del iPad, también en instalaciones sin cobertura. Si necesitas que el checklist sea privado (no público en GitHub), puede alojarse igualmente en cualquier hosting con HTTPS de tu organización; el procedimiento de "Añadir a pantalla de inicio" es idéntico.
