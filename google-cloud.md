# Google Cloud

## Introduction

* [https://cloud.google.com/sdk/docs/quickstarts](https://cloud.google.com/sdk/docs/quickstarts)
* [https://cloud.google.com/docs/overview/](https://cloud.google.com/docs/overview/)
* [https://github.com/GoogleCloudPlatform/awesome-google-cloud](https://github.com/GoogleCloudPlatform/awesome-google-cloud)
* [https://cloud.google.com/tools/docs/](https://cloud.google.com/tools/docs/)

## gcloud command line tool <a id="m_3622083399163848014gmail-GCP-gcloudcommandlinetool"></a>

[https://cloud.google.com/sdk/downloads](https://cloud.google.com/sdk/downloads)

[https://cloud.google.com/sdk/gcloud/reference/](https://cloud.google.com/sdk/gcloud/reference/)

## Kubernetes Engine <a id="m_3622083399163848014gmail-GCP-KubernetesEngine"></a>

[https://cloud.google.com/kubernetes-engine/docs/](https://cloud.google.com/kubernetes-engine/docs/)[https://kubernetes.io/docs/reference/kubectl/cheatsheet/\#kubectl-context-and-configuration](https://kubernetes.io/docs/reference/kubectl/cheatsheet/#kubectl-context-and-configuration)  
[https://cloud.google.com/kubernetes-engine/docs/tutorials/installing-istio](https://cloud.google.com/kubernetes-engine/docs/tutorials/installing-istio)

**k8s login GCP preprod**

| `gcloud container clusters get-credentials prod --zone europe-west1-b --project project-name` |
| :--- |


[https://kubernetes.io/docs/reference/kubectl/cheatsheet/](https://kubernetes.io/docs/reference/kubectl/cheatsheet/)

[https://eu.udacity.com/course/scalable-microservices-with-kubernetes–ud615](https://eu.udacity.com/course/scalable-microservices-with-kubernetes--ud615)

## Big Table <a id="m_3622083399163848014gmail-GCP-BigTable"></a>

* [https://cloud.google.com/bigtable/](https://cloud.google.com/bigtable/)
* [https://cloud.google.com/bigtable/docs/](https://cloud.google.com/bigtable/docs/)
* [https://cloud.google.com/bigtable/docs/go/cbt-overview](https://cloud.google.com/bigtable/docs/go/cbt-overview)
* [https://cloud.google.com/bigtable/docs/access-control](https://cloud.google.com/bigtable/docs/access-control) 
* **cbt command line tool**

```bash
https://
cloud.google.com/bigtable/docs/go/cbt-overview

/Users/username/.cbtrc    
project = project-name   
instance = instance-name

$cbt ls
```

## Storage <a id="m_3622083399163848014gmail-GCP-Storage"></a>

[https://console.cloud.google.com/storage/browser/](https://console.cloud.google.com/storage/browser/payments-bgl-preprod)

[https://cloud.google.com/storage/](https://cloud.google.com/storage/)

## Load Balancing <a id="m_3622083399163848014gmail-GCP-LoadBalancing"></a>

* [https://cloud.google.com/load-balancing/docs/network/](https://cloud.google.com/load-balancing/docs/network/)
* [https://cloud.google.com/kubernetes-engine/docs/tutorials/http-balance](https://cloud.google.com/kubernetes-engine/docs/tutorials/http-balancer)
* [https://cloud.google.com/load-balancing/docs/internal/](https://cloud.google.com/load-balancing/docs/internal/)
* [https://medium.com/google-cloud/kubernetes-nodeport-vs-loadbalancer-vs-ingress-when-should-i-use-what-922f010849e0](https://medium.com/google-cloud/kubernetes-nodeport-vs-loadbalancer-vs-ingress-when-should-i-use-what-922f010849e0)
* [https://cloud.google.com/kubernetes-engine/docs/how-to/internal-load-balancing](https://cloud.google.com/kubernetes-engine/docs/how-to/internal-load-balancing)
* [https://medium.com/google-cloud/internal-load-balancing-for-kubernetes-services-on-google-cloud-f8aef11fb1c4](https://medium.com/google-cloud/internal-load-balancing-for-kubernetes-services-on-google-cloud-f8aef11fb1c4)
* [https://estl.tech/configuring-https-to-a-web-service-on-google-kubernetes-engine-2d71849520d](https://estl.tech/configuring-https-to-a-web-service-on-google-kubernetes-engine-2d71849520d)
* [https://cloud.google.com/load-balancing/docs/health-check-concepts](https://cloud.google.com/load-balancing/docs/health-check-concepts)
* [https://kubernetes.io/docs/concepts/services-networking/service/](https://kubernetes.io/docs/concepts/services-networking/service/)
* [http://nishadikirielle.blogspot.com/2016/03/load-balancing-kubernetes-services-and.html](http://nishadikirielle.blogspot.com/2016/03/load-balancing-kubernetes-services-and.html)

"By default, to distribute traffic to instances, the Session Affinity is set to NONE. Google Cloud Load Balancing picks an instance based on a hash of the source IP and port, destination IP and port, and protocol. This means that incoming TCP connections are spread across instances and each new connection may go to a different instance. All packets for a connection are directed to the same instance until the connection is closed. Established connections are not taken into account when balancing.

Regardless of the session affinity setting, all packets for a connection are directed to the chosen instance until the connection is closed and have no impact on load balancing decisions for new incoming connections. This can result in imbalance between backends if long-lived TCP connections are in use.

You can choose a different Session Affinity setting if you need multiple connections from a client to go to the same instance. See sessionAffinity in the Target Pools documentation for more information."  
  
"In any of these proxy model, any traffic bound for the Service's IP:Port is proxied to an appropriate backend without the clients knowing anything about Kubernetes or Services or Pods. Client-IP based session affinity can be selected by setting service.spec.sessionAffinity to "ClientIP" \(the default is "None"\), and you can set the max session sticky time by setting the field service.spec.sessionAffinityConfig.clientIP.timeoutSeconds if you have already set service.spec.sessionAffinity to "ClientIP" \(the default is "10800"\)."

## Preemptible VM Instances <a id="m_3622083399163848014gmail-GCP-PreemptibleVMInstances"></a>

[https://cloud.google.com/compute/docs/instances/preemptible](https://cloud.google.com/compute/docs/instances/preemptible)

## Deployment Manager <a id="m_3622083399163848014gmail-GCP-DeploymentManager"></a>

Deployment Manager is an infrastructure deployment service that automates the creation and management of Google Cloud Platform resources for you.

Write flexible template and configuration files and use them to create deployments that have a variety of Cloud Platform services, such as Google Cloud Storage, Google Compute Engine, and Google Cloud SQL, configured to work together.

1. Docs [https://cloud.google.com/deployment-manager/docs/](https://cloud.google.com/deployment-manager/docs/)
2. How to use it [https://cloudplatform.googleblog.com/2016/11/what-is-Google-Cloud-Deployment-Manager-and-how-to-use-it.html](https://cloudplatform.googleblog.com/2016/11/what-is-Google-Cloud-Deployment-Manager-and-how-to-use-it.html) and [https://medium.com/google-cloud/infrastructure-as-code-on-google-cloud-platform-beginning-templates-68882e68d666](https://medium.com/google-cloud/infrastructure-as-code-on-google-cloud-platform-beginning-templates-68882e68d666)
3. Preview Configuration [https://cloud.google.com/deployment-manager/docs/configuration/preview-configuration-file](https://cloud.google.com/deployment-manager/docs/configuration/preview-configuration-file) \(project with activated billing is needed\)
4. gcloud command line reference tool [https://cloud.google.com/sdk/gcloud/reference/deployment-manager/](https://cloud.google.com/sdk/gcloud/reference/deployment-manager/)
5. examples [https://github.com/GoogleCloudPlatform/deploymentmanager-samples/tree/master/examples/v2](https://github.com/GoogleCloudPlatform/deploymentmanager-samples/tree/master/examples/v2)
6. GCP API roles [https://cloud.google.com/iam/docs/understanding-roles](https://cloud.google.com/iam/docs/understanding-roles)
7. Custom roles [https://cloud.google.com/iam/docs/understanding-custom-roles](https://cloud.google.com/iam/docs/understanding-custom-roles)
8. Sample permissions for BigTable [https://cloud.google.com/bigtable/docs/access-control](https://cloud.google.com/bigtable/docs/access-control)
9. Alternative to deployment-manager is [https://www.terraform.io/docs/providers/google/index.html](https://www.terraform.io/docs/providers/google/index.html)

### **custom role**

```bash
### jinja
  resources:
  - name: custom-role
    type: gcp-types/iam-v1:projects.roles
    properties:
      parent: projects/{{ env["project"] }}
      roleId: {{ properties["roleId"] }}
      role:
        title: {{ properties["title"] }}
        description: {{ properties["description"] }}
        stage: {{ properties["stage"] }}
        includedPermissions: {{ properties["includedPermissions"] }}
 
 
### yaml
 - name: app-bigtable-role
    type: roles/project_custom_role.jinja
    properties:
      roleId: bigtable.app
      title: App Bigtable role
      description: Role for managing BigTable
      stage: GA
      includedPermissions:
      - bigtable.tables.create
      - bigtable.tables.update
      - bigtable.tables.checkConsistency
      - bigtable.tables.generateConsistencyToken
      - bigtable.tables.get
      - bigtable.tables.list
      - bigtable.tables.mutateRows
      - bigtable.tables.readRows
      - bigtable.tables.sampleRowKeys
      - bigtable.appProfiles.get
      - bigtable.appProfiles.list
      - bigtable.clusters.get
      - bigtable.clusters.list
      - monitoring.metricDescriptors.get
      - monitoring.metricDescriptors.list
      - monitoring.timeSeries.list
      - resourcemanager.projects.get
```

### **service account**

```bash
### jinja
resources:
- name: {{ env['name'] }}
  type: iam.v1.serviceAccount
  properties:
    accountId: {{ properties['name'] }}
    displayName: serviceAccount-{{ properties['name'] }}
 
 
### yaml
 - name: app-bigtable-sa-prod
    type: accounts/service_account.jinja
    properties:
      name: app-prod
```

### add roles to service accounts

```bash
- name: get-iam-policy
   action: gcp-types/cloudresourcemanager-v1:cloudresourcemanager.projects.getIamPolicy
   properties:
     resource: project-id
 - name: add-iam-policy
   action: gcp-types/cloudresourcemanager-v1:cloudresourcemanager.projects.setIamPolicy
   properties:
     resource: project-id
     policy: $(ref.get-iam-policy)
     gcpIamPolicyPatch:
       add:
       - role: projects/project-name/roles/bigtable.app # custom role
         members:
         - serviceAccount:app-prod@project-id.iam.gserviceaccount.com
         - serviceAccount:app-stg@project-id.iam.gserviceaccount.com
       - role: roles/bigtable.reader
         members:
         - serviceAccount:app-prod-reader@project-id.iam.gserviceaccount.com
         - serviceAccount:app-stg-reader@project-id.iam.gserviceaccount.com
```

### Makefile deployment

```bash
DRY_RUN=true
 
ifeq ($(DRY_RUN), false)
    EXTRA_ARGS=
else
    EXTRA_ARGS=--preview
endif
 
# preprod
.PHONY: create-deployment
create-deployment:
    gcloud deployment-manager deployments create deployment-name --config config.yaml --project project-id $(EXTRA_ARGS)
 
.PHONY: update-deployment
update-deployment:
    gcloud deployment-manager deployments update deployment-name --config config.yaml --project project-id $(EXTRA_ARGS)
 
.PHONY: delete-deployment
delete-deployment:
    gcloud deployment-manager deployments delete deployment-name --project project-id
```

## Problems encountered <a id="m_3622083399163848014gmail-GCP-Problemsencountered"></a>

1. Created a role bigtable.some\_name , few weeks later that bigtable prefix became reserved name
2. Created service accouunt manually, later created account and assigned role using deployment manager. Older role was also assigned and was acting like the old one. Unassigned and assigned correct role and started working.
3. Was hard to find correct api resource for IAM. Cloud Resource Manager was the answer. 

## Terraform  <a id="m_3622083399163848014gmail-GCP-Terraform(currentlynotused)"></a>

**Roles, IAM, ServiceAccounts, BigTable done with Terraform**

```bash
provider "google" {
  project = "project-name"
}
 
 
### Big Table
resource "google_bigtable_instance" "bigtable-name" {
  name         = "bigtable-name"
  cluster_id   = "bigtable-name-cluster"
  zone         = "europe-west1-b"
  num_nodes    = 3
  storage_type = "SSD"
}
 
### Custom role
resource "google_project_iam_custom_role" "app-bigtable-role" {
  role_id     = "bigtable.app"
  title       = "App BigTable Role"
  description = "Role for managing BigTable"
  permissions = ["bigtable.tables.create",
    "bigtable.tables.update",
    "bigtable.tables.checkConsistency",
    "bigtable.tables.generateConsistencyToken",
    "bigtable.tables.get",
    "bigtable.tables.list",
    "bigtable.tables.mutateRows",
    "bigtable.tables.readRows",
    "bigtable.tables.sampleRowKeys",
    "bigtable.appProfiles.get",
    "bigtable.appProfiles.list",
    "bigtable.clusters.get",
    "bigtable.clusters.list",
    "monitoring.metricDescriptors.get",
    "monitoring.metricDescriptors.list",
    "monitoring.timeSeries.list",
    "resourcemanager.projects.get",]
}
 
### service account
resource "google_service_account" "app-bigtable-sa-prod" {
  account_id   = "app-prod"
  display_name = "serviceAccount-app-prod"
}
 
### service account
resource "google_service_account" "app-bigtable-sa-prod-reader" {
  account_id   = "app-prod-reader"
  display_name = "serviceAccount-app-prod-reader"
}
 
 
### assigned custom role
resource "google_project_iam_binding" "app-prod-role" {
  role    = "projects/project-name/roles/bigtable.app"
 
  members = ["serviceAccount:app-prod@project-name.iam.gserviceaccount.com"]
}
 
 
### assigned predefined BigTable role
resource "google_project_iam_binding" "app-prod-role-reader" {
  role    = "roles/bigtable.reader"
 
  members = ["serviceAccount:app-prod-reader@project-name.iam.gserviceaccount.com"]
}
```

