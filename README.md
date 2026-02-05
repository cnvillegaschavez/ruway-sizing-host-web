# Aplicativo Tallas SAMITEX - Especificación Funcional

## 1. Objetivo

El presente desarrollo debe ser un diseño web responsivo, que permite el acceso a usuarios para registrar tallaje y ventas.

## 2. Estructura General

### 2.1. Respecto a los usuarios

- El módulo podrá ser accedido por cualquier usuario al que se le otorgue permiso.
- Se desarrollará en modo web, por lo tanto, podrá acceder desde cualquier dispositivo (laptop, pc, celular, Tablet, etc.), garantizando capacidad responsiva.

## 3. Módulo de Inicio de Sesión

### 3.1. Autenticación de usuario

- El sistema debe generar un usuario único y una contraseña inicial para cada usuario registrado.
- El sistema debe permitir que el usuario autorizado ingrese mediante credenciales de acceso (usuario y contraseña).
- La contraseña debe almacenarse en la base de datos de manera encriptada
- El sistema debe validar las credenciales y mostrar mensajes claros en caso de error (usuario no encontrado, contraseña incorrecta, usuario inactivo).

### 3.2. Cierre de sesión

- El sistema debe permitir al usuario cerrar sesión de forma segura.

## 4. Olvidé mi Contraseña 

Recuperación de contraseña 

El sistema debe ofrecer una opción “Olvidé mi contraseña” en la pantalla de inicio de sesión. 

Al seleccionar esta opción, el usuario ingresará su correo electrónico registrado. 

El sistema enviará un enlace seguro de recuperación de contraseña al correo ingresado. 

 

Restablecimiento de contraseña 

El enlace debe llevar a una pantalla para ingresar la nueva contraseña. 

La nueva contraseña debe cumplir con políticas mínimas de seguridad (ejemplo: mínimo 8 caracteres, una mayúscula, un número y un carácter especial). 

El sistema debe invalidar el enlace de recuperación después de un tiempo configurable (ejemplo: 15 minutos).

## 5. Módulo de gestión de usuario del sistema 

El sistema debe permitir registrar, modificar y eliminar los usuarios con los siguientes datos mínimos: 

Nombre completo 

Correo electrónico (único) 

Documento de identidad (DNI, CE.) 

Empresa asociada al usuario 

Código de empleado 

Perfil  

Validar que el correo electrónico y el documento no estén duplicados. 

Enviar correo de bienvenida con credenciales iniciales (usuario y contraseña temporal). 

Roles y permisos 

El sistema debe restringir el acceso de acuerdo con el perfil de usuario: 

Carga Masiva de Usuarios 

Importación desde archivo Excel 

El sistema debe permitir importar usuarios en bloque mediante un archivo Excel. 

El archivo debe tener un formato predefinido con las siguientes columnas mínimas: 

Nombre completo 

Correo electrónico 

Documento de identidad 

El sistema debe validar: 

Estructura del archivo (formato correcto). 

Que los correos y documentos no estén repetidos. 

Que los usuarios cargados tengan empresa asociada válida. 

Campos obligatorios no vacíos. 

Resumen de carga 

El sistema debe mostrar un reporte al finalizar la carga: 

Total de registros procesados. 

Registros exitosos. 

Registros con error y descripción del motivo (correo duplicado, empresa inexistente, formato inválido, etc.). 

Generación de credenciales 

El sistema debe generar automáticamente credenciales para cada usuario cargado correctamente. 

Las credenciales iniciales deben enviarse al correo electrónico del usuario.

## 6. Módulo de registro de perfil (cargo del personal) 

 

El sistema debe permitir registrar, modificar y eliminar los perfiles. 

El sistema debe almacenar una lista de cargos predefinidos, entre ellos: 

Gerente General 

Gerente de Planta 

Jefatura de Calidad 

Auditor de Calidad 

Jefe de Desarrollo de Producto 

Desarrolladores de Producto 

Almaceneros de Tela 

Jefe de Planeamiento 

Administrador de Ventas 

Vendedores 

Supervisor de Sastres 

Sastres 

Digitadores 

Modelistas

## 7. Módulo de gestión del personal 

El sistema debe permitir registrar, modificar y eliminar los siguientes datos de cada personal: 

1. Tipo de Documento de Indentidad 

2. Numero de Doc. de Identidad 

3. Nombres del personal 

4. Apellidos del personal 

5. Correo corporativo 

6. Celular 

7. Perfil 

El sistema debe validar si el perfil es sastre, el sistema debe habilitar la siguiente informarcion: 

Es Interno o Externo: 

Si el sastre es externo, el sistema bloquea el registro de SCTR 

Si el sastre es interno, el sistema debe de activar SCRT y su Vigencia del SCTR 

El sistema debe validar que el DNI y el correo corporativo no se repitan para más de un personal. 

Carga Masiva de personal 

Importación desde archivo Excel 

El sistema debe permitir importar personal en bloque mediante un archivo Excel. 

El archivo debe tener un formato predefinido. 

El sistema debe validar los campos minimos. 

Estructura del archivo (formato correcto). 

Que los correos y documentos no estén repetidos. 

Campos obligatorios no vacíos. 

Resumen de carga 

El sistema debe mostrar un reporte al finalizar la carga: 

Total de registros procesados. 

Registros exitosos. 

Registros con error y descripción del motivo (correo duplicado, formato inválido, etc.).

## 8. Módulo de asignación de accesos por perfil de cargo 

El sistema debe permitir asignar a cada perfil de cargo los módulos del sistema a los que tendrá acceso. 

El sistema debe permitir configurar accesos a nivel de: 

Visualización 

Registro 

Modificación 

Eliminación 

 El sistema debe permitir revocar accesos a cualquier cargo cuando sea necesario. 

El sistema debe garantizar que los colaboradores hereden automáticamente los accesos definidos en su cargo. 

El sistema debe permitir la reasignación de accesos cuando un colaborador cambie de cargo.

