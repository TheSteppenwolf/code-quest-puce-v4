# CODE QUEST V4 · Ingeniería en Sistemas PUCE

Versión 4.0.2. Aplicación educativa para la casa abierta, publicada de forma independiente de V3.

- [Abrir e instalar la aplicación](https://thesteppenwolf.github.io/code-quest-puce-v4/)
- [Revisar la vista para celular](https://thesteppenwolf.github.io/code-quest-puce-v4/ver-celular.html)

## Mejoras de interacción

- Texto principal de 18 px con la configuración habitual del navegador, con opciones Cómodo, Grande y Muy grande.
- Cuatro accesos permanentes: Inicio, Retos, Entrena IA y Tú vs la IA.
- Bloques con explicación visible y ayuda contextual para la pantalla actual.
- Deshacer y Rehacer, revisión por pasos y acceso directo entre tablero y editor.
- Estados de actividad, resultados y progreso de entrenamiento con etiquetas claras.
- Música opcional y juego preparado para posteriores usos sin conexión.

El motor de retos y aprendizaje se mantiene. La instalación, el progreso y las cachés de V4 usan su propia identidad. V3 conserva su dirección y sus archivos.

## Instalación

Android: abrir el enlace en Chrome y elegir Instalar aplicación o Agregar a la pantalla principal. iPhone: abrir en Safari y usar Compartir → Agregar a Inicio. El QR debe apuntar al enlace de la aplicación.

## Publicación

Este repositorio contiene el paquete de recursos web públicos `CODE_QUEST_v4_Publicar.zip.b64`. El respaldo completo de desarrollo, pruebas y documentación de trabajo se conserva aparte.

GitHub Actions reconstruye el paquete público, comprueba su integridad y publica su contenido en Pages. El flujo tiene acceso de lectura al contenido del repositorio.

Para recuperar el paquete con Python 3:

```sh
python -c "import base64,pathlib; pathlib.Path('CODE_QUEST_v4_Publicar.zip').write_bytes(base64.b64decode(pathlib.Path('CODE_QUEST_v4_Publicar.zip.b64').read_bytes()))"
```

SHA-256 del paquete: `3190c79d6eb269757be45b2067cc06fd0e30f8a03b9046d2efc5965103f57264`.

## Verificación

22 pruebas automáticas superadas en el proyecto de desarrollo. En el sitio publicado se revisaron las cuatro secciones en vistas de 320 y 390 px y texto ampliado al 200 %, sin desbordamiento horizontal. Se comprobaron navegación, edición, recuperación de bloques y preferencia de lectura guardada.

La captura del editor publicado se conserva como `docs/CODE_QUEST_v4_editor.jpg.b64`.

## Referencias

- [Heurísticas de Nielsen](https://www.nngroup.com/articles/ten-usability-heuristics/)
- [W3C: ampliación de texto](https://www.w3.org/WAI/WCAG22/Understanding/resize-text.html)

El sitio permanece disponible mientras este repositorio y GitHub Pages sigan activos.
