Git Repo: https://github.com/YuvarajRajadurai/Brain-Tasks-App.git

Application deployed kubernetes Loadbalancer ARN: 
aff9d061f895b4fb48a1c4e48b760cca-2068598688.us-east-2.elb.amazonaws.com

 <img width="940" height="385" alt="image" src="https://github.com/user-attachments/assets/069f0e81-41fa-4a91-b2f5-dbdab4794183" />


**ECR:**

 <img width="940" height="365" alt="image" src="https://github.com/user-attachments/assets/7f9f442d-1921-4c1e-92db-382c33b5d8b6" />

 <img width="940" height="301" alt="image" src="https://github.com/user-attachments/assets/72f0eae5-4d4c-436a-ac0a-be4f70f6501c" />


**Docker Build:**

PS E:\YuvarajJR\Devops\Projects\Brain-Tasks-App> docker build -t brain-tasks-app:1.0 .
[+] Building 15.8s (9/9) FINISHED                                                                                     docker:desktop-linux
 => [internal] load build definition from dockerfile                                                                                  0.2s
 => => transferring dockerfile: 194B                                                                                                  0.1s
 => [internal] load metadata for docker.io/library/nginx:alpine                                                                       3.2s
 => [auth] library/nginx:pull token for registry-1.docker.io                                                                          0.0s
 => [internal] load .dockerignore                                                                                                     0.0s
 => => transferring context: 163B                                                                                                     0.0s
 => [1/3] FROM docker.io/library/nginx:alpine@sha256:72ba65eb42c10344912a84ff42408db7d34f2feb642204570ab8fc5ffd29f1d3                11.4s
 => => resolve docker.io/library/nginx:alpine@sha256:72ba65eb42c10344912a84ff42408db7d34f2feb642204570ab8fc5ffd29f1d3                 0.0s
 => => sha256:6636b9fc203ce74d0b07a1d3f48cfa0151b23fa5e787232908e560673a66b553 20.52MB / 20.52MB                                     10.6s
 => => sha256:51900e10fb9cfad93aa74360e5f938efcbe6d3396a380867b7561c84e5cd2daf 1.21kB / 1.21kB                                        0.9s
 => => sha256:8f924cf5086c7b8a67e8b3e03b22851c1de8e11b0433c21904ef340d89e5014e 1.40kB / 1.40kB                                        0.9s
 => => sha256:bc98d76756163f687c200ed6114df3904623bbb5e7698b420efaf8ef3c81dfcf 404B / 404B                                            0.9s
 => => sha256:58c524ea09ced2269cb14533d95b80de9fea9532abbf171585d8acee413893f2 956B / 956B                                            0.4s
 => => sha256:af7dd138f4591521064c208da6af07f487ebc3e5b350989c0ec2017b3e5208e3 628B / 628B                                            0.4s
 => => sha256:850bf2dcecff7924b238f0b7cbae7b456e5206453b784fe6b4adfc949add274a 4.40MB / 4.40MB                                        4.8s
 => => extracting sha256:850bf2dcecff7924b238f0b7cbae7b456e5206453b784fe6b4adfc949add274a                                             0.3s
 => => extracting sha256:af7dd138f4591521064c208da6af07f487ebc3e5b350989c0ec2017b3e5208e3                                             0.0s
 => => extracting sha256:58c524ea09ced2269cb14533d95b80de9fea9532abbf171585d8acee413893f2                                             0.0s
 => => extracting sha256:bc98d76756163f687c200ed6114df3904623bbb5e7698b420efaf8ef3c81dfcf                                             0.0s
 => => extracting sha256:51900e10fb9cfad93aa74360e5f938efcbe6d3396a380867b7561c84e5cd2daf                                             0.0s
 => => extracting sha256:8f924cf5086c7b8a67e8b3e03b22851c1de8e11b0433c21904ef340d89e5014e                                             0.0s
 => => extracting sha256:6636b9fc203ce74d0b07a1d3f48cfa0151b23fa5e787232908e560673a66b553                                             0.6s
 => [internal] load build context                                                                                                     0.2s
 => => transferring context: 318.42kB                                                                                                 0.2s
 => [2/3] COPY nginx.conf /etc/nginx/conf.d/default.conf                                                                              0.2s
 => [3/3] COPY dist/ /usr/share/nginx/html/                                                                                           0.1s
 => exporting to image                                                                                                                0.4s
 => => exporting layers                                                                                                               0.1s
 => => exporting manifest sha256:8370ec2771debbed4c8b82bfcc6b62ed17cf555a89c4e9a2a2a6335c45a72a0e                                     0.0s
 => => exporting config sha256:c5940562a5c7f45d9c2a2439a857aaa2a289c51474bb402a7a43cda26f2bf049                                       0.0s
 => => exporting attestation manifest sha256:744cac5b698cc280423cadc1de810fa18d3af9f44611dfd9ed06d39fdfc0fcda                         0.0s
 => => exporting manifest list sha256:7a188140222bf77fc4621a1ad6c0ead163840ad9d7b081f039c21d0d9accaba6                                0.0s
 => => naming to docker.io/library/brain-tasks-app:1.0                                                                                0.0s
 => => unpacking to docker.io/library/brain-tasks-app:1.0                                                                             0.1s

