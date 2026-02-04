[README.md](https://github.com/user-attachments/files/25078662/README.md)


---

## Reliability & Scalability
- Multi-AZ deployment across all critical components
- Auto Scaling Group automatically replaces failed instances
- Application Load Balancer routes traffic only to healthy targets
- Amazon RDS Multi-AZ performs automatic failover during outages

---

## Cost Considerations
- Primary cost drivers: EC2 instances, RDS Multi-AZ, ALB, NAT Gateway
- Architecture prioritizes availability and resilience over minimal cost
- Cost optimization options include Savings Plans, right-sizing, and VPC endpoints

---

## Trade-offs
- EC2 chosen over Lambda or ECS to demonstrate foundational high-availability patterns
- RDS chosen over DynamoDB to support relational data requirements
- Multi-AZ cost accepted to eliminate Availability Zone–level failure risk

---

## Lessons Learned
- High availability significantly increases database and networking costs
- Security group referencing scales better than IP-based network controls
- Correct service placement provides more resilience than adding complexity
