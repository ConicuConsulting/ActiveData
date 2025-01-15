# ActiveData: A Relational Intelligence Ecosystem

ActiveData is a cutting-edge relational intelligence ecosystem designed to redefine how data is understood and leveraged. Moving beyond traditional databases, ActiveData utilizes relational intelligence principles, dynamic graph structures, and adaptive queries to create systems that are intelligent, scalable, and empowering.

## Key Features

### 1. **ActiveGraph**
The dynamic data layer that models relationships between entities in real-time:
- **Nodes**: Represent entities (e.g., patients, conditions, symptoms).
- **Edges**: Represent relationships between nodes, dynamically updating based on context.
- **Dynamic Mapping**: Adapts to changes in data and relationships in real-time.

### 2. **ActiveShell**
A human-readable interface for interacting with data:
- **Noun-Verb-Truth Syntax**: Enables intuitive and powerful queries.
- **CRUD Operations**: Manage data easily with commands like `Get-Node`, `New-Node`, `Update-Node`, and `Remove-Node`.
- **Real-Time Updates**: Make immediate changes to relationships and data.

### 3. **Relational API**
Seamless integration with external platforms:
- **Memory Layer**: Retains historical context for deeper insights.
- **Integration Middleware**: Connects ActiveData with LLMs, external databases, and applications.

### 4. **ActiveData Studio**
A visual interface for managing relational intelligence:
- **Graph Visualization**: Explore and interact with dynamic graph structures visually.
- **User-Friendly Interface**: Accessible to both technical and non-technical users.

### 5. **ActiveData Modules**
Expandable modules for advanced functionality:
- **ActiveMetrics**: Real-time analytics and insights.
- **ActiveAutomation**: Workflow automation based on relational triggers.
- **ActiveAccess**: Fine-grained permissions tied to graph relationships.

## Quick Start

### Installation
To get started, clone the repository and install dependencies:

```bash
# Clone the repo
git clone https://github.com/ConicuConsulting/ActiveData.git
cd ActiveData

# Install dependencies
pip install -r requirements.txt
```

### Setting Up ActiveData
1. **Configure ActiveData**: Adjust settings in the `config.yaml` file for your environment.
2. **Run the Application**:

```bash
python app.py
```

3. **Access the UI**: Navigate to `http://localhost:5000` to explore the ActiveData Studio.

### ActiveShell Commands
Below are some example commands to get started with ActiveShell:

- **Find all patients with a specific condition**:

```powershell
Get-Node -Type Patient | Where-Object { $_.Condition -eq 'Cancer' }
```

- **Add a new patient**:

```powershell
New-Node -Type Patient -Attributes @{ 
    Name = 'John Doe'; 
    Age = 45; 
    Gender = 'Male'; 
    Condition = 'Diabetes'; 
    Location = 'Melbourne' 
}
```

- **Update patient information**:

```powershell
Update-Node -Type Patient -Id 123 | Set-Property -Phone '0400-123-456' -Email 'john.doe@example.com'
```

- **Delete a patient record**:

```powershell
Remove-Node -Type Patient -Id 123
```

## Architecture

ActiveData is built using a cloud-agnostic architecture for scalability, accessibility, and security:

- **Azure Front Door**: Scalable and secure entry point.
- **Azure API Management**: Middleware for seamless integration.
- **Azure Cosmos DB**: Persistent and scalable graph storage.
- **Azure Key Vault**: Secure storage for secrets.
- **Azure Application Insights**: Real-time monitoring and performance tracking.

## Contributing

We welcome contributions to improve ActiveData. To contribute:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-name`).
3. Commit changes (`git commit -m 'Add feature'`).
4. Push to the branch (`git push origin feature-name`).
5. Open a Pull Request.

## License

This project is licensed under the [CC-BY-NC-SA 4.0 License](LICENSE.md).

## Documentation

For detailed documentation, check out:
- [Whitepaper: ActiveData](./docs/whitepaper.md)
- [ActiveShell Queries](./docs/activeshell_queries.md)
- [API Reference](./docs/api_reference.md)

## Contact

For questions, issues, or collaboration inquiries:
- **Email**: callum@youmatter.systems
- **GitHub Issues**: [Report an Issue](https://github.com/ConicuConsulting/ActiveData/issues)

---
**ActiveData: Redefining Relational Intelligence.**
