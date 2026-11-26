# CST8915-Lab-8

**Student Name**: Collin MacLeod
**Student ID**: macl0379
**Course**: CST8915 Full-stack Cloud-native Development
**Semester**: Fall 2026

---

## Demo Video

🎥 [Watch Demo Video](https://youtu.be/bQDElL7mYno)

---

## Deployment Files

:memo: [All in One Deployment File](/aps-all-in-one.yaml)
:memo: [Admin Task File](/admin-tasks.yaml)

## Investigate Azure Managed Services

### What Azure managed services could replace self-hosted MongoDB and RabbitMQ?

Through my research, I found a few PaaS options to replace the self-hosted MongoDB and RabbitMQ services. These services remove the need to manage the state of the servers, making the workload lighter for developers.

For self-hosted MongoDB, the easiest solution is to move to Azure Cosmos DB for MongoDB, a managed database service. This would reduce the operational expense. Cosmos DB performs automatic updates, removing the need to orchestrate the containers for updates. It also handles the storage of data, backups and point-in-time restore out of the box.

Using Azure Service Bus instead of RabbitMQ as a messaging queue provides a lot of the same benefits. As a PaaS, Azure Service Bus also benefits from automatic updates and patches. Azure Service Bus comes with great redundancy, with data replicated across all availability zones and supports geo-redundancy. Scaling would also be a benefit, as traffic spikes could be handled without the need to orchestrate containers.
