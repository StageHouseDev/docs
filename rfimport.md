# Índice

1. [Registrar Usuario](#registrar-usuario)
2. [Mi Cuenta](#mi-cuenta)
   - [Ver y Editar Información de la Cuenta](#ver-y-editar-información-de-la-cuenta)
   - [Reiniciar Contraseña](#reiniciar-contraseña)
   - [Ver Mi Estado de Cuenta](#ver-mi-estado-de-cuenta)
   - [Ver Mis Paquetes](#ver-mis-paquetes)
3. [Paquetería](#paquetería)
   - [Manejo de Guías](#manejo-de-guías)
     - [Ingresar Guía](#ingresar-guía)
     - [Editar Guía](#editar-guía)
     - [Borrar Guía](#borrar-guía)
   - [Manejo de Paquetes](#manejo-de-paquetes)
     - [Ingresar Paquete](#ingresar-paquete)
     - [Editar Paquete](#editar-paquete)
     - [Borrar Paquete](#borrar-paquete)
4. [Manejo de Cuentas](#manejo-de-cuentas)
   - [Clientes Finales](#clientes-finales)
     - [Crear Usuario](#crear-usuario-clientes)
     - [Editar Información](#editar-información-clientes)
     - [Bloquear/Desbloquear](#bloqueardesbloquear-clientes)
     - [Resetear Contraseña](#resetear-contraseña-clientes)
   - [Revendedores](#revendedores)
     - [Crear Usuario](#crear-usuario-revendedores)
     - [Editar Información](#editar-información-revendedores)
     - [Bloquear/Desbloquear](#bloqueardesbloquear-revendedores)
     - [Resetear Contraseña](#resetear-contraseña-revendedores)
     - [Editar Roles](#editar-roles)
5. [Cuentas por Cobrar](#cuentas-por-cobrar)
   - [Facturación](#facturación)
     - [Generar Factura](#generar-factura)
     - [Editar Factura](#editar-factura)
     - [Borrar Factura](#borrar-factura)
     - [Otros Servicios](#otros-servicios)
   - [Notas de Crédito](#notas-de-crédito)
     - [Crear Nota de Crédito](#crear-nota-de-crédito)
     - [Editar Nota de Crédito](#editar-nota-de-crédito)
     - [Borrar Nota de Crédito](#borrar-nota-de-crédito)
   - [Pagos](#pagos)
     - [Registrar Pago](#registrar-pago)
     - [Editar Pago](#editar-pago)
     - [Cancelar Pago](#cancelar-pago)
   - [Tarifas](#tarifas)
     - [Establecer Tarifas](#establecer-tarifas)

---

### Registrar Usuario

**1. Título del Caso de Uso:**
Registrar Usuario

**2. Descripción:**
Permite a un nuevo usuario crear una cuenta en la aplicación de RF Import.

**3. Actores:**
- Usuario

**4. Flujo Básico:**
1. **Usuario** selecciona "Registrar" en la pantalla principal.
2. **Sistema** muestra un formulario de registro.
3. **Usuario** completa el formulario con su nombre, correo electrónico y contraseña.
4. **Usuario** envía el formulario.
5. **Sistema** guarda la información y confirma el registro al usuario.

**5. Postcondiciones:**
- El usuario tiene una cuenta creada y puede iniciar sesión.

**6. Flujos Alternativos:**
- Si la información es incorrecta o el correo ya está registrado, el sistema muestra un mensaje de error y solicita corrección.

---

### Mi Cuenta

#### Ver y Editar Información de la Cuenta

**1. Título del Caso de Uso:**
Ver y Editar Información de la Cuenta

**2. Descripción:**
Permite a un usuario ver y editar la información de su cuenta.

**3. Actores:**
- Usuario

**4. Flujo Básico:**
1. **Usuario** selecciona "Mi Cuenta" en el menú principal.
2. **Sistema** muestra la información de la cuenta del usuario.
3. **Usuario** edita la información de su cuenta (nombre, correo electrónico, teléfono, dirección).
4. **Usuario** guarda los cambios.
5. **Sistema** actualiza la información en la base de datos y confirma la actualización.

**5. Postcondiciones:**
- La información de la cuenta del usuario está actualizada.

**6. Flujos Alternativos:**
- Si la información es incorrecta, el sistema muestra un mensaje de error y solicita corrección.

---

#### Reiniciar Contraseña

**1. Título del Caso de Uso:**
Reiniciar Contraseña

**2. Descripción:**
Permite a un usuario recuperar su contraseña en caso de haberla olvidado.

**3. Actores:**
- Usuario

**4. Flujo Básico:**
1. **Usuario** selecciona "Olvidé mi contraseña" en la pantalla de inicio de sesión.
2. **Sistema** solicita al usuario que ingrese su correo electrónico.
3. **Usuario** ingresa su correo electrónico y envía la solicitud.
4. **Sistema** envía un enlace de restablecimiento de contraseña al correo electrónico del usuario.
5. **Usuario** abre el correo y selecciona el enlace de restablecimiento.
6. **Sistema** muestra un formulario para ingresar una nueva contraseña.
7. **Usuario** ingresa y confirma la nueva contraseña.
8. **Sistema** actualiza la contraseña en la base de datos y confirma el restablecimiento al usuario.

**5. Postcondiciones:**
- El usuario puede iniciar sesión con su nueva contraseña.

**6. Flujos Alternativos:**
- Si el correo electrónico no está registrado, el sistema muestra un mensaje de error.

---

#### Ver Mi Estado de Cuenta

**1. Título del Caso de Uso:**
Ver Mi Estado de Cuenta

**2. Descripción:**
Permite a un usuario ver su estado de cuenta con detalles de transacciones y saldos.

**3. Actores:**
- Usuario

**4. Flujo Básico:**
1. **Usuario** selecciona "Mi Estado de Cuenta" en el menú principal.
2. **Sistema** muestra el estado de cuenta del usuario con transacciones recientes y saldo actual.

**5. Postcondiciones:**
- El usuario ve su estado de cuenta actualizado.

**6. Flujos Alternativos:**
- Si hay un error al recuperar los datos, el sistema muestra un mensaje de error.

---

#### Ver Mis Paquetes

**1. Título del Caso de Uso:**
Ver Mis Paquetes

**2. Descripción:**
Permite a un usuario ver el estado y detalles de sus paquetes enviados desde Estados Unidos a Panamá.

**3. Actores:**
- Usuario

**4. Flujo Básico:**
1. **Usuario** selecciona "Mis Paquetes" en el menú principal.
2. **Sistema** muestra una lista de paquetes asociados con el usuario, incluyendo detalles de seguimiento y estado actual.

**5. Postcondiciones:**
- El usuario ve los detalles y estado de sus paquetes.

**6. Flujos Alternativos:**
- Si hay un error al recuperar los datos, el sistema muestra un mensaje de error.

---

### Paquetería

#### Manejo de Guías

##### Ingresar Guía

**1. Título del Caso de Uso:**
Ingresar Guía

**2. Descripción:**
Permite a la franquicia ingresar una nueva guía en el sistema.

**3. Actores:**
- Usuario (Franquicia)

**4. Flujo Básico:**
1. **Usuario (Franquicia)** selecciona "Ingresar Guía" en el menú de paquetería.
2. **Sistema** muestra un formulario para ingresar detalles de la guía.
3. **Usuario** completa el formulario con la información requerida y envía el formulario.
4. **Sistema** guarda la información de la guía y confirma la creación al usuario.

**5. Postcondiciones:**
- La nueva guía está registrada en el sistema.

**6. Flujos Alternativos:**
- Si la información es incorrecta, el sistema muestra un mensaje de error y solicita corrección.

---

##### Editar Guía

**1. Título del Caso de Uso:**
Editar Guía

**2. Descripción:**
Permite a la franquicia editar una guía existente en el sistema.

**3. Actores:**
- Usuario (Franquicia)

**4. Flujo Básico:**
1. **Usuario (Franquicia)** selecciona "Editar Guía" y elige la guía a modificar.
2. **Sistema** muestra la información actual de la guía.
3. **Usuario** realiza los cambios necesarios y guarda las modificaciones.
4. **Sistema** actualiza la información de la guía y confirma los cambios al usuario.

**5. Postcondiciones:**
- La guía está actualizada en el sistema.

**6. Flujos Alternativos:**
- Si la información es incorrecta, el sistema muestra un mensaje de error y solicita corrección.

---

##### Borrar Guía

**1. Título del Caso de Uso:**
Borrar Guía

**2. Descripción:**
Permite a la franquicia borrar una guía del sistema.

**3. Actores:**
- Usuario (Franquicia)

**4. Flujo Básico:**
1. **Usuario (Franquicia)** selecciona "Borrar Guía" y elige la guía a eliminar.
2. **Sistema** solicita confirmación de la acción.
3. **Usuario** confirma la eliminación.
4. **Sistema** borra la guía y confirma la eliminación al usuario.

**5. Postcondiciones:**
- La guía ha sido eliminada del sistema.

**6. Flujos Alternativos:**
- Si hay un error, el sistema muestra un mensaje de error y solicita confirmación.

---

#### Manejo de Paquetes

##### Ingresar Paquete

**1. Título del Caso de Uso:**
Ingresar Paquete

**2. Descripción:**
Permite a un usuario ingresar un nuevo paquete en el sistema.

**3. Actores:**
- Usuario

**4. Flujo Básico:**
1. **Usuario** selecciona "Ingresar Paquete" en el menú de paquetería.
2. **Sistema** muestra un formulario para ingresar detalles del paquete.
3. **Usuario** completa el formulario con la información requerida y envía el formulario.
4. **Sistema** guarda la información del paquete y confirma la creación al usuario.

**5. Postcondiciones:**
- El nuevo paquete está registrado en el sistema.

**6. Flujos Alternativos:**
- Si la información es incorrecta, el sistema muestra un mensaje de error y solicita corrección.

---

##### Editar Paquete

**1. Título del Caso de Uso:**
Editar Paquete

**2. Descripción:**
Permite a un usuario editar un paquete existente en el sistema.

**3. Actores:**
- Usuario

**4. Flujo Básico:**
1. **Usuario** selecciona "Editar Paquete" y elige el paquete a modificar.
2. **Sistema** muestra la información actual del paquete.
3. **Usuario** realiza los cambios necesarios y guarda las modificaciones.
4. **Sistema** actualiza la información del paquete y confirma los cambios al usuario.

**5. Postcondiciones:**
- El paquete está actualizado en el sistema.

**6. Flujos Alternativos:**
- Si la información es incorrecta, el sistema muestra un mensaje de error y solicita corrección.

---

##### Borrar Paquete

**1. Título del Caso de Uso:**
Borrar Paquete

**2. Descripción:**
Permite a un usuario borrar un paquete del sistema.

**3. Actores:**
- Usuario

**4. Flujo Básico:**
1. **Usuario** selecciona "Borrar Paquete" y elige el paquete a eliminar.
2. **Sistema** verifica que el paquete no haya sido facturado.
3. **Sistema** solicita confirmación de la acción.
4. **Usuario** confirma la eliminación.
5. **Sistema** borra el paquete y confirma la eliminación al usuario.

**5. Postcondiciones:**
- El paquete ha sido eliminado del sistema.

**6. Flujos Alternativos:**
- Si hay un error o el paquete ha sido facturado, el sistema muestra un mensaje de error y solicita confirmación.

---

### Manejo de Cuentas

#### Clientes Finales

##### Crear Usuario

**1. Título del Caso de Uso:**
Crear Usuario (Clientes Finales)

**2. Descripción:**
Permite a la franquicia crear un nuevo usuario cliente final en el sistema.

**3. Actores:**
- Usuario (Franquicia)

**4. Flujo Básico:**
1. **Usuario (Franquicia)** selecciona "Crear Usuario" en el menú de cuentas.
2. **Sistema** muestra un formulario para ingresar detalles del nuevo cliente.
3. **Usuario** completa el formulario y envía la solicitud.
4. **Sistema** guarda la información del cliente y confirma la creación al usuario.

**5. Postcondiciones:**
- El nuevo cliente está registrado en el sistema.

**6. Flujos Alternativos:**
- Si la información es incorrecta, el sistema muestra un mensaje de error y solicita corrección.

---

##### Editar Información

**1. Título del Caso de Uso:**
Editar Información (Clientes Finales)

**2. Descripción:**
Permite a la franquicia editar la información de un cliente final en el sistema.

**3. Actores:**
- Usuario (Franquicia)

**4. Flujo Básico:**
1. **Usuario (Franquicia)** selecciona "Editar Información" y elige el cliente a modificar.
2. **Sistema** muestra la información actual del cliente.
3. **Usuario** realiza los cambios necesarios y guarda las modificaciones.
4. **Sistema** actualiza la información del cliente y confirma los cambios al usuario.

**5. Postcondiciones:**
- La información del cliente está actualizada en el sistema.

**6. Flujos Alternativos:**
- Si la información es incorrecta, el sistema muestra un mensaje de error y solicita corrección.

---

##### Bloquear/Desbloquear

**1. Título del Caso de Uso:**
Bloquear/Desbloquear (Clientes Finales)

**2. Descripción:**
Permite a la franquicia bloquear o desbloquear la cuenta de un cliente final en el sistema.

**3. Actores:**
- Usuario (Franquicia)

**4. Flujo Básico:**
1. **Usuario (Franquicia)** selecciona "Bloquear/Desbloquear" y elige el cliente a modificar.
2. **Sistema** muestra el estado actual de la cuenta del cliente.
3. **Usuario** cambia el estado de la cuenta (bloquear o desbloquear).
4. **Sistema** actualiza el estado de la cuenta y confirma el cambio al usuario.

**5. Postcondiciones:**
- La cuenta del cliente está bloqueada o desbloqueada según la acción realizada.

**6. Flujos Alternativos:**
- Si hay un error, el sistema muestra un mensaje de error y solicita confirmación.

---

##### Resetear Contraseña

**1. Título del Caso de Uso:**
Resetear Contraseña (Clientes Finales)

**2. Descripción:**
Permite a la franquicia restablecer la contraseña de un cliente final en el sistema.

**3. Actores:**
- Usuario (Franquicia)

**4. Flujo Básico:**
1. **Usuario (Franquicia)** selecciona "Resetear Contraseña" y elige el cliente a modificar.
2. **Sistema** envía un enlace de restablecimiento de contraseña al correo electrónico del cliente.
3. **Cliente** abre el correo y selecciona el enlace de restablecimiento.
4. **Sistema** muestra un formulario para ingresar una nueva contraseña.
5. **Cliente** ingresa y confirma la nueva contraseña.
6. **Sistema** actualiza la contraseña en la base de datos y confirma el restablecimiento al cliente.

**5. Postcondiciones:**
- La contraseña del cliente está actualizada en el sistema.

**6. Flujos Alternativos:**
- Si hay un error, el sistema muestra un mensaje de error y solicita confirmación.

---

#### Revendedores

##### Crear Usuario

**1. Título del Caso de Uso:**
Crear Usuario (Revendedores)

**2. Descripción:**
Permite a la franquicia crear un nuevo usuario revendedor en el sistema.

**3. Actores:**
- Usuario (Franquicia)

**4. Flujo Básico:**
1. **Usuario (Franquicia)** selecciona "Crear Usuario" en el menú de cuentas.
2. **Sistema** muestra un formulario para ingresar detalles del nuevo revendedor.
3. **Usuario** completa el formulario y envía la solicitud.
4. **Sistema** guarda la información del revendedor y confirma la creación al usuario.

**5. Postcondiciones:**
- El nuevo revendedor está registrado en el sistema.

**6. Flujos Alternativos:**
- Si la información es incorrecta, el sistema muestra un mensaje de error y solicita corrección.

---

##### Editar Información

**1. Título del Caso de Uso:**
Editar Información (Revendedores)

**2. Descripción:**
Permite a la franquicia editar la información de un revendedor en el sistema.

**3. Actores:**
- Usuario (Franquicia)

**4. Flujo Básico:**
1. **Usuario (Franquicia)** selecciona "Editar Información" y elige el revendedor a modificar.
2. **Sistema** muestra la información actual del revendedor.
3. **Usuario** realiza los cambios necesarios y guarda las modificaciones.
4. **Sistema** actualiza la información del revendedor y confirma los cambios al usuario.

**5. Postcondiciones:**
- La información del revendedor está actualizada en el sistema.

**6. Flujos Alternativos:**
- Si la información es incorrecta, el sistema muestra un mensaje de error y solicita corrección.

---

##### Bloquear/Desbloquear

**1. Título del Caso de Uso:**
Bloquear/Desbloquear (Revendedores)

**2. Descripción:**
Permite a la franquicia bloquear o desbloquear la cuenta de un revendedor en el sistema.

**3. Actores:**
- Usuario (Franquicia)

**4. Flujo Básico:**
1. **Usuario (Franquicia)** selecciona "Bloquear/Desbloquear" y elige el revendedor a modificar.
2. **Sistema** muestra el estado actual de la cuenta del revendedor.
3. **Usuario** cambia el estado de la cuenta (bloquear o desbloquear).
4. **Sistema** actualiza el estado de la cuenta y confirma el cambio al usuario.

**5. Postcondiciones:**
- La cuenta del revendedor está bloqueada o desbloqueada según la acción realizada.

**6. Flujos Alternativos:**
- Si hay un error, el sistema muestra un mensaje de error y solicita confirmación.

---

##### Resetear Contraseña

**1. Título del Caso de Uso:**
Resetear Contraseña (Revendedores)

**2. Descripción:**
Permite a la franquicia restablecer la contraseña de un revendedor en el sistema.

**3. Actores:**
- Usuario (Franquicia)

**4. Flujo Básico:**
1. **Usuario (Franquicia)** selecciona "Resetear Contraseña" y elige el revendedor a modificar.
2. **Sistema** envía un enlace de restablecimiento de contraseña al correo electrónico del revendedor.
3. **Revendedor** abre el correo y selecciona el enlace de restablecimiento.
4. **Sistema** muestra un formulario para ingresar una nueva contraseña.
5. **Revendedor** ingresa y confirma la nueva contraseña.
6. **Sistema** actualiza la contraseña en la base de datos y confirma el restablecimiento al revendedor.

**5. Postcondiciones:**
- La contraseña del revendedor está actualizada en el sistema.

**6. Flujos Alternativos:**
- Si hay un error, el sistema muestra un mensaje de error y solicita confirmación.

---

##### Editar Roles

**1. Título del Caso de Uso:**
Editar Roles

**2. Descripción:**
Permite a la franquicia editar los roles de un revendedor en el sistema.

**3. Actores:**
- Usuario (Franquicia)

**4. Flujo Básico:**
1. **Usuario (Franquicia)** selecciona "Editar Roles" y elige el revendedor a modificar.
2. **Sistema** muestra los roles actuales del revendedor.
3. **Usuario** realiza los cambios necesarios en los roles y guarda las modificaciones.
4. **Sistema** actualiza los roles del revendedor y confirma los cambios al usuario.

**5. Postcondiciones:**
- Los roles del revendedor están actualizados en el sistema.

**6. Flujos Alternativos:**
- Si hay un error, el sistema muestra un mensaje de error y solicita confirmación.

---

### Cuentas por Cobrar

#### Facturación

##### Generar Factura

**1. Título del Caso de Uso:**
Generar Factura

**2. Descripción:**
Permite a la franquicia generar una nueva factura para un cliente final y un revendedor.

**3. Actores:**
- Usuario (Franquicia)

**4. Flujo Básico:**
1. **Usuario** selecciona "Generar Factura" en el menú de cuentas por cobrar.
2. **Sistema** muestra un formulario para ingresar detalles de la factura.
3. **Usuario** completa el formulario con la información requerida, selecciona paquetes a facturar y agrega otros servicios si es necesario.
4. **Usuario** guarda la factura.
5. **Sistema** guarda la información de la factura y confirma la creación al usuario.

**5. Postcondiciones:**
- La nueva factura está registrada en el sistema y se han generado dos facturas, una para el revendedor y otra para el cliente final.

**6. Flujos Alternativos:**
- Si la información es incorrecta, el sistema muestra un mensaje de error y solicita corrección.

---

##### Editar Factura

**1. Título del Caso de Uso:**
Editar Factura

**2. Descripción:**
Permite editar una factura existente en el sistema.

**3. Actores:**
- Usuario (Franquicia)

**4. Flujo Básico:**
1. **Usuario** selecciona "Editar Factura" y elige la factura a modificar.
2. **Sistema** muestra la información actual de la factura.
3. **Usuario** realiza los cambios necesarios y guarda las modificaciones.
4. **Sistema** actualiza la información de la factura y confirma los cambios al usuario.

**5. Postcondiciones:**
- La factura está actualizada en el sistema.

**6. Flujos Alternativos:**
- Si la factura tiene pagos asociados, no se puede editar y el sistema muestra un mensaje de error.
- Si la información es incorrecta, el sistema muestra un mensaje de error y solicita corrección.

---

##### Borrar Factura

**1. Título del Caso de Uso:**
Borrar Factura

**2. Descripción:**
Permite borrar una factura del sistema.

**3. Actores:**
- Usuario (Franquicia)

**4. Flujo Básico:**
1. **Usuario** selecciona "Borrar Factura" y elige la factura a eliminar.
2. **Sistema** verifica que la factura no tenga pagos asociados.
3. **Sistema** solicita confirmación de la acción.
4. **Usuario** confirma la eliminación.
5. **Sistema** borra la factura y confirma la eliminación al usuario.

**5. Postcondiciones:**
- La factura ha sido eliminada del sistema.

**6. Flujos Alternativos:**
- Si la factura tiene pagos asociados, no se puede borrar y el sistema muestra un mensaje de error.
- Si hay un error, el sistema muestra un mensaje de error y solicita confirmación.

---

##### Otros Servicios

**1. Título del Caso de Uso:**
Otros Servicios

**2. Descripción:**
Permite agregar servicios adicionales (e.g., delivery) a una factura existente.

**3. Actores:**
- Usuario (Franquicia)

**4. Flujo Básico:**
1. **Usuario** selecciona "Otros Servicios" en el menú de facturación.
2. **Sistema** muestra un formulario para ingresar detalles del servicio adicional.
3. **Usuario** completa el formulario con la información requerida y guarda el servicio.
4. **Sistema** agrega el servicio a la factura existente y confirma la actualización al usuario.

**5. Postcondiciones:**
- El servicio adicional está registrado en la factura y los valores de la factura han sido actualizados.

**6. Flujos Alternativos:**
- Si la información es incorrecta, el sistema muestra un mensaje de error y solicita corrección.

---

#### Notas de Crédito

##### Crear Nota de Crédito

**1. Título del Caso de Uso:**
Crear Nota de Crédito

**2. Descripción:**
Permite crear una nueva nota de crédito en el sistema.

**3. Actores:**
- Usuario (Franquicia)

**4. Flujo Básico:**
1. **Usuario** selecciona "Crear Nota de Crédito" en el menú de cuentas por cobrar.
2. **Sistema** muestra un formulario para ingresar detalles de la nota de crédito.
3. **Usuario** completa el formulario con la información requerida y selecciona la factura a la que se aplicará o ingresa un monto libre.
4. **Usuario** guarda la nota de crédito.
5. **Sistema** guarda la información de la nota de crédito y confirma la creación al usuario.

**5. Postcondiciones:**
- La nueva nota de crédito está registrada en el sistema.

**6. Flujos Alternativos:**
- Si la información es incorrecta, el sistema muestra un mensaje de error y solicita corrección.

---

##### Editar Nota de Crédito

**1. Título del Caso de Uso:**
Editar Nota de Crédito

**2. Descripción:**
Permite editar una nota de crédito existente en el sistema.

**3. Actores:**
- Usuario (Franquicia)

**4. Flujo Básico:**
1. **Usuario** selecciona "Editar Nota de Crédito" y elige la nota de crédito a modificar.
2. **Sistema** muestra la información actual de la nota de crédito.
3. **Usuario** realiza los cambios necesarios y guarda las modificaciones.
4. **Sistema** actualiza la información de la nota de crédito y confirma los cambios al usuario.

**5. Postcondiciones:**
- La nota de crédito está actualizada en el sistema.

**6. Flujos Alternativos:**
- Si la información es incorrecta, el sistema muestra un mensaje de error y solicita corrección.

---

##### Borrar Nota de Crédito

**1. Título del Caso de Uso:**
Borrar Nota de Crédito

**2. Descripción:**
Permite borrar una nota de crédito del sistema.

**3. Actores:**
- Usuario (Franquicia)

**4. Flujo Básico:**
1. **Usuario** selecciona "Borrar Nota de Crédito" y elige la nota de crédito a eliminar.
2. **Sistema** solicita confirmación de la acción.
3. **Usuario** confirma la eliminación.
4. **Sistema** borra la nota de crédito y confirma la eliminación al usuario.

**5. Postcondiciones:**
- La nota de crédito ha sido eliminada del sistema.

**6. Flujos Alternativos:**
- Si hay un error, el sistema muestra un mensaje de error y solicita confirmación.

---

#### Pagos

##### Registrar Pago

**1. Título del Caso de Uso:**
Registrar Pago

**2. Descripción:**
Permite registrar un nuevo pago en el sistema.

**3. Actores:**
- Usuario (Franquicia)
- Usuario (Revendedor)

**4. Flujo Básico:**
1. **Usuario** selecciona "Registrar Pago" en el menú de cuentas por cobrar.
2. **Sistema** muestra un formulario para ingresar detalles del pago.
3. **Usuario** completa el formulario con la información requerida y guarda el pago.
4. **Sistema** guarda la información del pago y confirma la creación al usuario.

**5. Postcondiciones:**
- El nuevo pago está registrado en el sistema.

**6. Flujos Alternativos:**
- Si la información es incorrecta, el sistema muestra un mensaje de error y solicita corrección.

---

##### Editar Pago

**1. Título del Caso de Uso:**
Editar Pago

**2. Descripción:**
Permite editar un pago existente en el sistema.

**3. Actores:**
- Usuario (Franquicia)
- Usuario (Revendedor)

**4. Flujo Básico:**
1. **Usuario** selecciona "Editar Pago" y elige el pago a modificar.
2. **Sistema** muestra la información actual del pago.
3. **Usuario** realiza los cambios necesarios y guarda las modificaciones.
4. **Sistema** actualiza la información del pago y confirma los cambios al usuario.

**5. Postcondiciones:**
- El pago está actualizado en el sistema.

**6. Flujos Alternativos:**
- Si la información es incorrecta, el sistema muestra un mensaje de error y solicita corrección.

---

##### Cancelar Pago

**1. Título del Caso de Uso:**
Cancelar Pago

**2. Descripción:**
Permite cancelar un pago existente en el sistema.

**3. Actores:**
- Usuario (Franquicia)
- Usuario (Revendedor)

**4. Flujo Básico:**
1. **Usuario** selecciona "Cancelar Pago" y elige el pago a cancelar.
2. **Sistema** solicita confirmación de la acción.
3. **Usuario** confirma la cancelación.
4. **Sistema** revierte el pago y actualiza la información en el sistema, confirmando la cancelación al usuario.

**5. Postcondiciones:**
- El pago ha sido cancelado en el sistema.

**6. Flujos Alternativos:**
- Si hay un error, el sistema muestra un mensaje de error y solicita confirmación.

---

#### Tarifas

##### Establecer Tarifas

**1. Título del Caso de Uso:**
Establecer Tarifas

**2. Descripción:**
Permite a la franquicia y a los revendedores establecer tarifas para sus clientes.

**3. Actores:**
- Usuario (Franquicia)
- Usuario (Revendedor)

**4. Flujo Básico:**
1. **Usuario (Franquicia o Revendedor)** selecciona "Establecer Tarifas" en el menú de cuentas por cobrar.
2. **Sistema** muestra un formulario para ingresar detalles de las tarifas.
3. **Usuario** completa el formulario con la información requerida y guarda las tarifas.
4. **Sistema** guarda la información de las tarifas y confirma la creación al usuario.

**5. Postcondiciones:**
- Las nuevas tarifas están registradas en el sistema.

**6. Flujos Alternativos:**
- Si la información es incorrecta, el sistema muestra un mensaje de error y solicita corrección.
