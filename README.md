  <h1>Anthos Service Mesh</h1>
  <h2> Background: </h2>
<h3> Application architectures, along with examples for each architecture type: </h3>
  <table>
  <tr>
    <th>Architecture</th>
    <th>Characteristics</th>
    <th>Example</th>
  </tr>
  <tr>
    <td>Monolith</td>
    <td>
      <ul>
          <li>Single, tightly-coupled application where all components are interconnected</li>
          <li>Difficult to scale and maintain as the entire application needs to be deployed and updated together</li>
          <li>Changes to one part of the application can impact other parts</li>
      </ul> 
    </td>
    <td>
      <ul>
        <li>Traditional e-commerce platform with a single codebase</li>
        <li>A banking system with a single application handling customer accounts, transactions, and reports.</li>
    </td>
  </tr>
  <tr>
    <td>N-tier Architecture</td>
    <td>
      <ul>
          <li>Separation of application into distinct layers (presentation, business logic, data)</li>
          <li>Moderate coupling between layers, allowing for better maintenance and scalability</li>
          <li>Communication happens via APIs or function calls between layers</li>
      </ul> 
    </td>
    <td>
      <ul>
        <li>Three-tier web application with a separate database, backend, and frontend</li>
        <li>An online marketplace with separate frontend, backend, and database layers</li>
    </td>
  </tr>
  <tr>
    <td>Event-driven Architecture</td>
    <td>
      <ul>
          <li>System components communicate through events and messages</li>
          <li>Events trigger actions or updates in other components, promoting flexibility and Enables handling real-time data streams and reacting to events in near real-time</li>
      </ul> 
    </td>
    <td>
      <ul>
        <li>Internet of Things (IoT) platform processing sensor data</li>
        <li>A ride-sharing app where location updates trigger driver allocation and notifications</li>
    </td>
  </tr>
  <td>Microservices</td>
    <td>
      <ul>
          <li>Application divided into small, independent services that can be developed, deployed, and scaled separately</li>
          <li>Each service has its own data store and can be developed using different technologies</li>
          <li>Loose coupling between services enables flexibility and faster development and Services communicate via lightweight protocols such as HTTP or message queues</li>
      </ul> 
    </td>
    <td>
      <ul>
        <li>An e-commerce platform with separate services for user management, inventory, and payments</li>
        <li>Applications with separate services for user management, catalog, recommendations</li>
    </td>
  </tr>
  <tr>
    <td>Service-oriented Architecture</td>
    <td>
      <ul>
          <li>Application divided into self-contained services that expose their functionality as services</li>
          <li>Services can be combined to create composite applications and Communication occurs via standardized protocols like SOAP or REST	</li>
      </ul> 
    </td>
    <td>
      <ul>
        <li>Enterprise resource planning (ERP) system with modular services</li>
        <li>A logistics system with separate services for tracking shipments, inventory management, and billing</li>
    </td>
  </tr>
