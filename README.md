# Monitor Kafka Connect and Connectors
Kafka Connect is a free, open-source component of Apache Kafka® that serves as a centralized data hub for simple data integration between databases, key-value stores, search indexes, and file systems. You can use Kafka Connect to stream data between Apache Kafka® and other data systems and quickly create connectors that move large data sets in and out of Kafka.

# Benefits of Kafka Connect
Kafka Connect provides the following benefits:

- Data-centric pipeline: Connect uses meaningful data abstractions to pull or push data to Kafka.
- Flexibility and scalability: Connect runs with streaming and batch-oriented systems on a single node (standalone) or scaled to an organization-wide service (distributed).
- Reusability and extensibility: Connect leverages existing connectors or extends them to fit your needs and provides lower time to production.

# Use the Connect REST interface
Kafka Connect’s REST API enables administration of the cluster. This includes APIs to view the configuration of connectors and the status of their tasks, as well as to alter their current behavior (for example, changing configuration and restarting tasks).

Once a Kafka Connect cluster is up and running, you can monitor and modify it. This section describes some common management tasks you can do when using the REST API.

Since Kafka Connect is intended to be run as a service, it also supports a REST API for managing connectors. By default this service runs on port 8083. When executed in distributed mode, the REST API will be the primary interface to the cluster. You can make requests to any cluster member; the REST API automatically forwards requests if required.

Although you can use standalone mode by submitting a connector on the command line, it also runs the REST interface. This is useful for getting status information, adding and removing connectors without stopping the process, and more.