## 9. Módulo de registro de parámetros de medidas corporales 

El sistema debe permitir registrar, editar y eliminar parámetros de medidas corporales. 

El sistema debe permitir definir un código único para cada parámetro de medida. 

El sistema debe permitir ingresar medidas corporales como: 

Talle De Espalda 

Largo Total 

Ancho De Espalda 1 

Ancho De Espalda 2 

Ancho De Pecho (Mitad) 

Ancho De Cintura (Mitad) 

Ancho De Cadera (Mitad) 

Hombro 

Largo De Manga 

Ancho De Brazo (Mitad) 

Alto De Sisa 

Talle De Delantero 

Largo Delantero 

Amplitud De Pecho 

Alto De Busto 

Separación De Busto 

Mitad De Busto 

Largo Total C/Pretina 

Largo De Entrepierna 

Ancho Cintura (Mitad) 

Ancho Cadera (Mitad) 

Ancho De Muslo (Mitad) 

Ancho De Rodilla (Mitad) 

Ancho Botapie (Mitad) 

Tiro Delantero C/Pretina 

Tiro De Fundillo C/Pretina 

Tiro En "U" 

Prolong. Tiro Fundillo 

 

El sistema debe permitir definir un rango válido de valores (límite inferior y límite superior) para cada medida. 

El sistema debe permitir la consulta de parámetros de medidas previamente registrados para reutilización en productos.

## 10. Módulo de registro de talla 

 

El sistema debe permitir registrar, editar y eliminar la talla. 

El sistema debe permitir definir: 

Código de talla único. 

Nombre de talla

## 11. Módulo registro de tipo de producto 

 

El sistema debe permitir registrar, editar y eliminar tipos de producto. 

El sistema debe permitir definir: 

Código de producto único. 

Nombre del producto: Saco, Camisa, Blusa, Pantalon, Terno, etc. 

Tallas: XXS-XS-S-M-L-XL-XXL-XXXL-XXXXL 

Medidas de tallas: Medida corporal 

Rango de tallas: Límite Inferior - Límite superior (cm.) 

El sistema debe permitir asociar cada producto con las tallas correspondientes (ejemplo: XXS–XS–S–M–L–XL–XXL–XXXL). 

El sistema debe permitir asociar un producto con los parámetros de medidas corporales previamente registrados. 

El sistema debe permitir establecer los rangos de tallas (mínimo y máximo) para cada tipo de producto.

## 12. Módulo de registro de tipo de negocio 

 

El sistema debe permitir registrar, editar y eliminar tipos de negocio. 

El sistema debe permitir seleccionar entre diferentes tipos de negocio predefinidos, como: 

 

A medida 

Tallaje 

Autotallaje

## 13. Módulo de registro de tipo de proceso 

El sistema debe permitir registrar, editar y eliminar tipos de proceso. 

El sistema debe permitir seleccionar entre diferentes tipos de proceso predefinidos, como: 

Licitación Pública 

Adjudicación Simplificada 

Subasta Electrónica 

Consumo Privado, etc.

## 14. Módulo de registro de tipos de medida de producto 

El sistema debe permitir registrar, editar y eliminar tipos de medida de producto. 

El sistema debe permitir seleccionar entre diferentes tipos de medida de producto predefinidos, como: 

Samitex 

Cliente

## 15. Módulo de registro de Packing 

El sistema debe permitir registrar, editar y eliminar packing de producto. 

El sistema debe permiter seleccionar los productos y cantidad para el packing. 

Ejemplos: 

Packing 1: Camisa-pantalon-saco 

Packing 2: Camisa-pantalon-casaca  

Packing 3: Pantalon- 2 polos

## 16. Módulo Registro de la venta en el aplicativo 

Este módulo permitirá registrar la venta de mercadería. 

 

El sistema debe permitir registrar o actualizar un cliente, para esto el sistema debe permitir el ingreso del RUC para determinar si existe o no el cliente. 

Si el cliente es nuevo: 

El sistema debe abrir una ventana para el registro del cliente con los siguientes datos: 

Código de Cliente 

Nombre completo/Razón Social 

RUC 

Domicilio fiscal 

Tipo de cliente:  

Público 

Privado 

Representante del cliente: 

Nombre 

Correo 

Celular 

Cargo 

Área usuaria: 

Nombre 

Correo 

Celular 

Cargo 

Área Logística: 

Nombre 

Correo 

Celular 

Cargo 

Sucursales:  

Dirección. 

Si el cliente no es nuevo: 

El sistema debe de mostrar la información del cliente. 

El usuario podrá actualizar la información en los campos autorizados de los datos en 6.1.1 (según perfil de usuario). 

Validaciones: 

El RUC debe cumplir con la estructura válida según SUNAT (11 dígitos). 

El sistema debe validar que no existan duplicados de RUC en la base de datos. 

Los campos de correo deben ser validados con formato estándar usuario@dominio.com 

Los números de celular deben validarse en base a cantidad de dígitos. 

Cada cliente debe tener un código único. 

El sistema debe permitir marcar un cliente como Activo/Inactivo para efectos de uso en ventas. 

 

El sistema debe permitir el registro de una nueva venta. 

Pantalla de creación de la nueva venta se debe de tener las siguientes consideraciones: 

Tipo de Proceso: Lista desplegable- Licitación, adjudicación, subasta, etc. (Debe contemplar un mantenimiento) 

Tipo de Negocio: Lista desplegable (Tallaje, auto tallaje, a medida). (contemplar un mantenimiento) 

Requerimiento de SCTR para sastres 

Fecha de firma de contrato: dd/mm/yyyy (Obligatorio) 

Definir tipo de medidas de producto: Lista desplegable (contemplar un mantenimiento) 

Samitex (Existe definida) 

Cliente 

Se deben clasificar las medidas según los puntos a y b. 

