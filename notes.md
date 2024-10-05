
# Notas untopic

## SQL

### Dada una pregunta:

En el mundo real, todas las consultas SQL empiezan con una pregunta empresarial. Luego tú decides cómo escribir la consulta que responda a la pregunta. Probemos esto.

**Pregunta:**

> ¿Qué `release_year` tuvo más diversidad lingüística?

Tómate tu tiempo para traducir esta pregunta a código. Nosotros te ayudaremos a empezar y luego debes probar tus consultas en la consola.

### Se considera:

```sql
SELECT release_year, COUNT(DISTINCT(language)) AS Languages
FROM films
GROUP BY release_year
ORDER BY Languages DESC;
