# Prueba Práctica — Unidad IV — Ingeniería de Requisitos (ISR-401)
Sistema de Gestión de Pedidos — Modelado, Especificación, Priorización y Validación de Requisitos.

**Estudiante:** Francisco Javier Arboleda Yanza
**Asignatura:** Ingeniería de Requisitos (ISR-401)
**Docente:** Ing. Gleiston Guerrero Ulloa, Mg.
**Universidad:** Universidad Técnica Estatal de Quevedo — Facultad de Ciencias de la Computación — Ingeniería de Software, Cuarto Semestre

## Estructura del repositorio

```
.
├── main.tex                    # Archivo principal LaTeX (P1-P7)
├── main.pdf                    # PDF compilado (versión final)
├── Imagen de evidencia 1.jpeg
├── Imagen de evidencia 2.jpeg
├── Imagen de evidencia 3.jpeg
├── Imagen de evidencia 4.jpeg
├── Imagen de evidencia 5.jpeg
├── Imagen de evidencia 6.png
└── README.md                   # Este archivo
```

## Instrucciones de compilación

**Compilador:** `pdflatex` (TeX Live / MiKTeX)

**Dependencias (paquetes LaTeX):** `inputenc`, `fontenc`, `babel`, `mathptmx`, `geometry`, `tikz` (con librerías `arrows.meta`, `positioning`, `shapes.multipart`, `shapes.geometric`, `calc`), `booktabs`, `longtable`, `array`, `enumitem`, `titlesec`, `hyperref`. Todos incluidos en una distribución estándar de TeX Live 2023+ o MiKTeX; no requieren instalación adicional.

**Archivo principal:** `main.tex`

**Orden de comandos** (se ejecuta dos veces para resolver referencias cruzadas y numeración):

```bash
pdflatex -interaction=nonstopmode main.tex
pdflatex -interaction=nonstopmode main.tex
```

Esto genera `main.pdf` en el mismo directorio.

### Compilar en Overleaf

1. Subir el contenido de este repositorio (o `main.tex`) como proyecto nuevo.
2. Overleaf detecta `main.tex` automáticamente como archivo raíz.
3. Compilar con el motor **pdfLaTeX** (configuración por defecto).

### Verificar reproducibilidad localmente

```bash
git clone <URL-del-repositorio>
cd <carpeta-del-repositorio>
pdflatex -interaction=nonstopmode main.tex
pdflatex -interaction=nonstopmode main.tex
```

Si `main.pdf` se genera sin errores, la compilación es reproducible.

## Contenido del documento

| Sección | Contenido |
|---|---|
| P1 | Diagrama de clases UML — Cliente, Pedido, LíneaPedido, Producto (TikZ) |
| P2 | Diagrama de actividades UML — "Registrador pedido" (TikZ) |
| P3 | Máquina de estados UML del ciclo de vida de Pedido (TikZ) |
| P4 | Tabla de consistencia entre P1–P3 e inconsistencia detectada y corregida |
| P5 | Especificación de 4 requisitos (2 funcionales, 2 no funcionales alineados a ISO/IEC 25010:2023) |
| P6 | Priorización MoSCoW |
| P7 | Validación por inspección (ISO/IEC/IEEE 29148): detección de defectos y retrabajo |
