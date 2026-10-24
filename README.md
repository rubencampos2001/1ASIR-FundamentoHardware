# Proyecto Fundamentos de Hardware \- Taller Rubenshicar

Este es mi trabajo del módulo de **Fundamentos de Hardware**, que entra dentro del Proyecto Intermodular de 1º de ASIR. Básicamente lo que me han pedido es pensar qué ordenadores y qué hardware necesitaría un negocio pequeño para funcionar, y yo he escogido un taller mecánico de barrio. En el documento voy contando qué equipos harían falta, qué lleva cada uno por dentro, cómo guardar los datos y qué mejoras se podrían ir haciendo si el taller va creciendo.

## Quién lo hace y cuándo

- **Alumno:** Rubén Campos  
- **Curso:** 1º ASIR  
- **Módulo:** Fundamentos de Hardware  
- **Curso académico:** 2025/2026  
- **Tema elegido:** Taller mecánico pequeño

## De qué va el trabajo

Me he inventado un taller pequeño de barrio y le he puesto de nombre **Taller Rubenshicar**. Es un negocio familiar con tres personas: el jefe (que lleva también las cuentas), un mecánico y una chica en recepción. Tienen un volumen de trabajo medio, o sea que están ocupados pero tampoco es una cadena grande. Las cosas que hacen con el ordenador son las típicas de una empresa así: facturar, pasar presupuestos, llevar la agenda de citas, buscar piezas en internet, imprimir albaranes y consultar manuales de los coches.

## Qué hay en la carpeta

| Fichero | Qué es |
| :---- | :---- |
| `Proyecto_Fundamentos_Hardware_Taller.pdf` | El documento entero del proyecto |
| `manual-hardware/Manual_Fundamentos_Hardware_Ruben_Campos.pdf` | Manual práctico de hardware y herramientas de diagnóstico (actividad entregable) |
| `README.md` | Este archivo, para presentar el repo |

## Cómo está montado el documento

El documento lo he dividido en siete apartados, siguiendo más o menos el orden que nos pedían en clase:

1. **Introducción y contexto** — presento el taller y cuento lo que voy a hacer.  
2. **Análisis de necesidades de hardware** — miro qué hace falta en cada puesto.  
3. **Componentes de un equipo informático** — explico por encima la CPU, la RAM, la placa base, los discos, la fuente y las tarjetas.  
4. **Configuración de hardware propuesta** — aquí pongo los equipos concretos con marca, modelo y **precio aproximado**.  
5. **Sistema de almacenamiento** — comparo SSD con HDD, hablo de capacidades y del NAS con RAID 1\.  
6. **Comparativa y posibles mejoras** — qué cambiaría a corto plazo y qué haría si el taller crece.  
7. **Conclusión** — lo que he sacado en claro haciendo el trabajo.

## Resumen rápido de lo que monto

- **PC del jefe:** i5-12400, 16GB DDR4, SSD NVMe 500 GB \+ HDD 1 TB. Sobre **630 €**.  
- **PC de recepción:** i3-12100, 8 GB DDR4, SSD NVMe 250 GB. Sobre **425 €**.  
- **Tablet del mecánico:** Lenovo Tab M10 \+ funda rugged \+ adaptador OBD-II. Sobre **205 €**.  
- **Zona compartida:** NAS Synology DS223j con 2x WD Red Plus 4 TB en RAID 1, impresora Brother, router WiFi 6, SAI, lector de códigos y un disco externo. Sobre **855 €**.  
- **Total inicial: unos 2.115 €** (sólo hardware, no cuento software ni licencias).

## Las copias de seguridad

Para no perder datos si pasa algo, he montado un plan en tres pasos:

- Los PCs hacen backup automático al NAS por las noches.  
- El NAS tiene dos discos en RAID 1, así que si muere un disco los datos siguen ahí.  
- Una vez por semana se copia todo a un disco externo USB que se lleva el jefe a casa. Así hay una copia fuera del taller por si pasa algo gordo (robo, incendio, lo que sea).

## Sobre la rúbrica

Estos son los puntos que me piden y que he intentado cubrir:

- [x] Análisis de necesidades de hardware  
- [x] Componentes del sistema  
- [x] Configuración propuesta (con precios aproximados)  
- [x] Sistema de almacenamiento  
- [x] Mejora o evolución del sistema  
- [x] Organización y documentación (repositorio \+ README)

## Cómo abrirlo

Solo hay que abrir el fichero `Proyecto_Fundamentos_Hardware_Taller.pdf` (se ve directamente en GitHub o con cualquier lector de PDF).

## 🔧 Manual práctico de hardware (actividad entregable)

Además del proyecto del taller, en [`manual-hardware/`](manual-hardware/Manual_Fundamentos_Hardware_Ruben_Campos.pdf) está el manual que hice para el módulo (37 páginas):

| Apartado | Qué hice |
|---|---|
| Configuración de equipos | Diseño de un PC para dibujo técnico (Ryzen 7 9700X, RTX 5050, 32 GB DDR5) con BuildCores |
| Placa base | Identificación de 17 componentes de una ASRock M3A785GMH |
| Montaje y mantenimiento | Guía de montaje en 10 fases, errores que evitar y plan de mantenimiento preventivo |
| Clonezilla | Clonación partición a partición paso a paso |
| RAID 6 | Funcionamiento con doble paridad, ventajas e inconvenientes |
| Información de componentes | CPU-Z y CrystalDiskInfo (S.M.A.R.T.) |
| Benchmarks | UserBenchmark y CrystalDiskMark, con análisis de resultados y problemas corregidos |
| Arranque desde UEFI | MemTest86 (0 errores) y GParted |
| Kali Linux | Instalación y configuración UEFI (Secure Boot, modo de arranque) |

## Licencia

Trabajo hecho como parte del Ciclo Formativo de Grado Superior en **Administración de Sistemas Informáticos en Red (ASIR)**. Libre para uso educativo.  
