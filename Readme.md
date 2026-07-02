ráctica 4 - Pruebas de Rendimiento con Apache JMeter
INF780 – Verificación y Validación de Software
Estudiante
Mauren Fernanda Villca Salas

Docente
M. Sc. Huáscar Fedor Gonzales Guzmán

Descripción
En esta práctica se realizaron pruebas de rendimiento sobre la API Movies API desarrollada en NestJS utilizando Apache JMeter 5.6.3.

Se ejecutaron los siguientes escenarios:

Smoke Test
Prueba de Carga
Prueba de Estrés
Prueba de Picos (Spike)
Tecnologías utilizadas
Apache JMeter 5.6.3
Java OpenJDK 21
NestJS
PostgreSQL
Node.js
JMETER-PRUEBAS/
│
├── reporte_estres_100/
├── reporte_estres_200/
├── reporte_estres_400/
├── reporte_picos/
│
├── carga.jmx
├── estres_100.jtl
├── estres_200.jtl
├── estres_400.jtl
├── estres.jmx
├── ids.csv
├── jmeter.log
├── picos.jmx
├── picos.jtl
├── Readme.md
└── smoke.jmx
├── Capturas e informe/

Ejecución
Iniciar PostgreSQL.
Levantar la API:
npm run start:dev
Abrir Apache JMeter.
Abrir el archivo .jmx correspondiente.
Ejecutar la prueba.
Escenarios
Escenario	Configuración
Smoke	1 usuario, Ramp-up 1 s, Loop 5
Carga	50 usuarios, Ramp-up 30 s, Loop 10
Estrés	100, 200 y 400 usuarios
Picos	200 usuarios, Ramp-up 5 s, Loop 10
Resultados
Los resultados obtenidos se encuentran en el informe PDF y en las capturas incluidas en el repositorio.