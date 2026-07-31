---
title: "Review CPTS de Hack The Box: mi experiencia y consejos"
date: 2026-07-30 22:34:00 -0400
categories: [Certificaciones, Hack The Box]
tags: [cpts, pentesting, hackthebox, active-directory]
image:
  path: /assets/review_ctps.png
---

## Introduccion

Hola!!, como estas? mi nombre es kylo, hace un par de semanas aprobé la CPTS de HTB, es por lo que decidí redactar esta review contando un poco mi experiencia durante la certificación. 

Bueno si más preámbulo a lo que vinimos, si llegaste a esta review puede ser por una de dos razones, 1) Decidiste realizar esta certificación y quieres conocer cómo es el examen para prepararte de mejor manera, 2) Ya estas dentro del examen, estas atrapado en una parte y buscas alguna pista que te ayude a avanzar.  

Independientemente de la etapa en la que te encuentres, **no te vayas**. Comenzaré siendo claro: aquí no encontrarás pistas ni respuestas del examen, pero sí información que podría ayudarte a prepararte correctamente o ver un camino que de primeras te saltaste. Dicho esto, empecemos desde el principio.

## 1. ¿Qué es la certificación CPTS y qué importancia tiene en el ámbito de la ciberseguridad?

La certificación **Certified Penetration Testing Specialist (CPTS)** de HackTheBox se convierte cada día en el estándar en el campo de la seguridad ofensiva. Una característica que destaca esta certificación por encima del resto, es que no es un CTF (Capture The Flag) tradicional, es una evaluación práctica que simula una organización real donde está pensada para poner a prueba todas tus capacidades de razonamiento y exprime al máximo tu metodología a la hora de encadenar ataques.

Así que la CPTS no es solo un examen, es **tu** demostración real de que sabes cómo llevar a cabo un **Pentesting Engagement** de principio a fin, aplicando una metodología profesional y que cuentas con las habilidades comunicativas necesarias para transformar tus resultados técnicos en un informe ejecutivo claro, comprensible y orientado al negocio.

### El Precio

Una de las cosas geniales que tiene esta certificación es que el modelo de precios es muy cómodo y flexible además de ser relativamente barato. En mi caso particular, debido a que yo tengo un trabajo pude comprar en oferta el plan **anual silver**, lo que me permitió tener acceso a dos vouchers de examen y a 5 **Paths de aprendizaje**. 

En caso de que seas estudiante, puedes aprovechar el plan especial que ofrece **HTB Academy**. Para acceder, solo debes verificar que te encuentras estudiando. No es necesario crear una cuenta nueva, ya que HTB permite registrar un correo electrónico secundario, donde puedes añadir tu dirección institucional para completar la validación.

> **Importante:** no podrás activar el voucher hasta completar el 100% del Penetration Tester Job Role Path.
{: .prompt-warning }

#### Resumen de los precios - Plan Estudiante

- **Precio**: $8 / por mes

#### Resumen de los precios - Plan Silver Annual

- **Precio**: $490 / anual
- **Beneficios**
	- 2 vouchers de examen
	- 5 rutas de aprendizaje
	- 289 módulos incluidos 


#### Resumen de los precios - Voucher CPTS

-  **Precio**: $210

> Sea el que elijas, vas a tener **2** oportunidades para rendir el examen
{: .prompt-info }

-----

## 2. Penetration Tester Job Role Path

El **Penetration Tester Job Role Path** contiene los conocimientos necesarios para afrontar el examen. En esta etapa, mi principal recomendación es que tomes apuntes lo más detallados, claros y ordenados posible.

Durante el examen, es muy probable que necesites consultar rápidamente un comando, una técnica o algún procedimiento específico. Si tus notas están redactadas a la rápida o carecen de una estructura clara, perderás tiempo intentando recordar en qué módulo o sección viste esa información. Un buen sistema de apuntes puede marcar una gran diferencia.

Los módulos que, según mi experiencia, considero más importantes y críticos para afrontar el examen son los siguientes:

