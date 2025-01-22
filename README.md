# ForoHub -
Desafio final para el programa Alura ONE (Oracle Next Education)
Foro Hub - API REST

Foro Hub es una API REST diseñada para simular distintos endpoints de un foro, permitiendo a los usuarios iniciar sesión, crear nuevos tópicos, modificarlos y realizar su eliminación lógica dentro de una base de datos. Este proyecto es parte del programa de formación ALura Latam ONE (Oracle Next Education).

⚙️ Funcionalidades del proyecto

    Login Usuario: Obtención del JSON Web Token (JWT) para acceder a las demás funciones de la API.
    Registrar Tópicos: Método POST para agregar nuevos registros en la base de datos.
    Listar Tópicos: Método GET que devuelve la lista de todos los tópicos almacenados.
    Actualizar Tópico: Método PUT para modificar un tópico existente, indicando su id en el path de la request.
    Eliminar Tópico: Método DELETE para eliminar un tópico, utilizando su id en el path de la request. (Eliminación lógica para mantener la integridad de los datos).

¿Cómo funciona?

Esta aplicación está desarrollada con Spring Framework, que se encarga de la gestión y seguridad de los endpoints, mientras que JWT se utiliza para la autenticación de usuarios. Cuando un usuario envía una solicitud de inicio de sesión a la ruta correspondiente, obtiene acceso a diversas operaciones sobre los tópicos, como consultarlos, crearlos, editarlos o eliminarlos.

Los tópicos generados se almacenan en una base de datos MySQL. Al consultar o modificar un tópico, se muestra el nombre del usuario que lo creó o realizó la última actualización. En cuanto a la eliminación, para preservar la integridad de la base de datos y mantener los registros, esta se maneja de manera lógica en lugar de eliminar físicamente los datos.
Instalación

    Descargue o clone el repositorio del proyecto.
    Abra el proyecto en el IDE de su elección.
    Instale las dependencias indicadas en el archivo pom.xml.
    Configure las propiedades necesarias del proyecto.
    Ejecute la aplicación.

Nota: Es imprescindible contar con MySQL instalado y configurado para gestionar la base de datos