</table>	
  
  <p> <b><i>As microservices architectures become more prevalent, effective service-to-service communication and management are crucial. Anthos Service Mesh addresses these challenges head-on.</i></b></p>
  
  <h2>Challenges of Microservices Architecture</h2>
  <ul>
    <li>Managing service-to-service communication in a distributed environment with numerous interconnected microservices</li>
    <li>Ensuring reliable and efficient communication between services as their number grows</li>
    <li>Complex tasks of service discovery, load balancing, routing, and fault tolerance</li>
  </ul>
  
  <h2>Effective Service-to-Service Communication and Management</h2>
  <ul>
    <li>Introduction of service mesh as a dedicated infrastructure layer for handling service-to-service communication</li>
    <li>Service mesh provides features such as traffic routing, load balancing, security, and observability</li>
    <li>Ensures resilience, security, and performance of applications</li>
  </ul>
  
  <h2>Development of Anthos Service Mesh</h2>
  <ul>
    <li>Anthos Service Mesh is developed based on Istio, an open-source service mesh project</li>
    <li>Google Cloud, in collaboration with other companies, contributed to the development of Istio</li>
    <li>Anthos Service Mesh builds upon Istio's foundation to provide a fully-managed service mesh solution</li>
    <li>Includes expertise and contributions from a vibrant open-source community</li>
  </ul>
  
  <h2>What is Anthos Service Mesh?</h2>
  <p>Anthos Service Mesh is a fully-managed service mesh designed specifically for applications with microservice architecture. It is built on Istio, an open-source project that provides a powerful framework for managing microservices. Anthos Service Mesh takes Istio's capabilities and offers a comprehensive, managed solution, making it easier to deploy and operate in production environments.</p>
  
  <h2>Deployment Options in Anthos Service Mesh</h2>
  <h3>Managed Anthos Service Mesh</h3>
  <ul>
    <li>Deployment: Fully managed by the provider</li>
    <li>Control Plane: Managed by the provider</li>
    <li>Operations: Provider handles operations</li>
    <li>Scalability: Automatically scalable</li>
    <li>Upgrades and Patches: Managed by the provider</li>
    <li>Availability: Provider ensures availability</li>
    <li>Configuration: Simplified configuration</li>
    <li>Cost and Complexity: Simplified setup and management, but comes with a cost</li>
    <li>Additional Features: May have additional features, integrations, and value-added managed services provided by the cloud provider</li>
  </ul>
  
  <h3>In-cluster control plane Anthos Service Mesh</h3>
  <ul>
    <li>Deployment: Deployed within the cluster</li>
    <li>Control Plane: Self-managed</li>
    <li>Operations: Requires manual operations</li>
    <li>Scalability: Limited by cluster resources</li>
    <li>Upgrades and Patches: Requires manual upgrades</li>
    <li>Availability: Reliant on cluster stability</li>
    <li>Configuration: Requires manual configuration</li>
    <li>Cost and Complexity: Lower upfront cost but requires more effort in setup and management</li>
    <li>Additional Features: Relies on the features available in the open-source Istio project</li>
  </ul>
  
  <h2>Key Features of Anthos Service Mesh</h2>
  <h3>Traffic Management</h3>
  <ul>
    <li>Efficient traffic routing and load balancing between microservices</li>
    <li>Definition and enforcement of sophisticated traffic management policies</li>
  </ul>
  
  <h3>Security and Observability</h3>
  <ul>
    <li>Enhanced application security through authentication, authorization, and encryption</li>
    <li>Built-in monitoring, tracing, and logging capabilities for deep insight into microservice behavior and performance</li>
  </ul>
  
  <h3>Service Mesh Expansion</h3>
  <ul>
    <li>Extension of the service mesh across multiple clusters and on-premises environments</li>
    <li>Consistent management and control over microservices regardless of their location</li>
  </ul>
  
  <h2>How to Use Anthos Service Mesh</h2>
  <h3>Deploying Anthos Service Mesh</h3>
  <ul>
  	    <li> Ensure you have the necessary permissions and access to manage the GKE cluster and install Anthos Service mesh in the cluster.</li> 
        <pre>
        <b>Roles required:</b>
              GKE Hub Admin 
              Kubernetes 
              Mesh Config Admin 
              Service Account Admin 
              Service Management Admin 
              Service Account Admin 
              CA Service Admin  
              Service Usage Admin
        </pre>
  	<li> Start by setting up a Kubernetes cluster where you want to deploy Anthos Service Mesh.</li>
    <pre>
    	<b>Export environment variables:</b>
          export PROJECT_ID=$(gcloud config get-value project)
          export PROJECT_NUMBER=$(gcloud projects describe ${PROJECT_ID} \
              --format="value(projectNumber)")
          export CLUSTER_NAME= #enter prefered cluster name
          export CLUSTER_ZONE= #enter prefered cluster zone
          export WORKLOAD_POOL=${PROJECT_ID}.svc.id.goog
          export MESH_ID="proj-${PROJECT_NUMBER}"
          export MEMBERSHIP= #enter cluster name
	</pre>
    <pre>
        <b>Create a GKE cluster:</b>
        	gcloud config set compute/zone ${CLUSTER_ZONE}
            gcloud beta container clusters create ${CLUSTER_NAME} \
                --machine-type=n1-standard-4 \
                --num-nodes=3 \
                --workload-pool=${WORKLOAD_POOL} \
                --enable-stackdriver-kubernetes \
                --subnetwork=default \
                --release-channel=regular \
                --labels mesh_id=${MESH_ID}
    </pre>
    <p><b>NOTE:</b>ASM requirements -
 If the machine type has 4 vCPUs, your cluster must have at least 2 nodes. If the machine type has 8 vCPUs, the cluster only needs 1 node.</p>
    </ul>
  
  <h3>Configuring Components</h3>
  <ul>
  	<li>Once the control plane is deployed, configure the components to fit your application's requirements.</li>
    <li>Define the namespaces and services that will be included in the service mesh.</li>
    </ul>
    
  
  <h3>Traffic Routing and Management</h3>
  <ul>
  <li>Utilize the powerful traffic management capabilities of Anthos Service Mesh.</li> <li>Define traffic routing rules based on HTTP headers, URL patterns, or specific user identities.
  <a href="https://istio.io/latest/docs/concepts/traffic-management/">Istio / Traffic Management</a></li> 
  <li>Leverage traffic splitting and canary deployments for gradual rollout of new service versions. 
  <a href="https://cloud.google.com/service-mesh/v1.16/docs/unified-install/plan-upgrade">Plan an upgrade | Anthos Service Mesh | Google Cloud</a></li>
  <li>Configure load balancing and circuit breaking policies to ensure optimal performance and resilience.</li></ul>
  
  <h3>Applying Security Policies</h3>
  <ul>
  <li>Apply authentication and authorization policies to authenticate incoming requests and enforce access control. </li>
  <li>Enable encryption and secure communication between services using mutual TLS (mTLS). 
  </li>
  <li>Anthos Service Mesh automatically generates and manages certificates for secure communication.</li>
  </ul>
  
  <h3>Enabling Observability</h3>
  <ul>
  <li>Enable built-in monitoring and distributed tracing for your services. </li>
  <li>Gain insights into service behavior, latency, error rates, and request traces for effective debugging and optimization.</li>
  <li>Configure logging to capture important events and diagnose issues. Anthos Service Mesh integrates with popular observability tools like Prometheus and Jaeger.</li>
  </ul>
  
  <h2>Advantages of Anthos Service Mesh</h2>
  <ul>
    <li>Enhanced observability for effective monitoring and troubleshooting</li>
    <li>Improved security and compliance with consistent policies and encryption</li>
    <li>Smarter traffic control and resilience with intelligent routing and fault tolerance mechanisms</li>
    <li>Increased developer productivity by abstracting low-level networking concerns</li>
  </ul>
  
  <h2>Disadvantages of Anthos Service Mesh</h2>
  <ul>
    <li>Introduction of additional complexity to the infrastructure and application stack</li>
    <li>Potential performance overhead due to additional layers of networking and proxying</li>
    <li>Increased resource consumption with additional infrastructure components</li>
    <li>Potential vendor lock-in and limited flexibility in adopting alternative service mesh solutions</li>
  </ul>
  
  <h2>Conclusion</h2>
  <p>Anthos Service Mesh is a powerful tool that simplifies the management and security of cloud-native applications. By leveraging its features, organizations can enhance observability, improve security, achieve smarter traffic control, and increase developer productivity. However, it is essential to consider the complexity, performance overhead, resource consumption, and potential vendor lock-in associated with Anthos Service Mesh.</p>
  
   <h4>________________________________________________________________________________________________________________________________________________________</h4>
   
  <h1>Steps to install Anthos Service Mesh on a GKE cluster</h1>
    
  <h2>Make sure to have all these permissions while installing the Anthos Service Mesh.</h2>
  <a href="https://cloud.google.com/service-mesh/docs/installation-permissions">Installation permissions</a>
  <pre>
