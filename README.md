# Intermodular-Nubes
# Fundamentos de Computación en la Nube (MPO / CMO)

# 1. Elección de proveedor Cloud

He elegido **Amazon Web Services (AWS)** porque es uno de los proveedores cloud más utilizados a nivel mundial. Cuenta con una gran cantidad de documentación, herramientas y servicios, además de disponer de un nivel gratuito (*Free Tier*) ideal para pequeñas empresas y proyectos iniciales.

AWS ofrece varias ventajas importantes para la empresa:

- Permite escalar fácilmente si la tienda aumenta sus clientes online.
- Dispone de servicios gestionados que reducen el mantenimiento.
- Ofrece alta disponibilidad para evitar pérdidas de datos.
- Incluye sistemas de seguridad integrados.
- Tiene una infraestructura muy estable y utilizada por grandes empresas.

Por estas razones, AWS es una opción adecuada para el proyecto de la empresa.



# 2. Arquitectura cloud propuesta

La empresa contará con una aplicación web donde los clientes podrán:
- Realizar pedidos.
- Consultar productos.
- Dejar opiniones.

Los empleados gestionarán la plataforma desde los ordenadores de la tienda mediante acceso a internet.

La aplicación web y la base de datos estarán alojadas en la nube, permitiendo el acceso desde navegadores web.

## Esquema de funcionamiento

```text
Usuarios → Servidor Web → Base de Datos
(Clientes y empleados) → (AWS EC2) → (AWS RDS)
```

## Flujo de funcionamiento

1. El usuario accede a la página web desde su navegador.
2. La petición llega al servidor web.
3. El servidor procesa la información.
4. Se consulta la base de datos para obtener productos, pedidos y datos necesarios.
5. El servidor devuelve la información al usuario.



# 3. Servicios cloud utilizados

## 1. Elastic Compute Cloud (EC2)

Servicio utilizado para:
- Ejecutar la aplicación web.
- Actuar como servidor virtual en la nube.

Es el equivalente a un ordenador o servidor físico alojado en AWS.



## 2. Relational Database Service (RDS)

Servicio utilizado para:
- Gestionar la base de datos de la empresa.
- Guardar productos, clientes, pedidos y otra información.

AWS se encargará automáticamente de:
- Copias de seguridad.
- Mantenimiento.
- Disponibilidad.



## 3. Simple Storage Service (S3)

Servicio utilizado para:
- Almacenar archivos multimedia.
- Guardar imágenes y vídeos de productos.



## 4. Identity and Access Management (IAM)

Servicio utilizado para:
- Gestionar usuarios y permisos.
- Controlar el acceso a los recursos cloud.
- Mejorar la seguridad de la infraestructura.



# 4. Estimación de costes

## Recursos utilizados

La infraestructura cloud contará con:
- Una instancia EC2 para el servidor web.
- Una base de datos básica en RDS.
- Almacenamiento S3 para archivos multimedia.



## Coste mensual aproximado

| Servicio | Coste aproximado |
|---|---|
| AWS EC2 | 8 - 10 € |
| AWS RDS | 10 - 15 € |
| AWS S3 | 1 - 3 € |

### Coste total estimado
El coste mensual aproximado será de:

```text
20 - 30 € al mes
```



## Uso del Free Tier de AWS

Se utilizará el nivel gratuito de AWS (*Free Tier*), que ofrece durante 12 meses:

- 750 horas mensuales de EC2.
- Uso limitado de RDS.
- Capacidad básica de almacenamiento en S3.

Esto permitirá reducir costes durante los primeros meses de funcionamiento de la empresa, cuando todavía contará con menos recursos económicos.
