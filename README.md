
CULTURA DIGITAL Y SOCIEDAD
Actividad Autónoma 5
Unidad 3: Datos, Privacidad y Seguridad en la Era Digital
Tema 1: Privacidad de Datos y Normativas Digitales


Nombres:Angel Quiguiri
Carrera: Ciencia de Datos 
Semestre:Tercero
 
Objetivo de la actividad:
Analizar e implementar técnicas de anonimización de datos respetando normativas internacionales como el GDPR y la CCPA, desarrollando pensamiento crítico sobre la ética y privacidad en el contexto de la Ciencia de Datos.
Recursos o temas que debe haber estudiado antes de hacer la actividad:
Conceptos clave de privacidad digital y normativas: GDPR, CCPA, LGPD.
Casos de estudio sobre ética de datos (COMPAS, reconocimiento facial, publicidad algorítmica).
Formato de entrega: PDF (máximo 5MB)
PDF con evidencias, capturas de pantalla, código comentado y reflexiones.
Debe incluir un enlace a GitHub con el código completo y documentación
Instrucciones:


PARTE 1: Análisis Crítico de Normativas
Responde las siguientes preguntas con un mínimo de 10 líneas por ítem, debe ser realizado a mano:
1.	Diferencia principal entre GDPR y CCPA en cuanto al consentimiento del usuario y el derecho al olvido
El GDPR (Reglamento General de Protección de Datos de la UE) y el CCPA (Ley de Privacidad del Consumidor de California) tienen enfoques distintos frente al consentimiento y el derecho al olvido. En el GDPR, el consentimiento debe ser explícito, informado, inequívoco y otorgado mediante una acción afirmativa clara (como marcar una casilla o firmar). No se permite el consentimiento implícito ni preseleccionado. Además, el GDPR reconoce el “derecho al olvido” (Artículo 17) de manera amplia: una persona puede solicitar la eliminación de sus datos cuando ya no sean necesarios, cuando retire su consentimiento, o cuando se oponga al tratamiento. En cambio, el CCPA tiene un modelo basado más en el “opt-out” (exclusión voluntaria): los consumidores deben tener la opción de decir que no se vendan sus datos personales, pero no se requiere un consentimiento explícito previo para la recolección. El derecho al olvido en CCPA es más limitado; permite solicitar la eliminación de datos, pero con más excepciones (por ejemplo, si la empresa necesita los datos para completar una transacción o por razones de seguridad interna). En resumen, el GDPR protege los datos desde el origen (consentimiento explícito), mientras que el CCPA da control posterior al consumidor (opt-out y eliminación limitada).

