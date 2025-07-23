# Seguridad

- de infreaestructura

Shared security model

## 1. On-premises

- datos
- dispositivos
- cuentas de acceso
- aplicaciones
- redes
- sistemas operativos
- virtualización
- red fisica
- servidores
- datacenters

## 2. OCI

- datos
- dispositivos
- cuentas de acceso
- aplicaciones
- redes
- sistemas operativos
- virtualización
- red fisica
- servidores
- datacenters

![1752976875287](image/3Seguridad/1752976875287.png)

## Zonas de seguridad

![1752977377950](image/3Seguridad/1752977377950.png)

## Cloud Guard

- servicio que verifica la seguridad de los recursos de OCI

![1752977731142](image/3Seguridad/1752977731142.png)

![1752977890439](image/3Seguridad/1752977890439.png)

## Security Xones y security advisor

- advisor: servicio en la nube que unifica las zonas de seguridad y otras capacidades de la nube.
- zones: se refiere al compartimiento en el cual no puedes deshabilitar la seguridad.

## Encryption o encriptacion cifrado

- Es una capa de seguridad
- proceso inverso de desifrado

![1753301307541](image/3Seguridad/1753301307541.png)

- **rest** cuando estan guardados
- **in transit**: cuando los datos viajan de un servidor a otro, se proteje el paquete en la transmision.

![1753301371362](image/3Seguridad/1753301371362.png)

## Tipos de Cifrados

### Simetrico

- se usa una unica llave para cifrar y descifrar
- seguridad baja
- la llave se envia en el mensaje

![1753301455992](image/3Seguridad/1753301455992.png)


### Asimetrico

- se usan diferentes llaves para cifrar y descifrar
- llave publica viaja en el mensaje
- llave privada se tiene en un lugar seguro, no se debe compartir

![1753301573223](image/3Seguridad/1753301573223.png)

## Modelos de cifrado Algoritmos

### AES advanced encryptatio standard

- la misma llave cifra y descifra
- no pueden ser usados para firma digital

### RSA rivest shamir adleman

- una llave cifra y otra llave descifra
- se puede usar para firma digital

### ECDSA elliptic curve digital signature algorithm

- solo se puede usar en firmas digitales
- no se usa para cifrar o descifrar

## HSM Hardware security module

- es un servicio de modulos de seguridad de hardware dedicado
- oci vault utiliza hsm
- cumple estandar FIPS 140-2, nivel de seguridad 3
- resistente a la manipulacion
- requiere autenticacion basada en la identidad
- elimina las claves del dispositivo cuando detecta manipulacion

# Vault

- baul de datos seguros
- manejo centralizado de llaves y credenciales
- puede ser por software
- puede ser por hardware HSM
- pueden existir varios vaults, cada vault tendrá su llave maestra o master key
- todo se puede auditar

![1753302310690](image/3Seguridad/1753302310690.png)

![1753302476359](image/3Seguridad/1753302476359.png)

### Envelope encryption

- una llave maestra puede envolver una llave data key

![1753302788573](image/3Seguridad/1753302788573.png)
