# erpnext-custom
Docker compose for v15 branch of ERPNext with payments and hrms modules.

The image used for this compose file is https://hub.docker.com/r/89neuron/erpnext_hrms_payments

The image is built with the documentation https://github.com/frappe/frappe_docker/blob/main/docs/custom-apps.md
From the above endpoint , it is important to set 
`export APPS_JSON_BASE64=$(echo ${APPS_JSON} | base64 -w 0)`
Without this, the installation may not be of use even if succeeded .

The documentation suggests to build with buildah but building with docker does the same job. We built it with docker. 


The **docker-compose** file used is pwd.yaml located at  https://github.com/frappe/frappe_docker/blob/main/pwd.yml . The only difference is that in the site app, we have added the hrms and payments modules commands for installations as they are already present in the image.

