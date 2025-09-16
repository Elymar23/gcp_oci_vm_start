# gcp_oci_vm_start
GCP and OCI step by step tutorial
# Vitual Machine Tutorial: GCP & OCI

**Recording:** [Watch on Loom](https://www.loom.com/share/3083d00be535445b97c2cb42f8e749ec?sid=a3792a61-d27b-4e74-8951-efa0eb55a19b)

## Prereqs
- Google Cloud Platform (GCP)
- Oracle Cloud Infrastructure (OCI)
- Smallest free/tier shapes and images

## Part 1: Google Cloud Platform (GCP)

### Step 1: Create a VM
- Go to **Compute Engine** > **VM Instances** > **Create**.
- Fill in instance name using lower cases letters, example: ahi-tester
- Region & Zone: Choose a location closest to you
- Machine type: Leave as default (e2-micro)
- Leave defaults unless specified

![GCP Create Image]

### Step 2: Running Instance
- After clicking **Create**, wait until status is **Running**.

![GCP Running Instance]

### Step 3: Terminate VM
- Select the VM.
- Click **Delete**.

![GCP Terminated]

*Pitfall:* Don’t forget to delete the VM — leaving it running may cost money.


## Part 2: Oracle Cloud Infrastructure (OCI)

### Step 1: Create a VM
- Go to **Compute** > **Instances** > **Create Instance**.
- Select image and shape.

![OCI Create Image]

### Step 2: Running Instance
- Wait until instance state is **Running**.

![OCI Running]

### Step 3: Terminate VM
- Select the instance.
- Click **Terminate**.

![OCI Terminated]

## Reflections
### Similarities
- Both require you to choose: which Machine type
-- OS image and Storage
### Differences
Networking setup:
- GCP has networking pre-configured
- - GCP assigns public IP 
- OCI makes you set up VCNs and subnets, which feels more complicated
- OCI requires a public subnet
- GCP lets you access SSH with your Google account directly.
- OCI requires uploading or generating an SSH key.
### Preference 
- I think for  beginners: GCP is easier because of the automatic setup and Google account integration,
	but for someone who wants to have more control, OCI is is a better option.