2.	Caso real de violación a normativa de privacidad y consecuencias
Un caso emblemático es el de British Airways ante el GDPR. En 2018, la aerolínea sufrió un ciberataque que expuso los datos personales y financieros de aproximadamente 500,000 clientes. La Oficina del Comisionado de Información del Reino Unido (ICO) impuso una multa inicial de £183 millones (luego reducida a £20 millones por circunstancias atenuantes y por el impacto de la pandemia). La violación consistió en que los atacantes desviaron el tráfico del sitio web y la aplicación de British Airways hacia un sitio falso, capturando nombres, direcciones de correo, números de tarjeta de crédito y códigos CVV. La ICO determinó que British Airways no implementó medidas técnicas y organizativas suficientes para garantizar la seguridad de los datos, incumpliendo así el Artículo 32 del GDPR. Este caso demostró que las consecuencias pueden ser no solo económicas (multas millonarias), sino también daño reputacional, pérdida de confianza de los clientes y mayor escrutinio regulatorio. Posteriormente, British Airways invirtió fuertemente en mejorar su ciberseguridad y auditorías internas.
3.	Retos de las pequeñas empresas para cumplir estas normativas
Las pequeñas empresas enfrentan retos significativos para cumplir con normativas como GDPR o CCPA. En primer lugar, carecen de equipos legales o de cumplimiento dedicados, por lo que entender e interpretar textos legales complejos consume tiempo y recursos. En segundo lugar, implementar medidas técnicas como el cifrado de datos, la anonimización o los sistemas de gestión de consentimientos requiere inversiones en software, capacitación o consultoría externa, lo cual puede resultar prohibitivo. En tercer lugar, las pequeñas empresas suelen depender de terceros (proveedores de nube, herramientas de marketing, CRMs) que también deben cumplir, lo que añade capas de responsabilidad compartida y complejidad contractual. Otro reto importante es la gestión de solicitudes de los usuarios (acceso, rectificación, olvido), que puede desbordar la capacidad operativa de un negocio pequeño. Finalmente, muchas pequeñas empresas desconocen siquiera la existencia de estas normativas o creen erróneamente que no aplican por su tamaño. Esto las expone a multas o sanciones que pueden ser devastadoras financieramente.
4.	Influencia de las regulaciones en el diseño de proyectos de Ciencia de Datos
Las regulaciones de privacidad como GDPR y CCPA han transformado el diseño de proyectos de Ciencia de Datos. Primero, impulsan el principio de Privacidad desde el Diseño (Privacy by Design), lo que significa que la protección de datos debe integrarse en todas las fases del proyecto: desde la recolección hasta el almacenamiento y el análisis. Segundo, obligan a minimizar la recolección de datos: solo se deben capturar aquellos estrictamente necesarios para el objetivo planteado, abandonando la vieja práctica de “recolectar todo por si acaso”. Tercero, exigen documentar el consentimiento y los propósitos del tratamiento, lo que lleva a crear registros detallados de linaje de datos. Cuarto, limitan el uso de datos para fines secundarios no autorizados. Quinto, requieren técnicas de anonimización o seudonimización antes de compartir o publicar datasets. Sexto, los proyectos que utilizan machine learning deben evitar sesgos discriminatorios y garantizar la posibilidad de explicabilidad, especialmente si se toman decisiones automatizadas que afecten a personas. Finalmente, incorporar estos requisitos desde el inicio reduce riesgos legales y genera confianza con los usuarios, pero también puede aumentar los tiempos de desarrollo y la necesidad de perfiles interdisciplinarios (abogados + científicos de datos).

PARTE 2: Investiga los tres casos propuestos:
Introducción 
La ética de datos es una rama aplicada de la ética que examina cómo recolectar, procesar, almacenar y utilizar los datos personales respetando los derechos humanos, la privacidad y la justicia social. En la sociedad actual, donde algoritmos y grandes volúmenes de información influyen en decisiones clave (contratación, crédito, justicia, salud), la ética de datos se vuelve imprescindible. Sin un marco ético sólido, los sistemas basados en datos pueden perpetuar desigualdades, discriminar a grupos vulnerables o vulnerar la autonomía de las personas. La creciente regulación (GDPR, CCPA) refleja esa preocupación, pero la normativa por sí sola no es suficiente; se requiere conciencia crítica por parte de científicos de datos, empresas y gobiernos. Este informe analiza tres casos concretos –COMPAS, reconocimiento facial y publicidad algorítmica– para extraer lecciones sobre cómo diseñar tecnologías más justas y transparentes.
Análisis de cada caso 
Caso 1: COMPAS (sistema de puntuación de riesgo en EE. UU.)
Problema ético principal: Sesgo algorítmico racial. COMPAS, utilizado por jueces para decidir si una persona acusada puede esperar su juicio en libertad, mostró tasas de falsos positivos más altas para personas afroamericanas que para blancas. Es decir, predecía incorrectamente que reincidirían cuando no lo hacían.
Consecuencias: Personas afroamericanas fueron encarceladas preventivamente de manera desproporcionada, aumentando la sobrepoblación carcelaria y perpetuando la injusticia racial. También se limitó el acceso a programas alternativos.
Actores involucrados: La empresa Northpointe (hoy Equivant) desarrolló el algoritmo. Los jueces y fiscales lo utilizan. Los acusados y sus defensores son afectados. Investigadores como ProPublica expusieron el sesgo.

Intereses: Northpointe buscaba vender un producto “científico” a tribunales. Los jueces querían herramientas objetivas. Los defensores buscan equidad.