Creación de Packing: Selección de lista desplegable de tipo y cantidad por producto. (Ejm. Packing 1: Camisa-pantalón-saco / Packing 2: Camisa-pantalón-casaca / Packing 3: Pantalón- 2 polos) (contemplar un mantenimiento) 

Cantidad por packing: Es la cantidad de packings a producir (Ejm. 300 packing 1 / 200 Packing 2 / 600 Packing 3). El sistema me expresa la cantidad por producto a producir. 

(Ejm. Pantalones = 300 packing 1 + 200 Packing 2 + 600 Packing 3 = 1100 pantalones) 

(Ejm. Camisa = 300 packing 1 + 200 Packing 2 = 500 camisas) 

(Ejm. Polo = 1200 packing 3 = 1200 polos) 

Cantidad para producir: 1100 pantalones, 500 camisas, 1200 polos. - Esta información es necesaria para que el sistema no permita fabricar más cantidad de lo estipulado en el contrato sin una aprobación previa que debe incluir una adenda sujeta al contrato. 

La sumatoria de packings debe ser automático 

Registrar los límites de tolerancia permitidos a las medidas por prenda para el control de calidad. (cargar de forma masiva). 

Firma de cuadro de medidas corporales: En el sistema se debe colocar ambas opciones a seleccionar de acuerdo con las bases del contrato. 

Firma Física: Requiere impresión del cuadro de la toma de medidas corporales para obtener la firma física del usuario. 

Firma Virtual: Se genera un PIN al usuario registrado para validar la toma de medidas corporales en el sistema. 

Instrucciones de embalaje:  

EJ: porta terno, bolsas individuales, empaque de transporte (caja corrugada, colgado, etc.) (Contemplar mantenimiento para las instrucciones) 

 Selección tipo de negocio: 

A medida: Participa un sastre. 

Si existe requerimiento de muestra: 

El administrador de venta debe de ingresar al sistema las medidas del producto para muestra. 

No existe requerimiento de muestra: 

El sistema debe de continuar con el proceso 

Tallaje: No participa el sastre.  

Tipo tallaje Samitex:   

El sistema utiliza la información de las medidas estándares de las tallas. 

Tipo tallaje cliente:  

El administrador de ventas debe de seleccionar en el sistema el tipo de producto e ingresar las medidas de las bases en los campos relacionados al tipo de producto. 

 

 Auto tallaje: El usuario se toma las medidas corporales. 

Tipo auto tallaje Samitex: 

El sistema asigna la talla con las medidas corporales precargadas en la tabla. 

Tipo auto tallaje Cliente:  

El sistema debe permitir ingresar las medidas de las bases en los campos desplegados relacionados al tipo de producto y el sistema asigna la talla con las medidas cargadas del cliente. 

Proceso final: Creación del código de la venta. 

El sistema debe crear un código único de venta con la siguiente estructura:  

Tipo de proceso: (del 1 al 9) (un dígito) (contemplar mantenimiento) 

Licitación Pública - 1 

Adjudicación Simplificada - 2 

Concurso Privado - 3 

Subasta Electrónica - 4 

ETC (llega hasta N° 9).  

Tipo de negocio: (1-9) (un dígito) 

A medida 

Tallaje 

Auto tallaje  

Registro de fecha 

La fecha debe considerar a partir de la firma de contrato 

Dia: (dos dígitos) 

01, 10, 15, 20, etc.   

Mes: (dos dígitos) 

Mayo (05) 

Noviembre (11) 

Año: (dos dígitos) 

25, 26, 27, etc. 

 

Correlativo del mes de firma de contrato: (dos dígitos- del 1 hasta el 99). - Indica los contratos firmados dentro del mes. (código de cliente 4 dígitos Alfanumérico) 

Ejemplo de código:  1116042501.- Licitación pública, uniforme a medida del día 16 del mes de abril del año 2025, negocio N° 1 

Licitación pública 

uniforme a medida 

 día 

 mes 

 año 

 correlativo por mes 

1 

1 

16 

04 

25 

001 

  

 

 

 

## 17. Módulo recibe información detallada del cliente

 

El módulo debe permitir registrar y administrar la información de los usuarios a quienes se les realizará la vestimenta. 

El registro podrá realizarse de dos formas: mediante un formulario web o mediante la carga de un archivo Excel. 

 

Registro de usuarios 

Registro a través de Formulario: 

DNI / CE / Código de Usuario (Identificador único) 

Nombres y Apellidos 

Celular (obligatorio, requerido para envío de mensajes de texto) 

Correo electrónico (obligatorio, requerido para envío de correos) 

Cargo 

Uniforme / Packing Asignados 

Sucursal 

Usuario del Sistema (DNI / CE/ Código de Usuario) 

Clave de acceso: 

El sistema debe permitir que el usuario ingrese su código identificador. 

El sistema debe enviar un enlace y un token al correo electrónico registrado para generar su contraseña. 

Recuperación de clave: 

El sistema debe permitir recuperar la contraseña mediante la opción “Olvidé mi contraseña”. 

El sistema debe enviar un enlace de recuperación vía correo electrónico y/o SMS. 

PIN (Firma Virtual): 

El sistema debe generar automáticamente un PIN de 3 dígitos aleatorios al completar el registro. 

El sistema debe enviarlo por SMS y correo electrónico. 

Recuperación de PIN: 

El sistema debe validar los datos ingresados por el usuario. 

En caso de ser correctos, se genera y envía un nuevo PIN. 

Validación de Packing: 

El sistema debe validar el packing asignado al usuario contra lo definido en el punto 6.2.1.7 del proceso. 

 

Registro a través de Archivo Excel 

El sistema debe proporcionar un enlace para descargar una plantilla de Excel con el formato definido para carga masiva. 

El sistema debe permitir subir el archivo Excel con la información de los usuarios. 

El sistema debe validar el contenido del archivo antes de registrar los usuarios. 

 

Validaciones del sistema para el registro de usuarios: 

 El sistema valida Validar que todos los campos obligatorios sean completados, tanto en el formulario como en el archivo Excel. 