- **Web Attacks**: Aquí encontraras varios módulos que cubren vulnerabilidades web (SQLI, XXE, IDOR, File Upload, etc). 
- **Attacking Common Apps & Services**: Este modulo cubre ataques a objetivos como los CMS (WordPress, Drupal, etc) y servicios comunes como lo es SMB, FTP y NFS
- **Pivoting**: Este modulo enseña técnicas de pivoting desactualizada, no es que este mal ni nada, pero hay mejores herramientas para esta parte y que te ahorraran mas tiempo.
- **Privilege Escalation**: La escalada de privilegios es una de las partes mas importante del examen, aquí se centra en las malas configuraciones que normalmente están presentes en el mundo real
- **Active Directory**: Esta parte es la que mas atención debes ponerle ya que cubre técnicas como Kerberoasting, AS-REP Roasting, captura de trafico con Responder y la relación de confianza entre bosques (Domain Trusts/Cross-Forest)
- **Attacking Enterprise Networks (AEN)**: Este es, probablemente, el módulo más importante de toda tu preparación técnica, ya que te permite poner a prueba tu metodología en un entorno muy similar al que enfrentarás durante el examen. Mi recomendación es que intentes completarlo por tu cuenta, sin consultar el paso a paso ni las soluciones. Si logras avanzar y comprometer el entorno utilizando únicamente tu propia metodología, tendrás una buena señal de que tu proceso de trabajo está bien estructurado y suficientemente pulido para afrontar el examen.
- **Documentation & Reporting**: Y aquí llegamos al módulo final del **Penetration Tester Job Role Path**, uno de los más importantes de toda la ruta. Este módulo debe convertirse en tu guía principal para aprender a documentar correctamente el trabajo realizado. El examen está diseñado con un equilibrio cercano al **50/50 entre la ejecución técnica y la calidad del reporte**. Esto significa que no basta con comprometer toda la red: si el informe no está bien estructurado, redactado y respaldado con evidencias claras, puedes reprobar igualmente. Por eso, toma apuntes detallados de cada recomendación, estructura y ejemplo que aparezca en este módulo, y construye tu metodología de documentación a partir de ellos.

----

## 3. Mi tiempo de estudio y preparación

Vamos desde el principio. Comencé el **Penetration Tester Job Role Path** el 25 de agosto de 2025 y lo terminé el 6 de junio de 2026. En total, fueron **41 semanas de estudio continuo**. Pero ¿por qué tanto tiempo?

Yo no llegué a la CPTS partiendo desde cero. Un par de meses antes, el 15 de junio de 2025, había rendido y aprobado la certificación **eJPT**. Sin embargo, la preparé principalmente resolviendo máquinas y enfrentándome a laboratorios prácticos, sin profundizar demasiado en la teoría que explicaba por qué funcionaba cada técnica.

Esa experiencia me ayudó a desarrollar habilidades prácticas, pero también me hizo darme cuenta de que muchas veces sabía **qué comando ejecutar**, aunque no siempre comprendía completamente **por qué debía ejecutarlo, qué estaba ocurriendo detrás o en qué otros escenarios podía aplicarlo**. Por eso, al comenzar la preparación para la CPTS, decidí cambiar mi forma de estudiar y construir una base mucho más completa, combinando práctica, teoría y documentación detallada. Esa fue una de las principales razones por las que completar el Path me tomó 41 semanas.

Mi metodología de estudio consistió en registrar no solo los comandos, sino también su propósito, el contexto en el que debían utilizarse, la razón por la que una vulnerabilidad podía existir y ejemplos de otros escenarios en los que esa misma técnica podía aplicarse. Esto hizo que mis apuntes fueran mucho más extensos y que avanzara con mayor lentitud, pero también me permitió construir una fuente de consulta mucho más útil.

La memoria es frágil y, según mi experiencia, es mucho mejor tener siempre a mano la explicación de por qué suceden las cosas. Esto te permite comprender mejor cada técnica y evita que termines limitándote a copiar y pegar comandos sin entender realmente su funcionamiento. Esa forma de estudiar fue la principal razón por la que tardé tanto tiempo en completar la ruta.

Así que, como consejo, **no te apresures por terminar el Path lo antes posible**. Tómate el tiempo necesario para comprender realmente cada técnica, concepto y procedimiento que vayas estudiando.

Puede que tardes más que yo o que logres completarlo en menos tiempo; eso dependerá de tu experiencia previa, disponibilidad y forma de aprender. Lo verdaderamente importante es desarrollar una mentalidad en la que primero busques **entender y comprender antes de ejecutar**. Ese enfoque marcará la diferencia entre limitarte a repetir comandos y saber realmente qué estás haciendo, por qué funciona y cuándo debes aplicarlo.

### Como me prepare después de terminar el Path

Jejeje, en esta parte, más que contarte lo que hice, **prefiero decirte lo que no hice**, para que tú no cometas los mismos errores.

Cuando contraté el plan anual, ese mismo día definí la fecha en la que rendiría el examen. Además, dejé reservado aproximadamente un mes para prepararme antes de utilizar el segundo intento, en caso de reprobar el primero. El problema fue que no consideré cuánto tiempo me tomaría realmente completar el **Penetration Tester Job Role Path**.

