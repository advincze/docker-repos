FROM alpine:3.3
MAINTAINER advincze@gmail.com

RUN apk update &&\
apk add openssl &&\
wget "https://releases.hashicorp.com/terraform/0.6.11/terraform_0.6.11_linux_amd64.zip" -O tf.zip &&\
unzip tf.zip -d tf &&\
rm tf/terraform-provider-atlas &&\
rm tf/terraform-provider-azure &&\
rm tf/terraform-provider-azurerm &&\
rm tf/terraform-provider-chef &&\
rm tf/terraform-provider-cloudflare &&\
rm tf/terraform-provider-cloudstack &&\
rm tf/terraform-provider-consul &&\
rm tf/terraform-provider-digitalocean &&\
rm tf/terraform-provider-dme &&\
rm tf/terraform-provider-dnsimple &&\
rm tf/terraform-provider-google &&\
rm tf/terraform-provider-heroku &&\
rm tf/terraform-provider-mailgun &&\
rm tf/terraform-provider-mysql &&\
rm tf/terraform-provider-openstack &&\
rm tf/terraform-provider-postgresql &&\
rm tf/terraform-provider-powerdns &&\
rm tf/terraform-provider-rundeck &&\
rm tf/terraform-provider-statuscake &&\
rm tf/terraform-provider-vcd &&\
rm tf/terraform-provider-vsphere &&\

COPY tf /tf

ENV env PATH /tf/:$PATH