Validar la cantidad de usuarios registrados en comparación con lo estipulado en el contrato: 

Si la cantidad es menor a la del contrato: 

El sistema debe permitir eliminar usuarios registrados que no participarán en el proceso de vestimenta. 

El sistema debe permitir registrar tallas genéricas (S, M, L, etc.) en caso de que el cliente desee la entrega de tallas estándar. 

Si la cantidad es mayor a la del contrato: 

El sistema debe permitir sustituir usuarios, eliminando a aquellos que no participarán y registrando a los nuevos usuarios. 

 El sistema, para adicionar usuarios, debe informar que se realizará una adenda al contrato, permitiendo mantener a todos los usuarios registrados para la toma de datos. 

Si el sistema no recibe el documento de la Adenda, la adición de usuarios queda bloqueada. 

Historial de cambios: 

El sistema debe guardar un historial que permita ver todos los movimientos realizados en el registro de usuarios.

## 18. Módulo informa la asignación de los sastres 

Este módulo tiene como finalidad gestionar la asignación de sastres para el proceso de medición de tallas corporales. 

Si el negocio exige SCTR para los sastres, debe de registrarse la fecha de vigencia del SCTR de cada sastre. (Cambio en el punto 44. Registro de la venta en el aplicativo – Nota del cuadro 10 – Anotación (2.1)) 

El sistema debe validar si fue solicitado con SCTR 

Asignación de sastres con SCTR: Asigna sastres internos 

Asignación de sastres sin SCTR: Asigna sastres internos o externos 

El sistema debe validar si el sastre solicitado cuenta o no con SCTR. 

El sistema debe permitir la asignación de sastres para las sesiones de medición corporal de acuerdo con las bases del contrato. 

El sistema debe habilitar la aprobación de los sastres seleccionados. 

El sistema debe enviar la notificación de asignación al área comercial mediante correo electrónico.

## 19. Módulo registro de la ficha de medidas para cada beneficiario 

Este módulo tiene como finalidad registrar la toma de medidas personalizadas para cada usuario. 

 

Verificación e ingreso del usuario 

El sistema debe permitir ingresar el código identificador del usuario (DNI/CE) para verificar que el usuario se encuentre registrado 

Si el usuario no está registrado: 

 

Registrar el usuario a traves del formulario “Registro de usuario. 

 

Si el usuario si está registrado: 

 

El sastre ingresa el DNI del usuario para proceder con la toma de medidas. 

El sistema muestra los campos de medidas corporales correspondientes a los productos asignados en el Packing. 

Ejemplo: Si se asignó una camisa, se mostrarán campos como cuello, pecho, brazo, etc. 

El sistema permite el ingreso de las medidas corporales del usuario. 

El sistema alerta al sastre si alguna medida está fuera del rango esperado, solicitando su corrección o ratificación. 

El sistema debe comparar las medidas tomadas por el sastre con las medidas establecidas en el sistema previamente registrados.  

El sistema permite confirmar las medidas registradas por el sastre. 

 

Validación de medidas por el usuario 

Registro de validación física: 

 

El sastre ingresa el PIN del usuario (4 dígitos) en el campo de firma virtual. 

El sistema agrupa y guarda las medidas en la matriz(tabla) de tallas del usuario. 

Ejemplo de formato: 

 

Producto/Medidas 

Pecho 

Cintura 

Cuello 

Largo de manga 

Saco 

xx cm. 

zz cm. 

0 cm. 

ww cm. 

Camisa 

xx cm. 

zz cm. 

yy cm. 

ww cm. 

 

El sistema permite imprimir una hoja con las medidas del usuario. 

(Formato de medidas de usuario – Jeruth debe de facilitarlo) 

 

Registro de validación virtual 

 

El usuario ingresa su PIN en el campo de firma virtual. 

El sistema debe indicar la aprobación por parte del usuario. 

 

El sistema agrupa las medidas en la matriz correspondiente. 

Ejemplo de formato: 

 

Producto/Medidas 

Pecho 

Cintura 

Cuello 

Largo de manga 

Saco 

xx cm. 

zz cm. 

0 cm. 

ww cm. 

Camisa 

xx cm. 

zz cm. 

yy cm. 

ww cm. 

 

 Campos para medir según el Packing asignado: 
Ejemplo: 

Packing 1: Saco y Camisa 

Medidas corporales: 

Pecho – Saco y Camisa 

Cintura – Saco y Camisa 

Cuello – Camisa 

Largo de Manga – Saco y Camisa 

Cadera – Saco y Camisa 

 

El sistema debe permitir consultar el reporte de tallas y medidas registradas por beneficiario, con el fin de enviar la información a producción hasta el número máximo de beneficiarios permitidos según lo establecido en el contrato 

 El sistema debe permitir registrar beneficiarios adicionales aun cuando se supere la cantidad permitida en el contrato; sin embargo, dichos beneficiarios no estarán habilitados para el proceso de producción hasta que se realice la adenda correspondiente o el reemplazo de beneficiarios, conforme a las indicaciones del cliente. 

Reporte de usuarios sin registro de medidas (Definir formato de Reporte) 

El sistema debe permitir al digitador generar un reporte con los usuarios que no han completado su toma de medidas corporales. 

 

Envío de reportes a administración (definir formato de correo) 

El sistema debe permitir al digitador generar y enviar dicho reporte al Administrador de Ventas vía correo electrónico.

## 20. Módulo control de calidad de producto terminado 

Este módulo permite realizar la verificación de la calidad de las prendas terminadas. 

 

 Ingreso de prenda al sistema 

El auditor de calidad podrá registrar una prenda en el sistema utilizando uno de los siguientes métodos: 

Ingreso manual del código de la prenda. 

Selección desde una lista en el sistema. 

Escaneo del código de barras de la prenda. 

Formato del código de barras: 
Contiene la concatenación del Número de DNI del usuario + Código del producto. 

 

Visualización de Medidas de Referencia 

