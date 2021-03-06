---
layout: default
title: 1. Create Kubernetes Cluster
---

# Lab 1 - Create a Kubernetes Cluster

1. [Register for IBM Cloud](#part-SETUP-00)
2. [Insert feature code](#part-SETUP-01)
3. [Create a free Kubernetes cluster](#part-SETUP-02)
4. [Configure the IBM Cloud Container Registry](#part-SETUP-03)

# 1. Register for IBM Cloud <a name="part-SETUP-00"></a>

#### Step 1: Open a browser window and navigate to the IBM Cloud [Registration page](https://cloud.ibm.com/registration){:target="_blank"}.

![image](images/registration.png)

#### Step 2: Follow the instructions to confirm your account.

You will receive an email with a confirmation code.

#### Step 3: [Login into IBM Cloud](https://cloud.ibm.com){:target="_blank"} using your account credentials.

_Note:_ By default, all new IBM Cloud accounts are set to a [lite version](https://www.ibm.com/cloud/pricing).

The lite account provides free access to a subset of IBM Cloud resources. Lite accounts **don't need a credit-card** to sign up and they **don't expire** after a certain period of time. 
In order to create a free Kubernetes cluster, you need a **feature code**.

---

# 2 Insert feature code <a name="part-SETUP-01"></a>

In order to execute the workshop easily, we provide **feature codes** to create free Kubernetes clusters, so no credit card details are required.
To apply the feature code to your [Cloud Account](https://cloud.ibm.com/account){:target="_blank"}, navigate to your "`Account settings`" and then to ("`Manage`" -> "`Account`").
Enter your unique Feature (Promo) Code to upgrade your lite account.

_Note:_ Free clusters expire after one month (30 days).

---

# 3 Create a free Kubernetes Cluster <a name="part-SETUP-02"></a>

#### Step 1: Logon to IBM Cloud

#### Step 2: Select in the menu "Catalog" and search for "Kubernetes"

![Kubernetes service](images/ibmcloud-catalog.png)

#### Step 3: Click on "Kubernetes Service"

#### Step 4: Select the "Free" plan

![create Kubernetes service](images/ibmcloud-create-kubernetes-1.png)

#### Step 5: Give it a name

Ensure you set following values in the creation dialog:

* Cluster name:     cloud-native
* Resource group:   Default

![create Kubernetes service](images/ibmcloud-create-kubernetes-2.png)

#### Step 6: Press "Create custer"

#### Step 7: Now you will be forwarded to your cluster on IBM Cloud and you can verify the status of the creation of your cluster

The creation of the cluster takes up to 20 min.

---

# 4 Configure the IBM Cloud Container Registry <a name="part-SETUP-03"></a>

1. Select in **Kubernetes** the entry **Registry** and ensure your are in the **Dallas location**.

![Select in Kubernetes the entry Registry](images/ibmcloud-configure-container-registry-1.gif)

2. The create a namespace with a unique name cloud-native-[YOURNAME]

![The create a namespace with a unique name cloud-native](images/ibmcloud-configure-container-registry-2.gif)

_Note:_ Namespaces are required to be **unique** across the entire **region** that the **specific registry** is located in, not just **unique to your account**. This is mentioned in the following [public documentation](https://cloud.ibm.com/docs/services/Registry?topic=registry-getting-started#gs_registry_namespace_add).

---

Now we have created a free IBM Kubernetes Cluster and we configured the IBM Cloud Container Registry.

__Continue with [the tools prerequisites](./1-prereqs.md#tools)__ 