View build details: docker-desktop://dashboard/build/desktop-linux/desktop-linux/py2nbwd26dztz3b7qi5gqkc8r

 
 <img width="940" height="274" alt="image" src="https://github.com/user-attachments/assets/7d158103-38a7-4ccc-ab5b-b507e30da472" />


 
<img width="940" height="319" alt="image" src="https://github.com/user-attachments/assets/d6e27ce8-86f8-4c52-95b5-64681524124d" />

 
<img width="940" height="334" alt="image" src="https://github.com/user-attachments/assets/fbea4bd5-2609-487d-86ae-255e0f7b31cd" />
 



**EKS Cluster create:** First I have created t3.micro --nodes 1 and again scale node to 2 the add t3.small again.

PS E:\YuvarajJR\Devops\Projects\Brain-Tasks-App> eksctl create cluster --name brain-tasks-cluster --region us-east-2 --nodegroup-name brain-tasks-nodes --node-type t3.micro --nodes 1 --nodes-min 1 --nodes-max 2
2026-09-13 18:26:37 [ℹ]  eksctl version 0.228.0
2026-09-13 18:26:37 [ℹ]  using region us-east-2
2026-09-13 18:26:38 [ℹ]  setting availability zones to [us-east-2a us-east-2b us-east-2c]
2026-09-13 18:26:38 [ℹ]  subnets for us-east-2a - public:192.168.0.0/19 private:192.168.96.0/19
2026-09-13 18:26:38 [ℹ]  subnets for us-east-2b - public:192.168.32.0/19 private:192.168.128.0/19
2026-09-13 18:26:38 [ℹ]  subnets for us-east-2c - public:192.168.64.0/19 private:192.168.160.0/19
2026-09-13 18:26:38 [ℹ]  nodegroup "brain-tasks-nodes" will use "" [AmazonLinux2023/1.34]
2026-09-13 18:26:38 [!]  Auto Mode will be enabled by default in an upcoming release of eksctl. This means managed node groups and managed networking add-ons will no longer be created by default. To maintain current behavior, explicitly set 'autoModeConfig.enabled: false' in your cluster configuration. Learn more: https://eksctl.io/usage/auto-mode/
2026-09-13 18:26:38 [ℹ]  using Kubernetes version 1.34
2026-09-13 18:26:38 [ℹ]  creating EKS cluster "brain-tasks-cluster" in "us-east-2" region with managed nodes
2026-09-13 18:26:38 [ℹ]  will create 2 separate CloudFormation stacks for cluster itself and the initial managed nodegroup
2026-09-13 18:26:38 [ℹ]  if you encounter any issues, check CloudFormation console or try 'eksctl utils describe-stacks --region=us-east-2 --cluster=brain-tasks-cluster'
2026-09-13 18:26:38 [ℹ]  Kubernetes API endpoint access will use default of {publicAccess=true, privateAccess=false} for cluster "brain-tasks-cluster" in "us-east-2"
2026-09-13 18:26:38 [ℹ]  CloudWatch logging will not be enabled for cluster "brain-tasks-cluster" in "us-east-2"
2026-09-13 18:26:38 [ℹ]  you can enable it with 'eksctl utils update-cluster-logging --enable-types={SPECIFY-YOUR-LOG-TYPES-HERE (e.g. all)} --region=us-east-2 --cluster=brain-tasks-cluster'
2026-09-13 18:26:38 [ℹ]  default addons kube-proxy, coredns, metrics-server, vpc-cni were not specified, will install them as EKS addons
2026-09-13 18:26:38 [ℹ]  
2 sequential tasks: { create cluster control plane "brain-tasks-cluster", 
    2 sequential sub-tasks: { 
        2 sequential sub-tasks: { 
            1 task: { create addons },
            wait for control plane to become ready,
        },
        create managed nodegroup "brain-tasks-nodes",
    } 
}
2026-09-13 18:26:38 [ℹ]  building cluster stack "eksctl-brain-tasks-cluster-cluster"
2026-09-13 18:26:40 [ℹ]  deploying stack "eksctl-brain-tasks-cluster-cluster"
2026-09-13 18:27:10 [ℹ]  waiting for CloudFormation stack "eksctl-brain-tasks-cluster-cluster"
2026-09-13 18:27:40 [ℹ]  waiting for CloudFormation stack "eksctl-brain-tasks-cluster-cluster"
2026-09-13 18:28:41 [ℹ]  waiting for CloudFormation stack "eksctl-brain-tasks-cluster-cluster"
2026-09-13 18:29:42 [ℹ]  waiting for CloudFormation stack "eksctl-brain-tasks-cluster-cluster"
2026-09-13 18:30:43 [ℹ]  waiting for CloudFormation stack "eksctl-brain-tasks-cluster-cluster"
2026-09-13 18:31:44 [ℹ]  waiting for CloudFormation stack "eksctl-brain-tasks-cluster-cluster"
2026-09-13 18:32:44 [ℹ]  waiting for CloudFormation stack "eksctl-brain-tasks-cluster-cluster"
2026-09-13 18:33:45 [ℹ]  waiting for CloudFormation stack "eksctl-brain-tasks-cluster-cluster"
2026-09-13 18:34:46 [ℹ]  waiting for CloudFormation stack "eksctl-brain-tasks-cluster-cluster"
2026-09-13 18:35:47 [ℹ]  waiting for CloudFormation stack "eksctl-brain-tasks-cluster-cluster"
2026-09-13 18:36:48 [ℹ]  waiting for CloudFormation stack "eksctl-brain-tasks-cluster-cluster"
2026-09-13 18:36:52 [ℹ]  creating addon: kube-proxy
2026-09-13 18:36:52 [ℹ]  successfully created addon: kube-proxy
2026-09-13 18:36:53 [ℹ]  creating addon: coredns
2026-09-13 18:36:54 [ℹ]  successfully created addon: coredns
2026-09-13 18:36:55 [!]  recommended policies were found for "vpc-cni" addon, but since OIDC is disabled on the cluster, eksctl cannot configure the requested permissions; the recommended way to provide IAM permissions for "vpc-cni" addon is via pod identity associations; after addon creation is completed, add all recommended policies to the config file, under `addon.PodIdentityAssociations`, and run `eksctl update addon`
2026-09-13 18:36:55 [ℹ]  creating addon: vpc-cni
2026-09-13 18:36:55 [ℹ]  successfully created addon: vpc-cni
2026-09-13 18:39:01 [ℹ]  building managed nodegroup stack "eksctl-brain-tasks-cluster-nodegroup-brain-tasks-nodes"
2026-09-13 18:39:02 [ℹ]  deploying stack "eksctl-brain-tasks-cluster-nodegroup-brain-tasks-nodes"
2026-09-13 18:39:02 [ℹ]  waiting for CloudFormation stack "eksctl-brain-tasks-cluster-nodegroup-brain-tasks-nodes"
2026-09-13 18:39:33 [ℹ]  waiting for CloudFormation stack "eksctl-brain-tasks-cluster-nodegroup-brain-tasks-nodes"
2026-09-13 18:40:33 [ℹ]  waiting for CloudFormation stack "eksctl-brain-tasks-cluster-nodegroup-brain-tasks-nodes"
2026-09-13 18:42:28 [ℹ]  waiting for CloudFormation stack "eksctl-brain-tasks-cluster-nodegroup-brain-tasks-nodes"
2026-09-13 18:42:28 [ℹ]  waiting for the control plane to become ready
2026-09-13 18:42:30 [✔]  saved kubeconfig as "C:\\Users\\Admin\\.kube\\config"
2026-09-13 18:42:30 [ℹ]  no tasks
2026-09-13 18:42:30 [✔]  all EKS cluster resources for "brain-tasks-cluster" have been created
2026-09-13 18:42:31 [ℹ]  nodegroup "brain-tasks-nodes" has 1 node(s)
2026-09-13 18:42:31 [ℹ]  node "ip-192-168-41-160.us-east-2.compute.internal" is ready
2026-09-13 18:42:31 [ℹ]  waiting for at least 1 node(s) to become ready in "brain-tasks-nodes"
2026-09-13 18:42:31 [ℹ]  nodegroup "brain-tasks-nodes" has 1 node(s)
2026-09-13 18:42:31 [ℹ]  node "ip-192-168-41-160.us-east-2.compute.internal" is ready
2026-09-13 18:42:31 [✔]  created 1 managed nodegroup(s) in cluster "brain-tasks-cluster"
2026-09-13 18:42:32 [ℹ]  creating addon: metrics-server
2026-09-13 18:42:33 [ℹ]  successfully created addon: metrics-server
2026-09-13 18:42:35 [ℹ]  kubectl command should work with "C:\\Users\\Admin\\.kube\\config", try 'kubectl get nodes'
2026-09-13 18:42:35 [✔]  EKS cluster "brain-tasks-cluster" in "us-east-2" region is ready