Al ingresar o escanear la prenda, el sistema debe mostrar automáticamente los campos de las medidas correspondientes a ese producto terminado. 

 Registro de medidas por el auditor de calidad 

El auditor podrá ingresar directamente en el sistema las medidas reales tomadas de la prenda.  

El sistema debe almacenar: 

Medidas registradas. 

Nombre del auditor. 

Fecha y hora de revisión. 

Número de revisión. 

 

Historial de Revisiones 

El sistema debe mantener un historial por cada prenda, incluyendo: 

Cantidad de revisiones. 

Identidad de los auditores involucrados. 

Fecha y hora de cada inspección. 

Resultado de cada revisión. 

 

Comparación de Medidas 

El sistema realizará una comparación automática entre: 

Las medidas registradas para la prenda del usuario. 

Las medidas ingresadas por el auditor. 

Según el resultado, el sistema notificará: 

Aprobado, si todas las medidas están dentro de tolerancia y agrupar las prendas asignadas por el usuario. 

Desaprobado, si alguna medida excede los límites de tolerancia permitidos. 

 

Agrupación de Prendas 

El sistema debe mostrar un listado agrupado de prendas: 

Por usuario asignado. 

Por estado (pendiente, revisada, aprobada, desaprobada) 

 

 Solicitud de Corrección de Datos 

El sistema debe permitir que el auditor solicite una corrección de datos en caso de error al ingresar medidas. 

La solicitud será enviada al Jefe de Calidad, incluyendo: 

1. Nombre del auditor solicitante. 

2. Tipo de producto. 
3. Tipo de negocio. 

4. Campos de medidas a corregir. 

El jefe de calidad podrá aprobar o rechazar la solicitud desde el sistema. 

Una vez aprobada, el sistema permitirá editar únicamente los campos autorizados al auditor. 

 

Reprocesos 

El sistema debe permitir marcar una prenda como reproceso cuando sea necesario. Esta información debe reflejarse en el historial y en los reportes. 

 

Aprobación por Gerencia General 

El Gerente General podrá: 

Aprobar o rechazar el envío final de prendas que hayan sido previamente desaprobadas por el sistema y por la desprobación del reproceso por parte del gerente de planta. 

Cada decisión debe quedar registrada en el historial del sistema. 

 Reportes Generales 

El sistema debe generar reportes sobre: 

Fallas detectadas en medidas. 

Historial de revisiones por prenda o por auditor.

Prendas reprocesadas.

## 21. Funcionalidades del módulo proceso de distribución  

Este módulo gestiona la entrega de mercadería al cliente, ya sea a nivel institucional o directamente al usuario final. Permite emitir reportes, realizar validaciones, gestionar inconformidades y registrar la conformidad del pedido. 

 

Emisión de Reportes de Entrega 

Reporte por Sucursal, Packing y Usuario 

El Adm. De Ventas podrá generar un reporte agrupado por: 

Sucursal (oficina) 

Packing (lote o grupo de entrega) 

Usuarios dentro de cada packing 

 

Filtros del Reporte 

El sistema permitirá aplicar los siguientes filtros: 

Rango de fecha 

Cliente 

Sucursal 

 

Nota: La información deberá paginarse en bloques de 30 registros por página. 

 

Envío y validación de entrega  

Opción 1: Entrega a la institución 

Envío de Packing por Sucursal 

El sistema permitirá ejecutar el envío de un packing por sucursal. 

Automáticamente se enviará un correo electrónico al responsable del área logística del cliente con la información: 

Notificación del envío en camino de la mercadería 

PIN de validación de recepción 

 

Validación de Entrega 

El sistema permitira la validación de entrega y conformidad de la mercadería por Email o PIN 

 

Validación por Email 

Si el cliente indica que el pedido está conforme: 

El administrador de ventas registra la conformidad en el sistema. 

 

Si el pedido no es conforme, se presentan dos escenarios: 

Sobrante de mercadería: 

El sistema debe de permitir generar una orden de recojo. 

El sistema envía un correo al cliente con la orden de recojo. 

Luego de confirmar el recojo, el administrador de ventas registra la conformidad en el sistema. 

 

Sobrante y/o faltante de mercadería: 

El administrador revisa en el sistema si los faltantes estan en la lista de usuarios por sucursal. 

Si el usuario no existe:  

No procede el reclamo. 

El administrador de ventas envia por correo que el reclamo no procede 

El administrador de venta procede a dar la conformidad del pedido en el sistema 

Si el usuario existe:  

Permitir Mostrar la lista de usuarios por sucursal, permitiendo su verificación. 

Permitir eliminar usuarios faltantes y agregar nuevos usuarios a la lista de una sucursal. 

Permitir el cambio de usuarios entre sucursales, previa aprobación de gerencia. 

Registrar nuevos usuarios en la sucursal ingresando el DNI, con autollenado automático de datos. 

Permitir la modificación de datos de usuario. 

Validar que la cantidad de prendas sobrantes sea igual a la cantidad de prendas faltantes. 

Para prendas sobrantes: 

Permitir generar una orden de recojo. 

Enviar automáticamente un correo al operador logístico del cliente. 

Para prendas faltantes: 

Si existe stock disponible: iniciar el proceso de distribución y entrega. 

Si no existe stock: iniciar automáticamente el proceso de corte. 

 

Validación por PIN 

Si el pedido es conforme: 

El operador logístico del cliente ingresa el PIN como firma virtual en el sistema. 

Si el pedido no es conforme: 

El operador logístico del cliente registra sobrantes y/o faltantes en el sistema. 

 

Solo sobrante:  

El sistema permitira registrar los usuarios sobrantes 

El sistema debe permitir al administrador de ventas generar la orden de devolución. 

Luego de confirmar el recojo, el administrador de ventas registra la conformidad en el sistema. 

 

Sobrante y/o faltante: 

Validar que no coincidan cantidades. 

Generar PIN de inconformidad y enviarlo. 

