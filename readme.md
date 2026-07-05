# Dark Imports — Identidad Sonora y Avatar Conversacional

## Proyecto
Dark Imports — Tienda de tecnología importada — Córdoba, Argentina

## Herramientas utilizadas
- ElevenLabs (voz)
- Suno v4.5 (música)
- Google Flow (personaje e imagen)
- HeyGen AI Studio (avatar conversacional)

---

## Activos generados

| Archivo | Descripción | Herramienta |
|---|---|---|
| `assets/voz_marca.mp3` | Voz en off del guion de marca | ElevenLabs |
| `assets/musica_marca.mp3` | Música instrumental de marca | Suno v4.5 |
| `assets/personaje.jpg` | Imagen del personaje consistente | Google Flow |
| `output/video_avatar.mp4` | Video final del avatar conversacional | HeyGen |

---

## Guion narrado (45 segundos)

"Hay productos que llevan meses en tu cabeza. Los mirás, los investigás, los comparás. Pero algo siempre frena el momento. En Dark Imports ese momento llega. Traemos tecnología original directo del exterior. MacBooks, iPhones, PS5, AirPods y más. El proceso es simple: lo encontrás, nos escribís, elegís cómo pagar, y llega a tus manos. Sin letra chica. Sin sorpresas. Solo el producto que siempre quisiste. ¿Cuál es el tuyo?"

---

## Prompts utilizados

### Voz — ElevenLabs
- Herramienta: ElevenCreative
- Voz: Verónica — Warm, Soft and Inviting
- Modelo: Eleven Multilingual v2
- Configuración: velocidad normal, estabilidad media, similitud alta

### Música — Suno v4.5
- Nombre: Neon Pulse
- Prompt de estilos: `minimal electronic, ambient, modern, clean, tech, subtle bass, no vocals, no singing, instrumental, 95 bpm, professional, sleek`
- Prompt de letra: `[instrumental] [no vocals]`

### Personaje — Google Flow
- Modelo: Imagen 3
- Prompt: `Photo sheet with 6 portrait headshots of the same young woman, 20-25 years old, tan skin, brown eyes, long wavy brown hair, white fitted t-shirt, arranged in 2 rows of 3 on white background, pose 1: facing camera smiling, pose 2: facing camera serious, pose 3: left side profile, pose 4: right side profile, pose 5: left three quarter back, pose 6: right three quarter back, studio lighting, white background, photorealistic, 8K, same identical face in every pose`

---

## Workflow técnico en HeyGen

1. Se subió `personaje.jpg` como **Photo Avatar** en HeyGen
2. Se seleccionó **Motor de movimiento Avatar IV** que controla los visemas (movimientos labiales) sincronizados fonema por fonema con el audio
3. Se cargó `voz_marca.mp3` de ElevenLabs como **audio externo** para controlar el tono emocional
4. Se insertaron **pausas entre oraciones** en el guion para permitir movimientos gestuales naturales del avatar
5. Se integró `musica_marca.mp3` como **pista de fondo al 15-20% de volumen** para no eclipsar la voz
6. Se configuró **fondo negro puro** coherente con el Manual de Identidad Visual del Módulo 3
7. Se validó la **sincronización labial cuadro a cuadro** antes de exportar

---

## Coherencia con el Manual de Identidad Visual

**Voz:** femenina, cálida y acogedora — alineada con la tonalidad del Briefing Estratégico: cercana, confiable y aspiracional sin distancia.

**Música:** instrumental minimalista y electrónica — refleja la estética oscura y premium del Manual de Identidad Visual. Tempo moderado que acompaña sin competir con la voz.

**Avatar:** mujer joven 20-25 años, tez trigueña, cabello castaño largo ondulado, remera blanca, fondo negro — consistente con el personaje diseñado en el Módulo 3.

Los tres assets funcionan como sistema unificado: la voz narra la promesa de marca, la música instala el ambiente y el avatar da cara humana a Dark Imports.

---

## Estructura del repositorio

```
/assets
  voz_marca.mp3
  musica_marca.mp3
  personaje.jpg
/output
  video_avatar.mp4
README.md
documento_coherencia.pdf
```
