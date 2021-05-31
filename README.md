# Smart Monkey

En esta rama se detalla el procedimiento para ejecutar pruebas de reconocimiento con Smart Monkey sobre GHOS v3.42.5

## Prerequisito

Node,              Version  12.17.0
Cypress,           Version  7.2.0
Chrome,            Version  90.0.4430.93
Git,               Version  2.21.0
Ghost ,            Version  3.42.5

## Procedimiento para la ejecución de Smart Monkey

1. Iniciar GHOST
2. Clonar este repositorio
3. Moverse al directorio raíz del repositorio con el comando cd JWDA-Semana8/
4. Hacer checkout en la rama Smart_monkey_Ghost3.42.5
5. Instalar las librerías requeridas con npm-install
6. Modificar con sus credenciales de GHOST el archivo ./integration/monkey/smart-monkey.js: poner el correo en la linea 660 y password en la linea 661
7. Ejecutar Smart-Monkey con el siguiente comando: cypress run -C smart-monkey.json
8. Al terminar la ejecución puede consultar en la carpeta de resultados el video generado por el Monkey