<img width="940" height="204" alt="image" src="https://github.com/user-attachments/assets/c756c78a-d3f3-4cd9-aa66-87278f89da03" />

 <img width="940" height="179" alt="image" src="https://github.com/user-attachments/assets/b1c3f408-a802-464c-8a31-d3ab29e25794" />

<img width="764" height="444" alt="image" src="https://github.com/user-attachments/assets/b4a5623f-e7ce-402a-b441-35d242acfc01" />

<img width="940" height="109" alt="image" src="https://github.com/user-attachments/assets/1fbd98e6-e2e8-434e-aaf1-aad1bf8c336b" />


**Create IAM role for code build:**

<img width="940" height="44" alt="image" src="https://github.com/user-attachments/assets/654f8e56-156b-4d62-817e-8ce932666d3a" />

 
Authorize the CodeBuild IAM role inside the EKS cluster:
 
<img width="935" height="266" alt="image" src="https://github.com/user-attachments/assets/ea95fb88-3280-45e1-806d-83560694f461" />

 <img width="940" height="271" alt="image" src="https://github.com/user-attachments/assets/14ae2b3d-52d3-4ef0-b295-75d71b4b3543" />


**Code Build:**
<img width="940" height="242" alt="image" src="https://github.com/user-attachments/assets/851d9817-ddf8-443a-b944-de394d19c993" />