ROLES=(
'roles/servicemanagement.admin' \
'roles/serviceusage.serviceUsageAdmin' \
'roles/meshconfig.admin' \
'roles/compute.admin' \
'roles/container.admin' \
'roles/iam.serviceAccountAdmin' \
'roles/iam.serviceAccountKeyAdmin' \
'roles/gkehub.admin')
for role in "${ROLES[@]}"
do
  gcloud projects add-iam-policy-binding &lt;project-id&gt; \
    --member "user:&lt;user-mail&gt;" \
    --role="$role"
done
  </pre>
  <h2>Configure environment variables:</h2>
  <pre>
export PROJECT_ID=$(gcloud config get-value project)
export PROJECT_NUMBER=$(gcloud projects describe ${PROJECT_ID} --format="value(projectNumber)")
export CLUSTER_NAME=CLUSTER_NAME
export CLUSTER_ZONE=CLUSTER_ZONE
export WORKLOAD_POOL=${PROJECT_ID}.svc.id.goog
export MESH_ID="proj-${PROJECT_NUMBER}"
export MEMBERSHIP=MEMBERSHIP_NAME
  </pre>
  <h2>Enable the APIs that you need:</h2>
  <pre>
gcloud services enable mesh.googleapis.com
  </pre>
  <h2>Set the mesh_id label:</h2>
  <pre>