Cuando finalmente terminé la ruta, solo me quedaba una semana y media antes de la fecha que yo mismo había establecido para rendir el examen.

Como consecuencia, mi preparación posterior al Path fue bastante limitada. Alcancé a resolver únicamente tres laboratorios de una playlist no oficial de **IppSec**. Para aprovechar mejor el poco tiempo disponible, creé un prompt en **Claude AI** para que actuara como profesor y me ayudara a estructurar un plan de estudio.

Claude me permitió organizar esa semana de manera mucho más eficiente, destinando cerca del **90 % del tiempo a Active Directory**, que era el área en la que me encontraba más débil. Para mi suerte, el plan de trabajo que me entregó fue una de las mejores decisiones que pude tomar, ya que me permitió repasar conceptos fundamentales que posteriormente aparecieron durante el examen.

Por último, repetí aproximadamente dos veces el módulo **Attacking Enterprise Networks (AEN)**, ya que era el simulacro más cercano al examen que tenía disponible en ese momento.

## Haz lo que yo no hice

Muchas de las recomendaciones que mencionaré a continuación las fui aprendiendo durante la semana previa al examen e incluso mientras lo estaba realizando.

### Realiza el track de la CPTS en HTB

Las máquinas incluidas en este track reúnen gran parte de los conceptos y técnicas que necesitarás dominar. No se trata únicamente de comprometerlas, sino de utilizarlas para practicar enumeración, explotación, movimiento lateral, escalada de privilegios y documentación.

### Repite Attacking Enterprise Networks

Como ya he mencionado varias veces, **Attacking Enterprise Networks (AEN)** es uno de los simulacros más fieles que tendrás antes de rendir el examen.

Repítelo todas las veces que consideres necesarias e intenta completarlo utilizando tu propia metodología. Evita consultar el paso a paso o las soluciones, salvo que realmente lleves mucho tiempo bloqueado y ya hayas agotado tus alternativas.

### Aprende de la metodología de otras personas

Cuando veas un video sobre la resolución de una máquina, no te concentres únicamente en los comandos o en la parte técnica. Observa cómo la persona analiza la información que entrega el entorno, cómo organiza la enumeración, qué hipótesis plantea y cómo decide cuál será su siguiente paso.

Comprender la metodología de otros profesionales puede ayudarte a mejorar tu propia forma de pensar y de resolver problemas. Personalmente, recomiendo encarecidamente el contenido de **S4vitar** e **IppSec**.

### Practica tus apuntes y la documentación

El primer informe profesional completo que redacté en mi vida fue el que entregué para el examen y con el cual conseguí aprobar. Durante la semana previa, algo que sí hice fue documentar los hallazgos de las máquinas siguiendo las recomendaciones del módulo **Documentation & Reporting**.

Esto me permitió llegar al examen con una idea más clara de la estructura que utilizaría para organizar mis evidencias y redactar el documento final.

Llegar al examen sin haber escrito antes un informe profesional no significa necesariamente que vayas a reprobar, pero sí puede hacer que el proceso sea mucho más difícil. Mi recomendación es que, con cada máquina que utilices para prepararte, documentes los hallazgos utilizando una estructura consistente y redactes un pequeño informe profesional.

Esto te ayudará en varios aspectos:

- **Crear tu propio formato de trabajo:** podrás definir cuántos niveles de encabezados utilizarás, cómo escribirás los títulos, cómo nombrarás las fases y de qué manera organizarás las capturas de pantalla.
- **Conocer cada sección del informe:** practicar previamente te permitirá redactar con mayor rapidez y evitará que pierdas tiempo durante el examen investigando qué información corresponde incluir en cada apartado.
- **Practicar la asignación del CVSS:** aunque no es la parte más compleja del informe, es importante familiarizarte con la métrica y aprender a justificar correctamente la puntuación.
- **Mejorar tus recomendaciones:** redactar informes te ayudará a desarrollar la capacidad de proponer medidas de mitigación claras, realistas y alineadas con la vulnerabilidad identificada. También aprenderás dónde buscar información confiable y cómo transformar una solución técnica en una recomendación comprensible para el cliente.

----

## 4. Mi experiencia del examen

Te diré la verdad: el examen es duro, y más aún si nunca has trabajado algunas de las áreas que evalúa. En mi caso, **logré aprobarlo en el segundo intento**, y gran parte de lo que aprendí durante el proceso no estuvo relacionado únicamente con lo técnico, sino también con la forma de enfrentar los bloqueos, administrar el tiempo y mantener la cabeza fría.