Responsable de área de logística registra cambios. 
 

Opción 2: Entrega al usuario cliente 

 

El sistema envía WhatsApp y correo con el PIN al usuario cliente. 

El operador logístico ingresa el PIN para registrar conformidad que es otorgado por el usuario. 

 

El Administrador de ventas genera en el sistema reporte de conformidad del cliente. 

El reporte debe mostrar todos los pedidos sean conformes o inconformes.  (Formato de reporte Jeruth debe facilitarlo) 

Filtros del reporte  

El sistema debe permitir mostrar el reporte según los criterios: 

 

Rango de fecha 

Cliente 

Sucursal 

Estado de pedido (Conforme e Inconforme)

Se implementará paginación de 30 registros por página.

## 22. Programa una visita de ajuste de prenda 

 

Este módulo permite gestionar visitas de ajuste, registrar inconformidades y realizar una nueva toma de medidas por parte del usuario o del sastre. 

 

 A medida 

El sistema debe permitir al administrador programar una visita de ajuste de prenda en una sucursal específica, previa coordinación con el cliente. 

El sistema debe permitir generar cronograma. 

El sistema debe permitir seleccionar el viaje y asignación de sastre a la sucursal. 

 

El sistema debe permitir al sastre registrar nuevas medidas corporales del usuario durante la visita. 

El sistema debe generar y permitir completar un formato digital de ajuste de prendas. 

El sistema debe permitir obtener la firma del usuario como validación del formato de ajuste. (Opcional: se debe definir si será firma virtual o física escaneada.) 

El sistema debe permitir generar una copia del formato de ajuste de prenda y entregarla (impresa o digital) al usuario. 

El sistema debe continuar el flujo con el módulo de procesamiento de ajustes de prenda tras el registro de la visita. 

 

 Tallaje – Autotallaje 

El sistema debe permitir al usuario registrar inconformidades con una prenda previamente entregada. 

El sistema debe permitir al área usuaria generar y compartir un enlace único para que el usuario acceda a registrar las inconformidades. 

El sistema debe mostrar al usuario las prendas asociadas a su packing (paquete de entrega) asignado. 

El sistema debe solicitar la toma de nuevas medidas al usuario y habilitar un formulario para ingresarlas. 

El sistema debe comparar automáticamente las nuevas medidas ingresadas con las medidas anteriores del usuario. 

Si las nuevas medidas son similares a las anteriores, el sistema debe seleccionar si desea una talla más pequeña o grande 

Si no existe similitud, el sistema debe sugerir una nueva talla basada en las nuevas medidas proporcionadas. 

El sistema debe generar un reporte con las nuevas medidas e inconformidades registradas, y enviarlo automáticamente al administrador de ventas.

## 23. Realización agrupación y clasificación de tallas 

 

Este proceso se genera una vez se haya realizado el registro de medidas corporales de cada usuario.  

 

El sistema debe validar que todas las medidas corporales necesarias para la generación de las prendas, en base al packing asignado al usuario, estén registradas, en caso de faltar alguna medida obligatoria, el sistema debe impedir la generación de tallas y emitir un mensaje de alerta especificando la medida faltante. 

El sistema debe validar que las medidas corporales registradas esten dentro del rango permitido, En caso de que alguna medida esté fuera de rango, el sistema debe marcarla como “fuera de rango” y emitir un mensaje de alerta especificando la(s) medida(s) corporal(es) que esta fuera del rango. 

El sistema debe permitir generar y mostrar las tallas de las prendas del packing asignada al usuario una vez se haya finalizado la toma corporal y se encuentre validado. 

El sistema deberá aplicar reglas específicas de cálculo, clasificación y validación, asegurando la correcta asignación de tallas, en base al tipo de negocio: 

 

Tipo de negocio a medida 

El sistema debe consolidar todas las medidas corporales previamente registradas y organizarlas en una matriz(Tabla) de medidas asociada a cada beneficiario, ubicar cada medida en la posición que le corresponde de la matriz (fila = producto, columna = medida), según lo requerido en el pedido. 

Producto/Medidas 

Pecho 

Cintura 

Cuello 

Largo de manga 

Saco 

xx cm. 

zz cm. 

0 cm. 

ww cm. 

Camisa 

xx cm. 

zz cm. 

yy cm. 

ww cm. 

 

El sistema debe validar completitud mínima por prenda 

Ejmplo: 

Packing 1: Saco y Camisa 

Medidas corporales: 

Pecho: Saco y Camisa. 

Cintura: Saco y Camisa. 

Cuello: Camisa. 

Largo de manga: Saco y Camisa. 

Cadera: Saco y Camisa. 

 

El sistema asigna la talla de acuerdo a la medida corporal principal de la prenda, por cada prenda el sistema lee la medida corporal principal del producto busca en la tabla la talla que corresponde a ese rango y asigna esa talla al producto.   

Ejemplo de medidas corporales por prenda. 

 

Ejemplos de asignación de la talla de acuerdo con la medida corporal principal definida por tipo de prenda 

Top Hombre: Pecho / Cuello (camisa). 

Top Mujer: Busto. 

Bottom Hombre: Cintura. 

Bottom Mujer: Cadera. 

 

El sistema clasifica los usuarios de tipo normal o especial 

Usuario normal: medidas dentro de la tolerancia de la talla estándar (±1). 

Usuario especial: medidas fuera de la tolerancia (>±2 en alguna medida clave). 

 

Es normal:  

El sistema debe identificar todas las prendas cuyas medidas corporales se encuentran dentro del rango definido con la tolerancia (±1) para una talla y agruparlas automáticamente bajo esa talla. 

 

Es especial:  

El sistema detecta que las medidas estan fuera de la tolerancia (>±2) 

 

Si existen parametros agrupables 

 

Su identificacón de compartir los mismos parametros se va a basar en: 

 

Si las medidas corporales ajenas a la medida principal esta fuera del rango de la talla seleccionada (mayor que +/- 2) se agruparán los campos de acuerdo con la jerarquía de medidas 

  

