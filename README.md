herramientas:

python
postgresql
git


---
python -m .venv .
source .venv/bin/activate
pip install -r requirements.txt
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver

---
funcionalidad de cada carpeta app_*

app_base: configuracion general como el footer, navigation settings, funcionalidades que puedan afectar a todo el proyecto en general

app_contact: relacionado a información de contacto o la manera en la que los usuarios puedan contactar al market place

app_cronjobs: relacionado a ejecutables periodicos, como lo es la generacion de informes de venta diarios, mensuales, comprobar constantemente que usuario esta actualizado en confirmación de pago para enviar notificación o certificado de compra, actualizar la base de datos, etc

app_dashboard: relacionado a personalizar el panel administrativo, en login, y en el panel de usuario administrativo registrado

app_integrations: gestion de integraciones externas como pasarelas de pago y aliados

app_payment_invoices: gestion de facturas de pago, metodos de pago, todo lo relacionado con el proceso de pagos

app_product: gestion de productos, como clasificacion, descripcion, imagen, etc

app_user_management: gestion de usuarios, administrativos, clientes, permisos de usos de api

home: configuracion de pagina de inicio