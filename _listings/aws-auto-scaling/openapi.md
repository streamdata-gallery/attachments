swagger: "2.0"
x-collection-name: AWS Auto Scaling
x-complete: 1
info:
  title: AWS Auto Scaling API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AttachInstances:
    get:
      summary: Attach Instances
      description: Attaches one or more EC2 instances to the specified Auto Scaling
        group.
      operationId: attachInstances
      x-api-path-slug: actionattachinstances-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the group
        type: string
      - in: query
        name: InstanceIds.member.N
        description: One or more instance IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Instance
  /?Action=AttachLoadBalancers:
    get:
      summary: Attach Load Balancers
      description: Attaches one or more Classic load balancers to the specified Auto
        Scaling group.
      operationId: attachLoadBalancers
      x-api-path-slug: actionattachloadbalancers-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the group
        type: string
      - in: query
        name: LoadBalancerNames.member.N
        description: One or more load balancer names
        type: string
      responses:
        200:
          description: OK
      tags:
      - Load Balancers
  /?Action=AttachLoadBalancerTargetGroups:
    get:
      summary: Attach Load Balancer Target Groups
      description: Attaches one or more target groups to the specified Auto Scaling
        group.
      operationId: attachLoadBalancerTargetGroups
      x-api-path-slug: actionattachloadbalancertargetgroups-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group
        type: string
      - in: query
        name: TargetGroupARNs.member.N
        description: The Amazon Resource Names (ARN) of the target groups
        type: string
      responses:
        200:
          description: OK
      tags:
      - Load Balancers