Ten en cuenta que, apenas comience el examen, probablemente vas a quemarte la cabeza durante un par de días. La parte web puede parecer extensa y, en cierta medida, lo es. Yo estuve atrapado durante dos días y medio, y llegué a frustrarme porque sentía que ya había enumerado todo lo habido y por haber, pero aun así no encontraba la pieza inicial del rompecabezas. Lo que finalmente me ayudó fueron tres cosas:

1. **Tomar un descanso**: estar 9 horas sentado no te va a dar la solución; necesitas refrescar la cabeza para volver a pensar mejor.
2. **Tener una pizarra**: la pizarra fue mi segundo mejor amigo durante el examen. Es verdad que hay páginas como Excalidraw y draw.io para dibujar tus diagramas mentales, pero no hay nada que se compare con llevar tus pensamientos a algo real, que puedas sentir y que te aleje de la pantalla unos minutos.
3. **Los apuntes**: antes de entrar al examen, tomé como base el módulo de **Documentation & Reporting** y creé mi propia plantilla con los puntos que debía enumerar de un servicio o página web. Esto me ayudó a llevar un control de las cosas que probé y dónde las probé.

Una vez conseguí el acceso inicial a la DMZ01, tocaba pivotar, y la herramienta perfecta para el trabajo fue **ligolo-ng**, que me acompañó durante todo el examen. Una de las cosas que más me costó fue **ver y hacer lo fácil**: me quedé estancado muchas veces, específicamente en SRV01 y WKS01. Estas dos máquinas fueron mi dolor de cabeza, y no porque la respuesta fuera difícil —de hecho es lo contrario—. Te lo cuento por partes.

En SRV01 encontré la respuesta apenas llegué al sistema. Decidí probar una herramienta que entregaba el Path, pero no funcionó, así que busqué una segunda alternativa que tampoco funcionó. El peor error que cometí fue no haber buscado una tercera, y esto llevó a que perdiera mucho tiempo.

Para WKS01 fue algo similar: llegué al sistema y encontré algo que llamaba la atención a la vista. Al buscar en internet, di con dos formas distintas de avanzar para el mismo objetivo, y mi error aquí fue perder el tiempo intentando la forma compleja: creé un script dentro del mismo sistema para que funcionara, e incluso le instalé Python :/. El resultado fue que insistí en algo que sabía que no funcionaba, buscándole la quinta pata al gato, cuando la respuesta era tan fácil y obvia que bastaba con mirar un poco —sin abrir ningún archivo ni nada, solo el escritorio de Windows—.

Colega, tú que estás en el examen y buscas una salida: mi mejor consejo es que pienses en lo básico. Sea cual sea la etapa del examen en la que estés, el consejo se repite en cada una de ellas. No busques 1 o 2 formas de hacer algo y descartes la opción; investiga más, busca 3, 4 o hasta 5 formas de hacerlo, y ya verás que vas a encontrar la solución en una de esas. A mí me pasaba que, apenas veía el entorno, mi cabeza ya sabía la respuesta, pero el no investigar más y descartar rápido me costó mucho. Vuelve a tus apuntes del Path, revisa las playlists de IppSec y el track de HTB. Eso hice yo cuando me estanqué en AD y, créeme, la respuesta está ahí.

Lo último, pero no por eso menos importante, es el informe. Este lo empecé a redactar desde el día 1: cada cadena de ataque o vulnerabilidad encontrada la documentaba al final del día. El reporte al principio me quedó desordenado, porque no tenía una estructura base, así que técnicamente tuve que modificar y estandarizar todo el documento. Eso me tomó varios días y toda una noche, pero es mejor eso que estar a última hora empezando de cero.

Bueno, esa es mi experiencia y aprendizaje en el examen. Fue duro, no tanto por lo técnico sino por cómo uno piensa, y es por eso que te dejo estos consejos: me hubiera gustado que alguien me los dijera tal cual. Para finalizar esta parte, te dejo los días que me tomó cada flag durante el examen:

### Primer intento

- Día 1-3: Flag 1
- Día 4:   Flags 2 y 3
- Día 5:   Flag 4
- Día 8:   Flag 5
- Día 9:   Flags 6 y 7

### Segundo intento

Este intento me lo tomé mucho más relajado que el primero. Durante los primeros 3 días me enfoqué en reconstruir el informe y en realizar algunos ajustes estéticos en SysReptor; en los días 8-10, empecé a documentar toda la cadena de ataque de AD y algunos hallazgos que me faltaban documentar o pulir.

- Día 4:   Flags 8 y 9
- Día 5:   Flags 10 y 11
- Día 7:   Flag 12
- Día 8-10: Perfeccionar el informe

### Resultados 

Los resultados me los entregaron súper rápido, 32 horas después de haber terminado el examen 

![](/assets/aprove.png)