**Build log:
**

[Container] 2026/09/13 16:11:07.055082 Running on CodeBuild On-demand 
[Container] 2026/09/13 16:11:07.055104 Waiting for agent ping 
[Container] 2026/09/13 16:11:07.634518 Waiting for DOWNLOAD_SOURCE 
[Container] 2026/09/13 16:11:09.184906 Phase is DOWNLOAD_SOURCE 
[Container] 2026/09/13 16:11:09.185713 CODEBUILD_SRC_DIR=/codebuild/output/src4135077381/src 
[Container] 2026/09/13 16:11:09.186135 YAML location is /codebuild/output/src4135077381/src/buildspec.yaml 
[Container] 2026/09/13 16:11:09.187851 Setting HTTP client timeout to higher timeout for S3 source 
[Container] 2026/09/13 16:11:09.187929 Processing environment variables 
[Container] 2026/09/13 16:11:09.589797 No runtime version selected in buildspec. 
[Container] 2026/09/13 16:11:09.608143 Moving to directory /codebuild/output/src4135077381/src 
[Container] 2026/09/13 16:11:09.608257 Cache is not defined in the buildspec 
[Container] 2026/09/13 16:11:09.771800 Skip cache due to: no paths specified to be cached 
[Container] 2026/09/13 16:11:09.772123 Registering with agent 
[Container] 2026/09/13 16:11:09.937912 Phases found in YAML: 3 
[Container] 2026/09/13 16:11:09.937940 BUILD: 4 commands 
[Container] 2026/09/13 16:11:09.937943 POST_BUILD: 5 commands 
[Container] 2026/09/13 16:11:09.937945 PRE_BUILD: 6 commands 
[Container] 2026/09/13 16:11:09.938253 Phase complete: DOWNLOAD_SOURCE State: SUCCEEDED 
[Container] 2026/09/13 16:11:09.938264 Phase context status code: Message: 
[Container] 2026/09/13 16:11:10.290156 Entering phase INSTALL 
[Container] 2026/09/13 16:11:10.446321 Phase complete: INSTALL State: SUCCEEDED 
[Container] 2026/09/13 16:11:10.446341 Phase context status code: Message: 
[Container] 2026/09/13 16:11:10.483251 Entering phase PRE_BUILD 
[Container] 2026/09/13 16:11:10.637349 Running command echo "Logging in to ECR..." 
Logging in to ECR... 

