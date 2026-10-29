# Indexa

Skill en español para usar un agente llamado **Indexa** que prepare y tramite el alta de una web en Google y Bing.

La versión 2 añade una revisión opcional de `llms.txt`: una guía Markdown curada para herramientas que decidan leerla. No es una garantía de aparición en asistentes de IA ni cambia la indexación o el ranking de Google.

## Uso

En un agente compatible con skills, instala la carpeta `indexa-web` en su directorio de skills. En Codex, puedes invocarla así:

```text
Usa $indexa-web como agente Indexa para https://mi-sitio.com
```

El dominio del ejemplo se sustituye por el sitio que administras. La skill también permite revisar bloqueos antes de hacer solicitudes.

## El flujo

1. Verificar la propiedad en Google Search Console.
2. Validar y enviar el sitemap del sitio.
3. Cuando aporte valor y esté autorizado, revisar o preparar un `llms.txt` de contenido público; no es un reemplazo de los pasos de indexación.
4. Inspeccionar las páginas públicas importantes y solicitar indexación.
5. Importar el sitio y su sitemap en Bing Webmaster Tools, o utilizar verificación manual.

Necesita acceso autorizado al sitio y a las cuentas correspondientes. Si una herramienta o permiso falta, informa del bloqueo y prepara los pasos independientes. No incluye contraseñas, claves API ni automatismos de inicio de sesión.

Distingue una solicitud enviada de una página indexada. Conserva privados los portales y las páginas protegidas; no elimina restricciones de una demostración por su cuenta. `llms.txt` sólo puede incluir una selección curada de URLs públicas verificadas y nunca debe copiar automáticamente el sitemap ni listar áreas privadas. La vinculación de Bing con Search Console se revisa antes de conceder acceso persistente.

## Archivos

- `SKILL.md`: instrucciones del agente.
- `agents/openai.yaml`: nombre visible y ejemplo de invocación.
- `references/seo-workflow.md`: documentación oficial y formato de evidencia.

Puedes descargar el paquete de tres archivos desde la sección [Releases](https://github.com/baudelioandalon/indexa-web/releases). La skill es un flujo de trabajo para un agente; no es un programa independiente ni garantiza indexación o posiciones en buscadores.

## Procedencia

Adaptación del flujo de cuatro pasos del [reel de Luis Álvarez Web](https://www.facebook.com/reel/2098623907436804), contrastada con la documentación oficial de Google y Bing enlazada en las referencias. No está afiliada a Google, Bing ni al autor del reel.