gcloud container clusters update ${CLUSTER_NAME} \
    --project ${PROJECT_ID} \
    --zone ${CLUSTER_ZONE} \
    --update-labels=mesh_id=${MESH_ID}
  </pre>
  <p><b>NOTE:</b> Follow this step if you didn't label the cluster with mesh_id while creating your cluster.</p>
  <h2>Enable Workload Identity:</h2>
  <p>To enable Workload Identity on an existing cluster, run the following command:</p>
  <pre>
gcloud container clusters update ${CLUSTER_NAME} \
    --zone=${CLUSTER_ZONE} \
    --workload-pool=${PROJECT_ID}.svc.id.goog
  </pre>
  <p><b>NOTE:</b> <a href="https://cloud.google.com/kubernetes-engine/docs/how-to/workload-identity#enable-existing-cluster">Enable workload identity</a> 
  Follow this step if you didn't enable workload identity while creating your cluster.</p>
  <h2>Enable Cloud Monitoring and Cloud Logging on GKE:</h2>
  <pre>
gcloud container clusters update ${CLUSTER_NAME} \
    --project ${PROJECT_ID} \
    --zone ${CLUSTER_ZONE} \
    --enable-stackdriver-kubernetes
  </pre>
  <p><b>Verify Cloud Monitoring and Cloud Logging is enabled:</b></p>
  <pre>
gcloud container clusters describe ${CLUSTER_NAME} --zone ${CLUSTER_ZONE} --format="value(monitoringService.enable)"
gcloud container clusters describe ${CLUSTER_NAME} --zone ${CLUSTER_ZONE} --format="value(loggingService.enable)"
</pre>

  <p><b>Note:</b> Returns true or an empty string.</p>
  <h2>Register your cluster to a fleet:</h2>
  <pre>
gcloud container fleet memberships register ${MEMBERSHIP} \
    --project ${PROJECT_ID} \
    --gke-cluster ${CLUSTER_ZONE}/${CLUSTER_NAME} \
    --enable-workload-identity
  </pre>
  <h2>Enable Anthos Service Mesh in your fleet:</h2>
  <pre>
gcloud container fleet mesh enable
  </pre>
  <h2>Connect to the GKE cluster:</h2>
  <pre>
gcloud container clusters get-credentials ${CLUSTER_NAME} \
    --zone ${CLUSTER_ZONE} \
    --project ${PROJECT_ID}
  </pre>
  <p><b>Ensure you have set the context to your user cluster:</b></p>
  <pre>
kubectl config use-context CONTEXT_NAME
  </pre>
  <p><b>NOTE:</b> To check existing contexts, run <code>kubectl config get-contexts</code>. You can use the default context (current context is indicated by the '*' mark).</p>
  <h2>Grant cluster admin permissions to your user account (your Google Cloud login email address):</h2>
  <pre>
kubectl create clusterrolebinding cluster-admin-binding \
  --clusterrole=cluster-admin \
  --user=<user-account>
  </pre>
  <p><b>Verify:</b> <code>kubectl describe clusterrolebinding cluster-admin-binding</code></p>
  <p><b>NOTE:</b> You need these permissions to create the necessary role-based access control (RBAC) rules for Anthos Service Mesh.</p>
  <h2>Install asmcli:</h2>
  <pre>