[Container] 2026/09/13 16:11:10.643146 Running command AWS_ACCOUNT_ID=$(aws sts get-caller-identity --query Account --output text) 

[Container] 2026/09/13 16:11:27.465349 Running command AWS_REGION=$AWS_DEFAULT_REGION 

[Container] 2026/09/13 16:11:27.470912 Running command ECR_URI=$AWS_ACCOUNT_ID.dkr.ecr.$AWS_REGION.amazonaws.com/brain-tasks-app 

[Container] 2026/09/13 16:11:27.475998 Running command aws ecr get-login-password --region $AWS_REGION | docker login --username AWS --password-stdin $ECR_URI 
WARNING! Your password will be stored unencrypted in /root/.docker/config.json. 
Configure a credential helper to remove this warning. See 
https://docs.docker.com/engine/reference/commandline/login/#credentials-store 

Login Succeeded 

[Container] 2026/09/13 16:11:28.050491 Running command IMAGE_TAG=$CODEBUILD_RESOLVED_SOURCE_VERSION 

[Container] 2026/09/13 16:11:28.056716 Phase complete: PRE_BUILD State: SUCCEEDED 
[Container] 2026/09/13 16:11:28.056730 Phase context status code: Message: 
[Container] 2026/09/13 16:11:28.097294 Entering phase BUILD 
[Container] 2026/09/13 16:11:28.098491 Running command echo "Building Docker image..." 
Building Docker image... 

[Container] 2026/09/13 16:11:28.104217 Running command docker build --platform linux/amd64 -t $ECR_URI:$IMAGE_TAG . 
Sending build context to Docker daemon 332.8kB 

