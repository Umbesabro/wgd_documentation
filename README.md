Warehouse Dog Guard is an efficient application that enables tracking of sales/purchase orders, stock levels, and historical demand. By analyzing demand and stock levels, it suggests new purchase orders to ensure product availability while optimizing warehousing costs.

From an architectural perspective, the application is comprised of loosely coupled and highly scalable microservices.

The following technologies are utilized:

Backend: TypeScript + NestJS
Database: Postgres
Communication: RabbitMQ
The following are the repository links for each microservice:

API Gateway: https://github.com/Umbesabro/wgd_api_gateway - serves as an entry point to the application.
Store: https://github.com/Umbesabro/wgd_store - keeps track of purchase and sales orders.
Event Log: https://github.com/Umbesabro/wgd_event_log - persists events and sends them to the queue.
Warehouse: https://github.com/Umbesabro/wgd_warehouse - persists product and their stock levels.
Analyzer: TODO - responsible for persisting usage data, analyzing the current stock situation, and generating issues if needed.