curl https://storage.googleapis.com/csm-artifacts/asm/{latest/stable-version} > asmcli
  </pre>
  <p><b>NOTE:</b> Replace {latest/stable-version} with the latest version of asmcli (Eg: asmcli_1.17.2 version).</p>
  <h2>Make the script executable:</h2>
  <pre>
chmod +x asmcli
  </pre>
  <p><b>NOTE:</b> Replace {latest/stable-version} with the latest version of asmcli (Eg: asmcli_1.17.2 version).</p>
  <h2>Validate that the GKE cluster is compatible with ASM:</h2>
  <pre>
./asmcli validate \
  --project_id ${PROJECT_ID} \
  --cluster_name ${CLUSTER_NAME} \
  --cluster_location ${CLUSTER_ZONE} \
  --fleet_id ${PROJECT_ID} \
  --output_dir DIR_PATH
  </pre>
  <p><b>NOTE:</b> Include the --output_dir option to specify a directory where asmcli downloads the asm package and extracts the installation file, which contains istioctl, samples, and manifests.</p>
  <h2>Install ASM on the cluster:</h2>
  <p>1. In-cluster control plane ASM on a GKE cluster:</p>
  <pre>
./asmcli install \
  --project_id ${PROJECT_ID} \
  --cluster_name ${CLUSTER_NAME} \
  --cluster_location ${CLUSTER_ZONE} \
  --fleet_id ${PROJECT_ID} \
  --output_dir asm-output \
  --enable_gcp_components \
  --enable_gcp_apis \
  --enable_namespace_creation \
  --option cloud-tracing \
  --ca mesh_ca
  </pre>
  <p><b>NOTE:</b> The "--option cloud-tracing" is used to enable Cloud Traces for the mesh. You can also use "--option legacy-default-ingressgateway" to install the default ingress gateway.</p>
  <p>2. Managed ASM on a GKE cluster:</p>
  <pre>
./asmcli install \
  -p ${PROJECT_ID} \
  -l ${CLUSTER_ZONE} \
  -n ${CLUSTER_NAME} \
  --fleet_id ${PROJECT_ID} \
  --managed \
  --verbose \
  --output_dir asm-output \
  --enable-all \
  --channel RELEASE_CHANNEL
  </pre>
  <p><b>NOTE:</b> Replace RELEASE_CHANNEL with the appropriate channel: regular, stable, or rapid. <a href="https://cloud.google.com/service-mesh/docs/managed/select-a-release-channel">Select a managed Anthos Service Mesh release channel | Google Cloud</a></p>
  <h2>To enable automatic sidecar injection on a namespace:</h2>
  <pre>
REVISION=$(kubectl get deploy -n istio-system -l app=istiod -o jsonpath={.items[*].metadata.labels.'istio\.io\/rev'}'{"\n"}')
kubectl label namespace NAMESPACE istio-injection- istio.io/rev=$REVISION --overwrite
</pre>

  <p><b>OR</b></p>
  <p><b>NOTE:</b> If the default tag is pointing to the installed revision, you can check that using <code>istioctl tag list</code>.</p>
  <pre>
kubectl label namespace NAMESPACE istio-injection=enabled istio.io/rev- --overwrite
  </pre>
  <p><b>NOTE:</b> Replace NAMESPACE with your namespace.</p>
  <h2>Verify that ASM is installed:</h2>
  <pre>
kubectl get namespaces -w
  </pre>
  <p><b>NOTE:</b> You should see the istio-system namespace being created, which contains the Istio components that make up ASM.</p>
  <h2>Update the existing deployments and services to use ASM:</h2>
  <pre>
kubectl rollout restart deployment -n NAMESPACE
  </pre>
  <p><b>NOTE:</b> Replace NAMESPACE with your namespace, replace with the deployment for which you want to inject the sidecar proxy.</p>
  <h3>Additional Note:</h3>
  <p><b>NOTE:</b> We can install Managed ASM using the fleet API also using this command:</p>
  <pre>
