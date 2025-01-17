


## August 30<sup>th</sup> 2021

Run:AI now supports a self-hosted installation. With the self-hosted installation the Run:AI control-plane (or _backend_) which typically resides on the cloud, is deployed at the customer's data center. For further details on  supported installation types see [Installation Types](../admin/runai-setup/installation-types.md).

!!! Note
    The Run:AI self-hosted installation requires a dedicated license, and has different pricing than the SaaS installation. For more details contact your Run:AI account manager.

NFS volumes can now be mounted directly to containers run by Run:AI while submitting jobs via Run:AI. See the `--nfs-server` flag of [runai submit](../Researcher/cli-reference/runai-submit.md).

To ease the manageability of user templates, Run:AI now supports _global user templates_. Global user templates are user templates that are managed by the Run:AI administrator and are available for all the projects within a specific cluster. The purpose of global user templates is to help define and enforce cross-organization resource policies.

To simplify researchers' job submission via the Run:AI Researcher User Interface (UI), the UI now supports autocomplete, which is based on pre-defined values, as configured by the Administrator using the administrative templates.

Run:AI extended the usage of Cluster name, as defined by the Administrator while configuring clusters at Run:AI. The Cluster name is now populated to the Run:AI dashboards as well as the Researcher UI.

The original command line, which was used for running a Job, is now shown under the Job details under the _General_ tab.
## August 4<sup>th</sup> 2021

Researcher User Interface (UI) enhancements:

* Revised user interface and user experience
* Researchers can create templates for the ease of jobs submission. Templates can be saved and used in the project level
* Researchers can be easily re-submit jobs from the Submit page or directly from the jobs list in the Jobs page
* Administrators can create administrative templates which set cluster-wide defaults, constraints and defaults for the submission of Jobs. For further details see [Configure Command-Line Interface Templates](../admin/researcher-setup/templates.md).
* Different teams can collaborate and share templates by exporting and importing templates in the Submit screen

Researcher Command Line Interface (CLI) enhancements:

* Jobs can be manually suspended and resumed using the new commands: `runai suspend` & `runai resume`
* A new command was added: `runai top job`

Kubeflow integration is now supported. The new integration allows building ML pipelines in [Kubeflow Pipelines](https://www.kubeflow.org/docs/components/pipelines/){target=_blank} as well as [Kubeflow Notebooks](https://www.kubeflow.org/docs/components/notebooks/){target=_blank} and run the workloads via the Run:AI platform. For further details see [Integrate Run:AI with Kubeflow](../admin/integration/kubeflow.md).

Mlflow integration is now supported. For further details see [Integrate Run:AI with MLflow](../admin/integration/mlflow.md).

Run:AI Projects are implemented as Kubernetes namespaces. Run:AI now supports customizable namespace names. For further details see [Manual Creation of Namespaces](../admin/runai-setup/cluster-setup/customize-cluster-install.md).


## May 10<sup>th</sup> 2021
 
Usability improvements of Run:AI Command-line interface (CLI). The CLI now supports autocomplete for all options and parameters.
 
Usability improvements of the Administration user interface navigation menu now allow for easier navigation.
 
Run:AI can be installed  when Kubernetes has [Pod Security Policy (PSP)](https://kubernetes.io/docs/concepts/policy/pod-security-policy/){target=_blank} enabled.


## April 20<sup>th</sup> 2021

Job List and Node list now show the GPU type (e.g. v-100).


## April 18<sup>th</sup>, 2021

Inference workloads are now supported. For further details see [Inference Overview](../developer/inference/overview.md).

JupyterHub integration is now supported. For further details see [JupyterHub Integration](../admin/integration/jupyterhub.md)


NVIDIA [MIG](https://www.nvidia.com/en-us/technologies/multi-instance-gpu/){target=_blank} is now supported. You can use the NVIDIA MIG technology to partition A-100 GPUs. Each partition will be considered as a single GPU by the Run:AI system and all the Run:AI functionality is supported in the partition level, including GPU Fractions.



## April 1<sup>st</sup>, 2021

Run:AI now supports Kubernetes 1.20

## March 24th 2021

Job List and Node list now show CPU utilization and CPU memory utilization.

## February 14th, 2021

The Job list now shows per-Job graphs for GPU utilization, GPU memory. 

The Node list now shows per-Node graphs for GPU utilization, GPU memory. 


## January 22<sup>nd</sup>, 2021

New Analytics dashboard with emphasis on CPU, CPU Memory, GPU and GPU Memory. Allows better diagnostics of resource misuse. 

## January 15th, 2021

New developer documentation area has been [created](../developer/overview-developer.md). In it:

* New documentation for [Researcher REST API](../developer/researcher-rest-api/overview.md).
* New documentation for [Administration Rest API](../developer/admin-rest-api/overview.md).
* Kubernetes-based API for [job creation](../developer/k8s-api/launch-job-via-kubernetes-api.md).

## January 9th 2021

A new Researcher user interface is now available. See [researcher UI setup](../admin/researcher-setup/researcher-ui-setup.md).

## January 2nd, 2021

Run:AI Clusters now support Azure Managed Kubernetes Service (AKS)

