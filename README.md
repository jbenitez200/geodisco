# Geodisco

**Sal sabiendo dónde.**

Geodisco es una app con un mapa de calor de las discotecas de Sevilla. Cuanto más caliente es el color, más gente hay. Además muestra qué DJ pincha esa noche y cómo está el ambiente (música y cola).

Proyecto de emprendimiento de 2.º SMR B · Unidad 2.

## Equipo

| Persona | Roles |
|---|---|
| Juanma Benitez | CEO y Diseño |
| Javier Bermejo Trabazo | CFO y CTO |

## La idea

- **Afluencia:** cuánta gente hay ahora en cada discoteca, con check-in anónimo de usuarios que dan permiso.
- **DJ de la noche:** lo publica el propio local desde su panel.
- **Ambiente:** música y cola, según lo que cuentan los usuarios.

**Mayor rival:** Google Maps, que ya muestra la afluencia, pero no el DJ ni el ambiente, y no está pensado para la noche.

## Diseño

- **Logo:** las letras G y D unidas dentro de un óvalo con degradado rosa-ámbar.
- **Colores:** primario `#14152B` (azul noche mate), secundario `#4B3F72` (violeta mate), acentos `#FF3D81` (rosa neón) y `#FFB020` (ámbar).
- **Tipografía:** Monoton (logotipo), Oswald (títulos) y DM Sans (texto).

## Modelo de negocio (CFO)

- **Ingresos:** suscripción de locales (30 €/mes, supuesto por validar); más adelante, anuncios y comisiones por entradas. Gratis para el público.
- **Costes:** unos 40 € iniciales (dominio y Google Play) y unos 35 €/mes (servidor y publicidad).
- **Punto de equilibrio:** 2 locales de pago.

## Tecnología (CTO)

| Necesidad | Elección |
|---|---|
| Lenguaje | JavaScript: app web instalable (PWA) y servidor Node.js |
| Mapa | Mapbox GL JS con capa de mapa de calor |
| Base de datos | PostgreSQL con PostGIS |
| IA | Predicción de afluencia con el historial |
| Despliegue | AWS |
| Dominio y HTTPS | No-IP y Let's Encrypt |

## Organización

Las tareas están en el Project Kanban del repositorio, con cuatro columnas: **To do**, **Doing**, **Done** y **Approved**. Las tareas no se borran: avanzan de columna.
