# erpnext-custom
Docker compose for v15 branch of ERPNext with payments and hrms modules.

The image used for this compose file is https://hub.docker.com/r/89neuron/erpnext_hrms_payments

The image is built with the documentation https://github.com/frappe/frappe_docker/blob/main/docs/custom-apps.md

The **docker-compose** file used is pwd.yaml located at  https://github.com/frappe/frappe_docker/blob/main/pwd.yml . The only difference is that in the site app, we have added the hrms and payments modules commands for installations as they are already present in the image.

