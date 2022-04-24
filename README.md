### Implementacion basica React en Rails

Esta es una pequeña guia personal para configurar un proyecto rails desde cero con la configuracion basica para funcionar con react js y un ejemplo de configuracion.

1. Crear aplicacion rails
    ```sh
      rails _6.1.5_ new react_on_rails --postgresql
    ```
    O
    ```sh
      rails new react_on_rails --postgresql
    ```
    O
    ```sh
      rails new react_on_rails
    ```
2. Ubicarse en el proyecto
    ```sh
      cd react_on_rails
    ```
3. Correr Gemas basicas
    ```sh
      bundle
    ```
4. Ir a la documentacion oficial de la gema react_on_rails
[https://github.com/shakacode/react_on_rails](https://github.com/shakacode/react_on_rails)
[https://www.shakacode.com/react-on-rails/docs/getting-started/](https://www.shakacode.com/react-on-rails/docs/getting-started/)
5. Agregar en el gemfile
    ```ruby
      gem "react_on_rails", "= 13.0"
    ```
6. Correr Gemas
    ```sh
      bundle
    ```
7. React on rails requiere un commit 
    ```sh
      git init; git add .; git commit -m "configuracion inicial proyecto rails"
    ```
8. Se genera la estructura basica y ejemplo basico de react en rails
    ```sh
      rails generate react_on_rails:install
    ```
9. reemplaze todos los archivos que recomienda el comando anterior
10. hagamos un prueba que puede darnos error
    ```sh
      rails s
    ```
11. ingresamos a la url de prueba
[http://localhost:3000/hello_world](http://localhost:3000/hello_world)
12. Si sale el siguiente error (Webpacker can't find hello-world-bundle.js in ...) seguir con los siguiente pasos
12. Cerrar el servidor de rails
crtl c
13. se corre el siguiente comando para corregir el error anterior
    ```sh
      bundle exec rails webpacker:install
    ```
14. reemplaze todos los archivos que recomienda el comando anterior
15. se corre el siguiente comando para corregir el error anterior
    ```sh
      bundle exec rails webpacker:install:react
    ```
16. hagamos otra prueba
    ```sh
      rails s
    ```
17. ingresamos a la url de prueba
[http://localhost:3000/hello_world](http://localhost:3000/hello_world)
18. Todo perfecto Fin :D


Creacion de un controlador vista y metodo de ejemplo