Jerarquia de Medidas: TOP - HOMBRE/MUJER (SACO, CAMISA, SACON, ABRIGO, CASACA, CHALECO, PULLOVER, CHOMPA, BLUSA, BLAZER) 

Definicion de talla: Pecho(H) - Cuello (Camisa H) - Busto (M todas las prendas) 

1. Largo Total. 

2. Largo de Manga. 

3. Cintura. 

4. Espalda Ancho. 

5. Cadera 

6. Contorno de Brazo. 

  

Jerarquia de Medidas: BOTTOM - HOMBRE (Pantalon) 

Definicion de talla: Cintura 

1. Largo Total. 

2. Cadera 

3. Talle Delantero 

4. Talle Fundillo 

5. Ancho de Muslo. 

6. Ancho de Rodilla. 

7. Ancho de Bota pie 

  

Jerarquia de Medidas: BOTTOM - MUJER (Pantalon - Falda) 

Definicion de talla: Cadera 

1. Largo Total. 

2. Cintura 

3. Talle Delantero 

4. Talle Fundillo 

5. Ancho de Muslo. 

6. Ancho de Rodilla. 

7. Ancho de Bota pie 

 

El sistema debe identificar y agrupar automáticamente a los usuarios que comparten los mismos parametros en una o varias prendas, una vez finalizada la toma corporal de cada usuario. 

 

No existen parametros agrupables 

 

 

El sistema debe identificar cuando una talla de prenda es única, es decir, cuando las medidas corporales del usuario no se ajustan a ninguna de las tallas estándar definidas 

Tipo de negocio tallaje o autotallaje 

Tipo de producto: Camisa 

El sistema debe validar que exista el valor de la medida cuello registrada para el usuario. 

El sistema debe comparar el valor de cuello contra la tabla de tallas estándar de camisas. 

 

Por ejemplo: Se registra la medida del cuello (15 pulgadas) de contorno: 

Valor del contorno: 15 pulgadas 

Resultado: La camisa estará en la talla 15 

 

El sistema debe asignar automáticamente la talla de camisa correspondiente según el rango encontrado. 

En caso de que la medida de cuello no se encuentre en ningún rango, el sistema debe marcar el caso como “fuera de rango”. 

 

Tipo de producto: Prendas bottom (Pantalón – Hombre y Mujer, Faldas – Mujer) 

Hombre (Pantalón) 

 

El sistema debe validar que exista el valor de la medida de cintura y cadera para el usuario. 

El sistema debe identificar la talla correspondiente de cintura y cadera según la tabla estándar. 

 

Si la talla de la cadera ≤ talla de la cintura, el sistema debe asignar la talla de acuerdo con la cintura. 

Ejemplo: 

 

Talla N° 

34 

36 

Talla 

L 

XL 

Cintura 

93-97 

98-102 

Cadera 

105-109 

110-114 

   

Datos: 

Medida de la cintura = 94 / Talla 34 

Medida de la cadera = 108 / Talla 34 

 

Sistema detecta que la medida de la cintura y cadera esta dentro del rango de la talla 34, talla resultante = 34  

 

Si la talla de la cadera > talla de la cintura, se valida la condición: 

Si la medida de la cadera < límite máximo de la talla anterior de la cadera + 2, el sistema mantiene la talla de acuerdo con la cintura. 

 

Si la medida de la cadera ≥ límite máximo de la talla anterior de la cadera + 2, el sistema asigna la talla de acuerdo con la cadera. 

 

Ejemplos:  

 

Talla N° 

34 - L 

36 - XL 

Medidas Corporales - Ej.1 

Talla resultante por campo - Ej. 1 

Medidas Corporales - Ej. 2 

Talla resultante por campo - Ej. 2 

Cintura 

93-97 

98-102 

94 

34 

94 

34 

Cadera 

105-109 

110-114 

110 

36 

111 

36 

   

Ejemplo 1:  

 

Medida de la cintura = 94 / Talla 34. 

Medida de la cadera = 110 / Talla 36. 

 

Sistema detecta que la medida de la cintura esta dentro del rango de la talla 34. 

Sistema detecta que la medida de la cadera esta dentro del rango de la talla 36. 

 

Logica: Si la medida de la cadera es mayor o igual que el limite maximo de la talla menor de la cadera +2 

Limite maximo de la talla menor = 109 

Medida de cadera = 110 

  

110 ≥ 109 + 2 

110 ≥ 111 (Falso) 

  

Resultado: Entonces La talla resultante que corresponde es la talla de la cintura (Talla 34) 

  

Ejemplo 2:  

Medida de la cintura = 94 / Talla 34. 

Medida de la cadera = 111 / Talla 36. 

  

Sistema detecta que la medida de la cintura esta dentro del rango de la talla 34. 

Sistema detecta que la medida de la cadera esta dentro del rango de la talla 36. 

 

Logica: Si la medida de la cadera es mayor o igual que el limite maximo de la talla menor de la cadera +2 

Limite maximo de la talla menor = 109 

Medida de cadera del usuario = 111 

  

111 ≥ 109 + 2 

111 ≥ 111 (Verdadero) 

  

Resultado: Entonces La talla resultante que corresponde es la talla de la cadera (Talla 36) 

  

Mujer (Pantalón y Falda) 

 

El sistema debe validar que exista el valor de la medida de cadera y cintura para el usuario. 

El sistema debe identificar la talla correspondiente de cadera y cintura según la tabla estándar, el sistema toma como referencia la talla de la cadera (Mujer) 

 

Si la talla de la cintura ≤ talla de la cadera, el sistema debe asignar la talla de acuerdo con la cadera. 

Ejemplo 

 Talla N° 

34 

36 

Talla 

L 

XL 

Cadera 

102 - 105 

106 - 109 

Cintura 

81 - 84 

85 - 90 

 

Medidas corporales del cliente Y:  

Cadera: 104 

