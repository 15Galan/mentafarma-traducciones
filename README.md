# Notas

## Repositorio

El archivo de configuración de Poedit (`es.mo`) es binario, por lo que puede causar conflicto en las fusiones, ya que no acepta modificaciones parciales de su contenido.

Este archivo define, por ejemplo, qué cadenas del `es.po` están marcadas como "Necesita trabajo" (en naranja) y avisos de cadenas mal formadas.

Para evitar problemas, propongo **no incluir el fichero `es.mo` en la rama _master_ y que cada usuario arrastre el suyo en su propia rama hasta el final**.

* Esto evitará conflictos de fusión combinando cambios únicamente en el fichero `es.po`, que sigue siendo texto plano.

* Además, se evitan las modificaciones de configuración entre usuarios, que quedarían sobreescritas, no combinadas.

* Una vez se alcance el 100 % de traducción, bastaría con resolver las definiciones del `es.mo` usuario a usuario, siendo estas definiciones prácticamente iguales entre ellos.


## Traducciones

* Las cadenas con HTML del módulo WebForms producen errores de "HTML mal formado" al importarse el fichero `es.po`, ya que solo permite su traducción desde su pestaña de traducciones. **Por tanto, dichas cadenas se traducirán a parte y al final, desde el módulo**.