Step 1/5 : FROM nginx:alpine 
alpine: Pulling from library/nginx 
55afa1ecc21d: Pulling fs layer 
850bf2dcecff: Pulling fs layer 
af7dd138f459: Pulling fs layer 
58c524ea09ce: Pulling fs layer 
bc98d7675616: Pulling fs layer 
51900e10fb9c: Pulling fs layer 
8f924cf5086c: Pulling fs layer 
6636b9fc203c: Pulling fs layer 
58c524ea09ce: Waiting 
8f924cf5086c: Waiting 
6636b9fc203c: Waiting 
51900e10fb9c: Waiting 
af7dd138f459: Verifying Checksum 
af7dd138f459: Download complete 
850bf2dcecff: Verifying Checksum 
850bf2dcecff: Download complete 
55afa1ecc21d: Verifying Checksum 
55afa1ecc21d: Download complete 
58c524ea09ce: Verifying Checksum 
58c524ea09ce: Download complete 
51900e10fb9c: Verifying Checksum 
51900e10fb9c: Download complete 
bc98d7675616: Verifying Checksum 
bc98d7675616: Download complete 
8f924cf5086c: Verifying Checksum 
8f924cf5086c: Download complete 
6636b9fc203c: Verifying Checksum 
6636b9fc203c: Download complete 
55afa1ecc21d: Pull complete 
850bf2dcecff: Pull complete 
af7dd138f459: Pull complete 
58c524ea09ce: Pull complete 
bc98d7675616: Pull complete 
51900e10fb9c: Pull complete 
8f924cf5086c: Pull complete 
6636b9fc203c: Pull complete 
Digest: sha256:72ba65eb42c10344912a84ff42408db7d34f2feb642204570ab8fc5ffd29f1d3 
Status: Downloaded newer image for nginx:alpine 
---> 1b595815db66 
Step 2/5 : COPY nginx.conf /etc/nginx/conf.d/default.conf 
---> 49228ea6e6cd 
Step 3/5 : COPY dist/ /usr/share/nginx/html/ 
---> feec9381c80f 
Step 4/5 : EXPOSE 80 
---> [Warning] The requested image's platform (linux/amd64) does not match the detected host platform (linux/arm64/v8) and no specific platform was requested 
---> Running in f8837903b8f8 
Removing intermediate container f8837903b8f8 
---> a3502cb89023 
Step 5/5 : CMD ["nginx", "-g", "daemon off;"] 
---> [Warning] The requested image's platform (linux/amd64) does not match the detected host platform (linux/arm64/v8) and no specific platform was requested 
---> Running in 8e2336fc6790 
Removing intermediate container 8e2336fc6790 
---> 404b57da973b 
Successfully built 404b57da973b 
Successfully tagged 251478238401.dkr.ecr.us-east-2.amazonaws.com/brain-tasks-app:1680b841a8e9313ea5cde7eaf4be2798e6650206 

[Container] 2026/09/13 16:11:31.807637 Running command echo "Pushing Docker image..." 
Pushing Docker image... 

[Container] 2026/09/13 16:11:31.813030 Running command docker push $ECR_URI:$IMAGE_TAG 
The push refers to repository [251478238401.dkr.ecr.us-east-2.amazonaws.com/brain-tasks-app] 
91216e975ceb: Preparing 
7381c2df26c6: Preparing 
bf413c2718bc: Preparing 
85c413237288: Preparing 
67184216cf5a: Preparing 
04a84c2e9c88: Preparing 
c6d0e2de973a: Preparing 
a90b008e1901: Preparing 
5c0955c965f2: Preparing 
34884abbe928: Preparing 
a90b008e1901: Waiting 
5c0955c965f2: Waiting 
34884abbe928: Waiting 
c6d0e2de973a: Waiting 
04a84c2e9c88: Waiting 
85c413237288: Layer already exists 
67184216cf5a: Layer already exists 
bf413c2718bc: Layer already exists 
04a84c2e9c88: Layer already exists 
a90b008e1901: Layer already exists 
c6d0e2de973a: Layer already exists 
5c0955c965f2: Layer already exists 
34884abbe928: Layer already exists 
7381c2df26c6: Pushed 
91216e975ceb: Pushed 
1680b841a8e9313ea5cde7eaf4be2798e6650206: digest: sha256:f421affb692ab75c6def5d147d5a1606fcca9a50b77132106fd5547abfdfa1fb size: 2406 

[Container] 2026/09/13 16:11:32.859874 Phase complete: BUILD State: SUCCEEDED 
[Container] 2026/09/13 16:11:32.859894 Phase context status code: Message: 
[Container] 2026/09/13 16:11:32.899176 Entering phase POST_BUILD 
[Container] 2026/09/13 16:11:32.900138 Running command echo "Updating Kubernetes deployment..." 
Updating Kubernetes deployment... 

[Container] 2026/09/13 16:11:32.905927 Running command aws eks update-kubeconfig --region $AWS_REGION --name brain-tasks-cluster 
Added new context arn:aws:eks:us-east-2:251478238401:cluster/brain-tasks-cluster to /root/.kube/config 

[Container] 2026/09/13 16:11:33.579474 Running command kubectl set image deployment/brain-tasks-app brain-tasks-app=$ECR_URI:$IMAGE_TAG 