Soluciones propuestas: Auditorías algorítmicas independientes, transparencia en las variables utilizadas, uso de métricas de equidad (paridad demográfica, igualdad de oportunidades), y en algunos casos, prohibición de estos sistemas en decisiones judiciales sensibles.
Caso 2: Reconocimiento facial (gobiernos y empresas)
Problema ético principal: Violación masiva de la privacidad, vigilancia desproporcionada y errores con alto impacto (falsas identificaciones). Los sistemas de reconocimiento facial tienen tasas de error más altas en personas de piel oscura, mujeres y minorías étnicas.
Consecuencias: En EE. UU., varios hombres afroamericanos fueron arrestados erróneamente por robos que no cometieron debido a falsas coincidencias. En China, el sistema de crédito social basado en vigilancia masiva genera control social extremo y disuade la disidencia.
Actores involucrados: Gobiernos (uso policial y militar), empresas tecnológicas (Amazon, Clearview AI, SenseTime), ciudadanos vigilados, grupos de derechos civiles.
Intereses: Gobiernos: seguridad y control social. Empresas: lucro con contratos públicos. Ciudadanos: privacidad y no discriminación.
Soluciones propuestas: Moratorias al uso por parte de gobiernos (varias ciudades de EE. UU. lo prohibieron), leyes como la AI Act de la UE que prohíben el reconocimiento facial en tiempo real en espacios públicos, mejora de datasets más diversos, y derecho a la revisión humana antes de tomar acciones adversas.
Caso 3: Publicidad algorítmica (Google/Facebook)
Problema ético principal: Manipulación, microsegmentación que permite exclusión discriminatoria y creación de burbujas de filtro. Los anuncios pueden dirigirse a grupos específicos excluyendo a otros por raza, género, religión o ingresos.

Consecuencias: Anuncios de vivienda que excluían a personas afroamericanas o hispanas (violación de leyes de vivienda justa en EE. UU.). Anuncios laborales que no se mostraban a mujeres mayores. También se ha usado para difundir desinformación política o aprovechar vulnerabilidades psicológicas.

Actores involucrados: Plataformas (Meta, Google), anunciantes, usuarios blanco, reguladores, competidores.

Intereses: Plataformas: maximizar ingresos publicitarios mediante segmentación precisa. Anunciantes: llegar a sus “clientes ideales”. Usuarios: información relevante pero sin ser manipulados o discriminados.

Soluciones propuestas: Transparencia en los criterios de segmentación, herramientas de “Ad Library” (Meta) para ver anuncios activos, auditorías externas, leyes como la Digital Services Act (UE) que exigen repositorios públicos de anuncios políticos, y opciones de “menos segmentación”.
Reflexión final 
Modelo:
Estos tres casos revelan una verdad incómoda: los sistemas basados en datos no son neutrales. Reflejan los sesgos históricos, las decisiones de diseño y los intereses comerciales de quienes los crean y despliegan. El caso COMPAS muestra cómo un algoritmo “objetivo” puede replicar la discriminación racial sistémica. El reconocimiento facial evidencia que la falta de diversidad en los datos de entrenamiento daña concretamente a minorías. La publicidad algorítmica demuestra que incluso sin intención maliciosa, los modelos de optimización de ingresos pueden violar derechos civiles.

Los principios éticos que deberían guiar el desarrollo tecnológico incluyen: (1) Transparencia: explicar cómo funciona el algoritmo y qué datos usa. (2) Equidad: auditar regularmente en busca de sesgos adversos. (3) Responsabilidad: establecer quién responde cuando el sistema causa daño. (4) Privacidad por diseño: minimizar datos y anonimizar siempre que sea posible. (5) Supervisión humana significativa, especialmente en decisiones con alto impacto.

Aprendo que la ciencia de datos no puede limitarse a la eficiencia predictiva; debe incorporar valores democráticos y derechos humanos desde la concepción del proyecto. La ética no es un añadido opcional, sino una competencia central del científico de datos contemporáneo.
Bibliografía:
•	Dwork, C. (2006). Differential privacy.
•	Sweeney, L. (2002). k-Anonymity: A model for protecting privacy.
•	Mehrabi et al. (2022). A Survey on Bias and Fairness in Machine Learning.
•	Reglamento General de Protección de Datos (GDPR): https://gdpr-info.eu/
•	Ley de Privacidad del Consumidor de California (CCPA): https://oag.ca.gov/privacy/ccpa
