"# Accesibilidad_Elementos_Bootstrap_Atributos_WAI_ARIA" 

Elementos Mejorados

1. Botones

Se añadieron atributos como role, aria-labelledby, y aria-expanded para describir mejor la funcionalidad y el estado del botón a los usuarios de tecnologías asistivas.

    <!-- Código mejorado con WAI-ARIA: -->
    <button role="button" aria-labelledby="ejemplo-boton-color-azul" aria-expanded="false" type="button" tabindex="0" class="btn btn-primary">Primary</button>

2. Menús Desplegables (Dropdowns)

Los menús desplegables ahora incluyen role="menu", aria-labelledby, y aria-describedby para identificar correctamente su propósito y contenido.

    <!-- Código mejorado con WAI-ARIA: -->
    <div class="dropdown" role="menu" aria-labelledby="dropdownDesplegable" aria-describedby="menuDesplegable" tabindex="-1" aria-expanded="false">
    <button role="button" class="btn btn-secondary dropdown-toggle" type="button" data-bs-toggle="dropdown" aria-expanded="false">Dropdown</button>
    </div>

3. Alertas

Se añadieron aria-live y aria-atomic para que las alertas sean detectadas correctamente por lectores de pantalla.

    <!-- Alerta mejorada con WAI-ARIA -->
<div class="alert alert-warning" role="alert" aria-live="assertive" aria-atomic="true">
  Este es un mensaje de alerta.
</div>

4. Barra de Navegación (Navbar)

Se aplicaron atributos como role="navigation" y aria-label para identificar la barra como un menú principal.

    <!-- Código mejorado con WAI-ARIA: -->
    <nav class="navbar navbar-expand-lg navbar-light bg-light" role="navigation" aria-label="Menú principal">
    <a class="navbar-brand" href="#" id="navbar-brand" aria-label="Volver al inicio">Navbar</a>
    </nav>

5. Pestañas de Navegación (Tabs)

Las pestañas ahora incluyen aria-controls, aria-selected, y tabindex para una mejor interacción con tecnologías asistivas.

    <!-- Código mejorado con WAI-ARIA: -->
    <ul class="nav nav-tabs" id="myTab" role="tablist" aria-label="Pestañas de navegación">
    <li class="nav-item" role="presentation">
        <button class="nav-link active" id="home-tab" data-bs-toggle="tab" data-bs-target="#home" type="button" role="tab" aria-controls="home" aria-selected="true" tabindex="0">Inicio</button>
    </li>
    </ul>
