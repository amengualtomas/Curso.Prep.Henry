* Funciones Callback:

Una función de callback es una función que se pasa a otra función como un argumento, que luego se invoca dentro de la función externa para completar algún tipo de rutina o acción.

ejemplo.

function decirHolaAlUsuario(usuario) {
    return 'Hola ' + usuario + '!';
}

function decirAdiosAlUsuario(usuario) {
    return 'Adiós ' + usuario + '!';
}

function crearSaludo(usuario, cb) {
    return cb(usuario);
}