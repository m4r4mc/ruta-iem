# Ruta de transición de Ingeniería en Mantenimiento Industrial a Ingeniería Electromecánica

Herramienta web para estudiantes activos de Ingeniería en Mantenimiento Industrial (ITCR/TEC) que quieren trasladarse a Ingeniería Electromecánica a partir del I-2027.

> **Aviso:** no es una herramienta oficial. Se basa en documentos públicos y en supuestos propios (ver [`docs/supuestos.md`](docs/supuestos.md)). Confirme siempre con la Escuela y con el Departamento de Admisión y Registro antes de matricular.

## Qué hace

- Muestra la malla de Mantenimiento Industrial para marcar los cursos aprobados.
- Calcula el avance en Electromecánica: qué cursos se reconocen por equivalencia y cuántos créditos lleva.
- Genera una ruta por semestre que tiene en cuenta:
  - cuándo abre cada curso de Electromecánica,
  - hasta cuándo se ofrece cada curso de Mantenimiento,
  - los requisitos y correquisitos de cada curso.
- Permite escoger el semestre desde el que se planea, fijar un máximo de créditos (general o por semestre), quitar cursos de un semestre y agregarlos desde una lista de opcionales.
- Funciona para solo bachillerato (135 créditos) o licenciatura (180) con los énfasis de Instalaciones, Aeronáutica o Sistemas ciberfísicos.
- Genera un informe en PDF (opcional).

## Cómo usarla

Abra [`index.html`](index.html) en el navegador, o use la versión publicada en GitHub Pages (ver abajo). Las instrucciones paso a paso están en [`docs/como-usar.md`](docs/como-usar.md).

Sus marcas se guardan solo en su navegador (`localStorage`). La página no envía datos a ningún servidor.

## Publicarla con GitHub Pages

1. En el repositorio: **Settings → Pages**.
2. En *Source* elija **Deploy from a branch**, rama `main`, carpeta `/ (root)`.
3. Guarde. En un par de minutos queda en `https://<usuario>.github.io/<nombre-del-repositorio>/`.

## Estructura del repositorio

```
.
├── index.html            Aplicación completa (HTML, CSS y JavaScript en un solo archivo)
├── README.md             Este archivo
├── LICENSE               Licencia
├── .gitignore
├── docs/
│   ├── como-usar.md          Guía de uso para estudiantes
│   ├── supuestos.md          Supuestos y limitaciones del cálculo
│   ├── actualizar-datos.md   Cómo modificar mallas, equivalencias y fechas de apertura
│   ├── fuentes.md            Documentos de donde salen los datos
│   └── CHANGELOG.md          Historial de cambios
└── versiones/            Versiones anteriores de la herramienta
```

## Actualizar los datos

Si la Escuela cambia el plan de transición, las mallas o las equivalencias, hay que editar las constantes de datos al inicio del `<script>` de `index.html`. La guía está en [`docs/actualizar-datos.md`](docs/actualizar-datos.md).

## Limitaciones conocidas

- Asume que los cursos de Electromecánica se ofrecen cada semestre después de su primera apertura. La guía solo indica la primera vez.
- No incluye las electivas de Mantenimiento (por ejemplo MI6253 y MI6255), cuyos requisitos no aparecen en la malla publicada.
- Los datos de énfasis y electivas deben verificarse contra el documento de la propuesta de la carrera.
- No considera cupos, horarios ni disponibilidad real de grupos.

## Fuentes

Ver [`docs/fuentes.md`](docs/fuentes.md).

## Contribuir

Los errores en mallas, requisitos o fechas se pueden reportar como *issues*. Si propone una corrección, indique el documento y la página de donde sale.

## Privacidad

No suba al repositorio notas, capturas de matrícula ni documentos con datos de estudiantes.

## Licencia

MIT. Ver [`LICENSE`](LICENSE).