Cintura: 83 

 

Resultado de tallas según datos de entrada: 

Medida de la cadera = 104 / Talla 34 

Medida de la cintura = 83 / Talla 34 

  

Sistema detecta que la medida de la cintura y cadera esta dentro del rango de la talla 34, entonces talla resultante = 34 

 

Si la talla de la cintura > talla de la cadera, se valida la condición: 

Si la medida de la cintura ≥ límite máximo de la talla menor + 2, el sistema asigna la talla de la cintura. 

Si la medida de la cintura < límite máximo de la talla menor + 2, el sistema mantiene la talla de la cadera. 

Ejemplo 

Talla N° 

34 - L 

36 - XL 

Medidas Corporales - Ej.1 

Talla resultante por campo - Ej. 1 

Medidas Corporales - Ej. 2 

Talla resultante por campo - Ej. 2 

Cadera 

102 - 105 

106 - 109 

104 

34 

104 

34 

Cintura 

81 - 84 

85 - 90 

85 

36 

86 

36 

  

Limite mínimo ≤ L ≤Limite Máximo  

  

Ejemplo 1:  

Medida de la cadera = 104 / Talla 34. 

Medida de la cintura = 85 / Talla 36. 

  

Sistema detecta que la medida de la cadera esta dentro del rango de la talla 34. 

Sistema detecta que la medida de la cintura esta dentro del rango de la talla 36. 

  

Logica: Si la medida de la cintura es mayor o igual que el limite maximo de la talla menor de la cintura +2 

Limite maximo de la talla menor de la cintura = 84 

Medida de cintura del usuario = 86 

  

85 ≥ 84 + 2 

85 ≥ 86 (Falso) 

  

Resultado: Entonces La talla resultante que corresponde es la talla de la cadera (Talla 34) 

  

Ejemplo 2:  

Medida de la cadera = 104 / Talla 34. 

Medida de la cintura = 86/ Talla 36 

  

Sistema detecta que la medida de la cintura esta dentro del rango de la talla 34. 

Sistema detecta que la medida de la cadera esta dentro del rango de la talla 36. 

 

Logica: Si la medida de la cintura es mayor o igual que El limite maximo de la talla menor de la cintura +2 

Limite maximo de la talla menor = 84 

Medida de cadera = 86 

 

86 ≥ 84 + 2 

86 ≥ 86 (verdadero) 

  

Resultado: Entonces La talla resultante que corresponde es la talla de la cintura (Talla 36) 

 

El sistema debe marcar el caso como “fuera de rango” si ninguna medida encaja en las tablas definidas. 

Prendas Top (Sacos, Abrigos, Casacas, Chalecos, Pullover) 

El sistema debe validar que exista el valor de la medida pecho/busto y cintura. 

El sistema debe identificar la talla correspondiente de pecho/busto y cintura según la tabla estándar, el sistema toma como medida referencial el Pecho 

 

Si la talla de la cintura ≤ talla de pecho/busto, el sistema asigna la talla de acuerdo con el pecho/busto. 

Ejemplo 

 

Talla N° 

36 

38 

Talla 

S 

M 

Pecho 

95-99 

100-104 

Cintura 

83-87 

88-92 

  

Medidas corporales del cliente Y:  

Pecho: 97 

Cintura: 85 

  

Tallas resultantes 

Medida del Pecho = 97 / Talla 36 

Medida de la cintura = 85 / Talla 36 

  

Sistema detecta que la medida de la cintura y pecho/busto esta dentro del rango de la talla 36, talla resultante = 36 

  

Si la talla de la cintura > talla de pecho/busto, se valida la condición: 

Si la medida de la cintura < límite máximo de la talla menor + 2, el sistema mantiene la talla del pecho/busto. 

Si la medida de la cintura ≥ límite máximo de la talla anterior + 2, el sistema asigna la talla de la cintura. 

 

Ejemplos 

 

Talla N° 

36- S 

38 - M 

Medidas Corporales - Ej.1 

Talla resultante por campo - Ej. 1 

Medidas Corporales - Ej. 2 

Talla resultante por campo - Ej. 2 

Pecho 

95-99 

100-104 

98 

36 

98 

34 

Cintura 

83-87 

88-92 

90 

38 

88 

36 

  

Limite mínimo ≤ L ≤Limite Máximo  

  

Ejemplo 1:  

Medida del pecho = 98 / Talla 36. 

Medida de la cintura = 90 / Talla 38. 

  

Sistema detecta que la medida del pecho esta dentro del rango de la talla 36. 

Sistema detecta que la medida de la cintura esta dentro del rango de la talla 38. 

  

Logica: Si la medida de la cintura es mayor o igual que el limite maximo de la talla menor de la cintura +2 

Limite maximo de la talla menor de la cintura = 87 

Medida de cintura del usuario = 90 

  

90 ≥ 87 + 2 

90 ≥ 89 (Verdadero) 

  

Resultado: Entonces La talla resultante que corresponde es la talla de la cintura (Talla 38) 

  

Ejemplo 2:  

Medida del pecho = 98 / Talla 36. 

Medida de la cintura = 88 / Talla 38. 

  

Sistema detecta que la medida del pecho esta dentro del rango de la talla 36. 

Sistema detecta que la medida de la cintura esta dentro del rango de la talla 38. 

  

Logica: Si la medida de la cintura es mayor o igual que El limite maximo de la talla menor de la cintura +2 

Limite maximo de la talla menor de la cintura = 87 

Medida de cintura del usuario = 88 

  

88 ≥ 87 + 2 

88 ≥ 89 (Falso) 

  

Resultado: Entonces La talla resultante que corresponde es la talla del pecho (Talla 36) 

 

El sistema debe permitir agrupar y listar las tallas registradas por prenda y por usuario para el proceso de producción, clasificándolas según el tipo de usuario (Normal, Especial) y considerando las tallas únicas u otras categorías definidas por el sistema. (formato de reporte, Jertuh debe facilitar) 

 