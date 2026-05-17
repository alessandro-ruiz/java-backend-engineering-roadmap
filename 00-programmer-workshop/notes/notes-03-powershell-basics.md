\# Clase 0.3 — Terminal profesional con PowerShell



\## ¿Qué es PowerShell?



PowerShell es una terminal de Windows que permite ejecutar comandos para controlar archivos, carpetas, programas y herramientas de desarrollo.



\## ¿Por qué es importante para backend?



Porque muchas herramientas profesionales se usan desde terminal:



\- Java

\- Maven

\- Git

\- Docker

\- Spring Boot

\- PostgreSQL



\## Comandos esenciales



| Comando | Significado | Uso |

|---|---|---|

| pwd | Print Working Directory | Muestra la ubicación actual |

| dir | Directory | Lista archivos y carpetas |

| ls | Alias de dir | Lista archivos y carpetas |

| cd | Change Directory | Entra a una carpeta |

| cd .. | Regresar | Vuelve una carpeta atrás |

| mkdir | Make Directory | Crea una carpeta |

| New-Item | Crear elemento | Crea un archivo |

| Get-Content | Obtener contenido | Lee un archivo |

| cat | Alias de Get-Content | Lee un archivo |

| cls | Clear Screen | Limpia la pantalla |



\## Ruta absoluta



Es la ruta completa desde el disco.



Ejemplo:



```text

C:\\Users\\Carla\\Desktop\\java-backend-engineering-roadmap



\## Ruta relativa



Es una ruta escrita desde la ubicación actual.



Ejemplo:



cd 00-programmer-workshop

Comandos de archivos



Crear archivo:



New-Item practice.txt



Escribir contenido:



"Hola Backend" | Out-File practice.txt



Agregar contenido:



"Segunda línea" | Add-Content practice.txt



Leer archivo:



cat practice.txt



Copiar archivo:



Copy-Item practice.txt practice-copy.txt



Mover o renombrar:



Move-Item practice-copy.txt practice-renamed.txt



Eliminar archivo:



Remove-Item practice-renamed.txt

Idea clave



La terminal permite trabajar de forma precisa, rápida y profesional.



Un backend developer debe dominar la terminal porque Git, Docker, Maven y servidores se manejan mucho por comandos.





\---



\# 11. Errores comunes



\## Error 1: no estoy en la carpeta correcta



Síntoma:



```text id="r3tggm"

No encuentro mis archivos.



Solución:



pwd

dir



Primero mira dónde estás y qué hay ahí.



Error 2: escribí mal el nombre de la carpeta



Ejemplo:



cd 00-programmer



Pero la carpeta real se llama:



00-programmer-workshop



Solución:



dir



Mira el nombre exacto y vuelve a intentar.



Error 3: la ruta tiene espacios



Ejemplo:



cd C:\\Users\\Carla Elias\\Desktop



Puede fallar por el espacio en Carla Elias.



Solución:



cd "C:\\Users\\Carla Elias\\Desktop"



Cuando una ruta tiene espacios, usa comillas.



12\. Trade-offs

Usar terminal



Ventajas:



Es rápida.

Es precisa.

Sirve para automatizar.

Es estándar en backend.

Ayuda a entender errores reales.



Desventajas:



Al inicio parece difícil.

Requiere escribir bien.

Puede eliminar archivos si usas mal un comando.

Usar interfaz gráfica



Ventajas:



Es visual.

Es cómoda para empezar.

Reduce miedo inicial.



Desventajas:



No sirve bien para automatizar.

No muestra todos los detalles técnicos.

No es suficiente para trabajar con servidores.

