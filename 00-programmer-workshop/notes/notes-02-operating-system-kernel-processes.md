\# Clase 0.2 — Sistema operativo, kernel, procesos, hilos y terminal



\## Sistema operativo



El sistema operativo es el software principal que administra los recursos de la computadora.



Administra:



\- CPU

\- RAM

\- Disco

\- Procesos

\- Archivos

\- Permisos

\- Red

\- Usuarios



\## Kernel



El kernel es el núcleo del sistema operativo.



Es la parte que se comunica de forma más directa con el hardware y administra recursos críticos como memoria, procesos, dispositivos y red.



\## Shell o terminal



La shell es un programa que permite enviar comandos al sistema operativo.



Ejemplos:



\- PowerShell

\- CMD

\- Bash

\- Zsh



\## PATH



PATH es una lista de carpetas donde el sistema operativo busca programas ejecutables.



Gracias al PATH podemos ejecutar comandos como:



```powershell

java --version

git --version

docker --version



\## Proceso 



Un proceso es una programa en ejecución 



Ejemplos: 

* Chrome abierto
* API Spring Boot corriendo



\## Hilo



Un hilo es una unidad de ejecución dentro de un proceso. Un proceso puede tener varios hilos



Diferencia entre proceso e hilo



Proceso:



Programa completo ejecutándose.



Hilo:



Camino de ejecución dentro de un proceso.

Aplicación en backend



Una API backend es un proceso.



Ese proceso puede tener varios hilos para atender varias solicitudes al mismo tiempo.



Ejemplo:



Proceso: API Spring Boot



Hilo 1: GET /tasks

Hilo 2: POST /tasks

Hilo 3: PUT /tasks/1

Hilo 4: DELETE /tasks/1

Idea clave



Si una API usa mal los recursos, puede consumir demasiada RAM, saturar la CPU o bloquear hilos.





\---



\# 12. Verificar herramientas instaladas



Ejecuta estos comandos en PowerShell:



```powershell

java --version

git --version

docker --version



Más adelante también usaremos:



mvn --version



Si alguno falla, no te preocupes. Eso nos sirve para detectar qué falta configurar.



13\. Posibles errores comunes

Error 1

java no se reconoce como un comando interno o externo



Significa normalmente una de estas dos cosas:



Java no está instalado.



O Java está instalado, pero no está configurado en PATH.

Error 2

git no se reconoce como un comando interno o externo



Significa:



Git no está instalado.



O Git no está agregado al PATH.

Error 3

docker no se reconoce como un comando interno o externo



Significa:



Docker Desktop no está instalado.



O Docker no está iniciado.



O Docker no está agregado correctamente al PATH.



14\. Trade-offs

Terminal vs interfaz gráfica

Usar interfaz gráfica



Ventajas:



Es más visual.

Es más fácil al inicio.

Sirve para tareas simples.



Desventajas:



Es más lenta para tareas repetitivas.

No siempre muestra todo lo que ocurre.

Es difícil automatizar.

Usar terminal



Ventajas:



Es rápida.

Es precisa.

Permite automatizar.

Es estándar en servidores.

Es fundamental para backend, Docker y Git.



Desventajas:



Al inicio parece menos amigable.

Un comando mal escrito puede causar errores.

Requiere práctica.

Apuntes de Oro — Terminal

Un backend developer debe sentirse cómodo usando terminal.



Git se usa mucho por terminal.



Docker se usa mucho por terminal.



Maven se usa mucho por terminal.



Los servidores reales casi siempre se administran por terminal.



Por eso no estudiaremos terminal como teoría aburrida, sino como herramienta diaria.

