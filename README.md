# Ruta de transición de Ingeniería en Mantenimiento Industrial a Ingeniería Electromecánica

Herramienta web para estudiantes activos de Ingeniería en Mantenimiento Industrial (ITCR/TEC) que quieren trasladarse a Ingeniería Electromecánica a partir del I-2027.

> **Aviso:** no es una herramienta oficial. Se basa en documentos públicos y en supuestos propios. Confirme siempre con la Escuela y con el Departamento de Admisión y Registro antes de matricular.

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

Abra [`index.html`](index.html) en el navegador (funciona con doble clic, sin servidor), o use la versión publicada: <https://m4r4mc.github.io/ruta-iem/>. 

Sus marcas se guardan solo en su navegador (`localStorage`). La página no envía datos a ningún servidor.





## Limitaciones conocidas

- Asume que los cursos de Electromecánica se ofrecen cada semestre después de su primera apertura (no asume que existan cursos cuya oferta sea anual).
- No incluye las electivas de Mantenimiento (por ejemplo MI6253 y MI6255), cuyos requisitos no aparecen en la malla publicada.
- Los datos de énfasis y electivas deben verificarse contra el documento de la propuesta de la carrera.
- No considera cupos, horarios ni disponibilidad real de grupos.