[Container] 2026/09/13 16:11:36.372820 Running command kubectl rollout status deployment/brain-tasks-app 
deployment "brain-tasks-app" successfully rolled out 

[Container] 2026/09/13 16:11:37.177731 Running command echo "Deployment successful." 
Deployment successful. 

[Container] 2026/09/13 16:11:37.183486 Phase complete: POST_BUILD State: SUCCEEDED 
[Container] 2026/09/13 16:11:37.183500 Phase context status code: Message: 
[Container] 2026/09/13 16:11:37.232316 Set report auto-discover timeout to 5 seconds 
[Container] 2026/09/13 16:11:37.232408 Expanding base directory path: . 
[Container] 2026/09/13 16:11:37.234915 Assembling file list 
[Container] 2026/09/13 16:11:37.234928 Expanding . 
[Container] 2026/09/13 16:11:37.237472 Expanding file paths for base directory . 
[Container] 2026/09/13 16:11:37.237488 Assembling file list 
[Container] 2026/09/13 16:11:37.237491 Expanding **/* 
[Container] 2026/09/13 16:11:37.240151 No matching auto-discover report paths found 
[Container] 2026/09/13 16:11:37.240167 Report auto-discover file discovery took 0.007851 seconds 
[Container] 2026/09/13 16:11:37.240180 Phase complete: UPLOAD_ARTIFACTS State: SUCCEEDED 
[Container] 2026/09/13 16:11:37.240184 Phase context status code: Message: 



**Code Pipeline:**
 
<img width="940" height="299" alt="image" src="https://github.com/user-attachments/assets/df9240d4-57fd-47ce-a67f-75aa952763db" />


**EC2 Instance:**

 <img width="964" height="230" alt="image" src="https://github.com/user-attachments/assets/7751235f-fc26-4fbb-a773-ac5b337f2dbc" />


**Cloudwatch:**
 
<img width="956" height="395" alt="image" src="https://github.com/user-attachments/assets/a50ff96d-b7f7-4060-b997-471d452908f4" />

 <img width="940" height="280" alt="image" src="https://github.com/user-attachments/assets/d0e68817-45c6-430d-a72a-483272ec6b78" />


**Sample Log:**

2026-09-13T16:11:37.531Z
[Container] 2026/09/13 16:11:37.183486 Phase complete: POST_BUILD State: SUCCEEDED
2026-09-13T16:11:37.531Z
[Container] 2026/09/13 16:11:37.183500 Phase context status code: Message:
2026-09-13T16:11:37.531Z
[Container] 2026/09/13 16:11:37.232316 Set report auto-discover timeout to 5 seconds
2026-09-13T16:11:37.531Z
[Container] 2026/09/13 16:11:37.232408 Expanding base directory path: .
2026-09-13T16:11:37.531Z
[Container] 2026/09/13 16:11:37.234915 Assembling file list
2026-09-13T16:11:37.531Z
[Container] 2026/09/13 16:11:37.234928 Expanding .
2026-09-13T16:11:37.531Z
[Container] 2026/09/13 16:11:37.237472 Expanding file paths for base directory .
2026-09-13T16:11:37.531Z
[Container] 2026/09/13 16:11:37.237488 Assembling file list
2026-09-13T16:11:37.531Z
[Container] 2026/09/13 16:11:37.237491 Expanding **/*
2026-09-13T16:11:37.531Z
[Container] 2026/09/13 16:11:37.240151 No matching auto-discover report paths found
2026-09-13T16:11:37.531Z
[Container] 2026/09/13 16:11:37.240167 Report auto-discover file discovery took 0.007851 seconds
2026-09-13T16:11:37.531Z
[Container] 2026/09/13 16:11:37.240180 Phase complete: UPLOAD_ARTIFACTS State: SUCCEEDED

**Application link:**
http://aff9d061f895b4fb48a1c4e48b760cca-2068598688.us-east-2.elb.amazonaws.com:3000/

 
<img width="940" height="473" alt="image" src="https://github.com/user-attachments/assets/7bca87f1-1dbb-45ed-a5a9-a02ff522f308" />

