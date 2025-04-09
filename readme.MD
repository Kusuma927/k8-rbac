# RBAC

#### PERMISSIONS ##############
## EKS is a different cluster and ALB is different service, EKS Cluster need to create and ALB Hence using this service.
REGION_CODE=us-east-1
CLUSTER_NAME=expense
ACC_ID=590184056608

Step1: OIDC Provider
eksctl utils associate-iam-oidc-provider \
    --region $REGION_CODE \
    --cluster $CLUSTER_NAME \
    --approve