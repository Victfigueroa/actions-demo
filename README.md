# Proyecto Node.js con GitHub Actions – CI Automatizado

**Grupo 5:**
- Juan Villaman  
- Cristóbal de Jesus  
- Victor Figueroa

## Descripción del Proyecto

Este proyecto implementa un entorno de integración continua (CI) usando GitHub Actions en una aplicación básica de Node.js. Se automatizan las pruebas con Jest para garantizar que el código se mantenga funcional tras cada cambio o push al repositorio.

---

## Ventajas observadas al automatizar pruebas con GitHub Actions

- Detecta errores de inmediato con cada cambio.
- Ahorra tiempo, garantiza calidad continua y mejora la colaboración del equipo en tiempo real.

---

## Diferencias frente a Jenkins u otras herramientas CI

- No requiere instalación local.
- Se integra nativamente con GitHub.
- Usa YAML, lo que lo hace más simple para proyectos pequeños o personales.

---

## Mejoras futuras al pipeline

- Integración de análisis estático de código (por ejemplo, ESLint o SonarCloud).
- Pruebas en múltiples versiones de Node.js.
- Despliegue automático a producción tras una validación exitosa.

---

## Consideraciones de seguridad aplicables a proyectos reales

- Nunca exponer secretos en texto plano.
- Utilizar GitHub Secrets para credenciales sensibles.
- Limitar permisos del workflow.
- Validar entradas externas antes de ejecutar acciones automatizadas.

---

## Automatización en otros aspectos del proyecto

1. **Despliegue Continuo Automatizado:**
Implementaremos un proceso de despliegue continuo (CD) configurando un "job" o tarea automatizada en nuestra pipeline de integración continua (CI/CD). Este job se encargará de desplegar automáticamente la aplicación en plataformas como Vercel o Heroku una vez que todas las pruebas automatizadas (unitarias, de integración, etc.) hayan sido superadas exitosamente. Esto asegura que solo las versiones estables y validadas del código lleguen a producción, reduciendo errores manuales y acelerando el ciclo de lanzamiento.
2. **Auditoría de dependencias:** Usar `npm audit` o integrar Dependabot para detectar y corregir vulnerabilidades.
3. **Build automático:** Ejecutar tareas de construcción al hacer push en ramas específicas, generando versiones listas para producción.

---

## Cómo ejecutar localmente

```bash
npm install
npm test
