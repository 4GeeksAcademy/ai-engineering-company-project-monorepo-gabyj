# Technical Context

## Current Stack and Systems

The available context does not specify a target stack for TrackFlow Tech. It does describe a legacy architecture consisting of:

- Two different warehouse management systems (WMS): commercial software at one warehouse and an advanced spreadsheet at the other.
- A corporate ERP system dating back to the early 2010s.
- Poorly documented point-to-point Python scripts.
- Databases hosted across two different cloud providers.
- System integrations built quickly and without sufficient documentation.
- Eight carriers across the two countries, each with independent APIs and tracking portals.

Therefore, no target programming language, framework, cloud provider, database, or deployment platform should be assumed until explicitly decided.

## Architecture and Technical Direction

The existing architecture is heterogeneous and provides neither centralized telemetry nor a shared view of data. The stated functional direction calls for unified APIs, event and data integration, centralized monitoring, and shared dashboards. Proposed capabilities include a global inventory API, an aggregated tracking endpoint, a data pipeline for dashboards, and ticketing and knowledge systems for customer support.

These capabilities are project needs, not implementation decisions that have already been adopted. The source document does not define services, contracts, protocols, data models, or a detailed target architecture.

## Technical Constraints and Requirements

- Operations span the United States and Spain, with different warehouses and systems.
- Integrations are needed with eight carriers and existing legacy platforms.
- Inventory, tracking, monitoring, and dashboard workflows need real-time or low-latency operational data.
- Order and customer inquiry workflows must remain available continuously, including outside office hours.
- The business operates in both Spanish and English. Multilingual support is recommended, though the system can start with one base language.
- Carrier, inventory, returns, and performance information needs to become structured and comparable.
- Automated decisions, such as return approvals and carrier selection, need to accommodate business rules and provide explainable recommendations.
- The technical team described has seven people, and new feature deployments currently take one to two weeks.