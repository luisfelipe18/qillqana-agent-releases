# qillqana-agent

Binarios de `qillqana-agent`, el agente local que compila tus proyectos de Qillqana con la instalación de TeX de tu equipo.

Este repositorio solo publica releases. El código fuente no está aquí.

## Instalación

1. Descarga desde [la última release](https://github.com/luisfelipe18/qillqana-agent-releases/releases/latest) el binario de tu sistema: macOS (`darwin-arm64` o `darwin-amd64`), Windows (`windows-amd64.exe`) o Linux (`linux-amd64` o `linux-arm64`).
2. Comprueba la suma con el archivo `.sha256` que lo acompaña.
3. Déjalo en una carpeta de tu `PATH` con el nombre `qillqana-agent` (`qillqana-agent.exe` en Windows).
4. Necesitas TeX Live o MiKTeX con `latexmk` y al menos uno de `pdflatex`, `xelatex` o `lualatex`.

Mientras los binarios no estén firmados, en macOS quita la cuarentena con `xattr -d com.apple.quarantine qillqana-agent` y en Windows confirma el aviso de SmartScreen.

## Uso

En Qillqana, abre Ajustes, Agentes locales y pulsa Instrucciones: ahí están los comandos con la dirección de tu instancia.

```bash
qillqana-agent login --api https://<tu-qillqana>
qillqana-agent run
```