Enable managed Anthos Service Mesh on the cluster using fleet API:
gcloud container fleet mesh update \
  --management automatic \
  --memberships ${MEMBERSHIP} \
  --project ${PROJECT_ID}
  </pre>
  
  <h4>________________________________________________________________________________________________________________________________________________________</h4>
  
  <h1 id="eq">Steps to install Anthos Service Mesh Installation on Equinix bare metal cluster(On prem clsuter)</h1>

<h2>Make sure to have all these permissions while installing the ASM (If you have all the roles mentioned, we don't need the Project IAM Admin role). <a href="https://cloud.google.com/service-mesh/docs/installation-permissions">Installation Permissions</a></h2>
<pre>
ROLES=(
'roles/servicemanagement.admin' \
'roles/serviceusage.serviceUsageAdmin' \
'roles/meshconfig.admin' \
'roles/compute.admin' \
'roles/container.admin' \
'roles/resourcemanager.projectIamAdmin' \
'roles/iam.serviceAccountAdmin' \
'roles/iam.serviceAccountKeyAdmin' \
'roles/gkehub.admin')
for role in "${ROLES[@]}"
do
  gcloud projects add-iam-policy-binding &lt;project-id&gt; \
    --member "user:&lt;user-mail&gt;" \
    --role="$role"
done
</pre>

<h2>Enable the APIs that you need:</h2>
<pre>
gcloud services enable \
    mesh.googleapis.com
</pre>

<h2>Connect to the Anthos Equinix cluster by exporting the kube-config file:</h2>
<pre>
export KUBECONFIG=&lt;KUBECONFIG_FILE&gt;
</pre>

<h2>Enable Anthos Service Mesh in your fleet:</h2>
<pre>
gcloud container fleet mesh enable
</pre>

<h2>Install asmcli:</h2>
<pre>
curl https://storage.googleapis.com/csm-artifacts/asm/{latest/stable-version} > asmcli
</pre>

<h2>Make the script executable:</h2>
<pre>
chmod +x asmcli
</pre>

<h2>Grant cluster admin permissions to your user account (your Google Cloud login email address):</h2>
<pre>
kubectl create clusterrolebinding cluster-admin-binding \
    --clusterrole=cluster-admin \
    --user=&lt;USER_ACCOUNT&gt;
</pre>
<p><b>NOTE:</b> You need these permissions to create the necessary role-based access control (RBAC) rules for Anthos Service Mesh.</p>

<h2>Validate project and cluster:</h2>
<pre>
./asmcli validate \
    --kubeconfig &lt;KUBECONFIG_FILE&gt; \
    --fleet_id &lt;FLEET_PROJECT_ID&gt; \
    --output_dir &lt;DIR_PATH&gt; \
    --platform multicloud
</pre>
<p><b>NOTE:</b> If you get errors on --enable_all or --enable_* tags, add the tag while installing ASM. asmcli validate doesn't allow any enablement flags because it only validates that your project and cluster are ready for installation.</p>

<h2>Install Anthos Service Mesh:</h2>
<pre>
./asmcli install \
    --fleet_id &lt;FLEET_PROJECT_ID&gt; \
    --kubeconfig &lt;KUBECONFIG_FILE&gt; \
    --output_dir &lt;DIR_PATH&gt; \
    --platform multicloud \
    --enable_all \
    --ca mesh_ca
</pre>
<p><b>NOTE:</b> This will install Anthos Service Mesh with the default supported features for your platform and enable Anthos Service Mesh certificate authority (Mesh CA) as the certificate authority. We can use other certificate authorities and explore other options according to the requirements and platform we're installing the ASM.</p>

<p>After successfully installing ASM, label the namespace you used to create the workloads on the cluster with "istio revision tag" or with istio-injection tag if the default tag is pointing to the current version revision tag (istioctl tag list). This will enable the sidecar injection automatically:</p>

<pre>
kubectl label namespace &lt;namespace&gt; istio-injection- istio.io/rev=asm-1162-2 --overwrite
</pre>

<h2>Restart the existing workloads to monitor the services on the ASM dashboard:</h2>
<pre>
kubectl rollout restart deployment/&lt;deployment-name&gt; -n &lt;namespace&gt;
</pre>
<p><b>NOTE:</b> Managed ASM is not supported on clusters outside Google cloud </p>
