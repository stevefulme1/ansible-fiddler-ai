> **EXPERIMENTAL** - This collection is a proof of concept and is not production ready.
> Modules may use placeholder API endpoints and have not been validated against real infrastructure.
> Do not use in production environments.

# Fiddler AI Ansible Collection

Ansible Collection for Fiddler AI model performance management platform. Provides modules for managing projects, models, datasets, alerts, custom metrics, explainability, and baselines via the Fiddler REST API.

## Requirements

- Ansible >= 2.16
- Python >= 3.9
- `requests` Python library

## Installation

```bash
ansible-galaxy collection install stevefulme1.fiddler_ai
```

## Modules

- `stevefulme1.fiddler_ai.project` - Manage projects in Fiddler AI
- `stevefulme1.fiddler_ai.project_info` - Retrieve project information from Fiddler AI
- `stevefulme1.fiddler_ai.model` - Manage models in Fiddler AI
- `stevefulme1.fiddler_ai.model_info` - Retrieve model information from Fiddler AI
- `stevefulme1.fiddler_ai.dataset` - Manage datasets in Fiddler AI
- `stevefulme1.fiddler_ai.dataset_info` - Retrieve dataset information from Fiddler AI
- `stevefulme1.fiddler_ai.alert` - Manage alerts in Fiddler AI
- `stevefulme1.fiddler_ai.alert_info` - Retrieve alert information from Fiddler AI
- `stevefulme1.fiddler_ai.custom_metric` - Manage custom metrics in Fiddler AI
- `stevefulme1.fiddler_ai.custom_metric_info` - Retrieve custom metric information from Fiddler AI
- `stevefulme1.fiddler_ai.explainability` - Configure explainability settings in Fiddler AI
- `stevefulme1.fiddler_ai.baseline` - Manage baselines in Fiddler AI

## Roles

- `fiddler_setup` - Install and configure Fiddler AI integration
- `fiddler_monitor` - Deploy monitoring configuration for Fiddler AI models

## Event-Driven Ansible

- `fiddler_alerts` - Fiddler AI Alerts event source plugin

## License

GPL-3.0-or-later

## Author

Steve Fulmer ([@stevefulme1](https://github.com/stevefulme1))
