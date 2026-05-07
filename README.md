## Taller practico 03 Laboratorio Ecosistema Odoo

Para la realización de esta actividad utilizamos **Odoo y Docker.**

*Antes de comenzar con la actividad instalaremos algunas extensiones de Odoo para que podamos realizar todo correctamente como **invoicing** (facturación) o **inventory** (inventario).*

Para comenzar la práctica creamos un archivo .csv con una pequeña base de datos con clientes *(archivo clientes\_mock.csv)* y la importamos ese registro y comprobaremos que todo funcione correctamente.

<img width="720" height="287" alt="image" src="https://github.com/user-attachments/assets/0d0767e0-836f-414e-8781-a83611a9c5a2" />

Ahora entraremos en el usuario comercial (creado anteriormente) y crearemos un producto (iphone 17 en mi caso). (No creamos un servicio ya que Odoo no genera una orden de entrega por no ocupar espacio físico como tal).

<img width="482" height="101" alt="image" src="https://github.com/user-attachments/assets/22bca49f-94fe-49b4-afef-e8a890eda621" />

Una vez que el producto haya sido creado crearemos una factura *(documento Pedido \- S00002.pdf)* del cliente que ha comprado el producto.

<img width="952" height="53" alt="image" src="https://github.com/user-attachments/assets/0ba0c948-da40-4eef-86fb-b1df25e6d60c" />

Después modificamos la parte de informes para que aparezca más presentable entrando en una vista específica (sale.report\_saleorder\_document.) que renderiza el HTML que luego el motor wkhtmltopdf convierte a un archivo PDF.

Al final de dicha vista insertamos un código **HTML/XML** *(código de marcas)*  que es lo que modificará el informe.

<img width="951" height="364" alt="image" src="https://github.com/user-attachments/assets/4c59f171-77c6-4c82-bab6-4d28b4e47ac3" />

Una vez hayamos modificado la vista los informes tendrán un aspecto más profesional como podemos ver en la siguiente imagen,

<img width="630" height="369" alt="image" src="https://github.com/user-attachments/assets/87bd74fa-ad65-4a2a-86c9-ea29e3116f19" />

Para finalizar exportamos los registros en formato .CSV para poder importarlos a cualquier otro sistema del mundo.

<img width="659" height="888" alt="image" src="https://github.com/user-attachments/assets/02c6e466-1043-41fd-be19-eb4d6b576314" />

Nos devolverá un archivo así:

<img width="602" height="270" alt="image" src="https://github.com/user-attachments/assets/d99b2236-6cf3-40a4-b72d-c3987d1f58ac" />

