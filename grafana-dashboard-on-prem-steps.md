# Steps to Import Grafana Rule and Dashboard

## Prerequisites
- Ensure you have Grafana installed and accessible.
- Have access to the Grafana instance where you want to import the rule and dashboard.

## Steps

### Step 1: Download the JSON Files
1. Go to [Link-1](https://github.com/pramodmax/artemis-grafana-dashboard/blob/main/amq-consumer-evaluation-group.json) for the Grafana rule and [Link-2](https://github.com/pramodmax/artemis-grafana-dashboard/blob/main/Red%20Hat%20AMQ%20Broker%20-%20On-prem.json) for the Grafana dashboard.
2. Click on the **Raw** button to view the raw JSON content.
3. Copy the JSON content and save it to your local machine as:
   - `amq-consumer-evaluation-group.json`
   - `Red-Hat-AMQ-Broker-On-prem.json`

### Step 2: Import Grafana Rule (Link-1 JSON)
1. Open your Grafana instance and log in with the necessary credentials.
2. Navigate to **Alerting > Manage alert riles** to manage rules.
3. Select **New alert rule** (depending on the Grafana version) and configure the rule settings.
4. In the JSON editor, paste the contents from `amq-consumer-evaluation-group.json`.
5. Save the rule.

### Step 3: Import Grafana Dashboard (Link-2 JSON)
1. In the Grafana UI, go to **Dashboards > Manage**.
2. Click **Import**.
3. In the **Import via panel json** field, paste the contents of `Red-Hat-AMQ-Broker-On-prem.json`.
4. Click **Load**.
5. Configure any required settings such as **Data Sources** if prompted.
6. Click **Import** to finalize the dashboard import.

### Step 4: Verify the Imports
1. Go to **Alerting** to ensure the rule appears as expected.
2. Navigate to **Dashboards** to verify that the "Red Hat AMQ Broker - On-prem" dashboard is available and functions correctly.

## Notes
- Ensure that the appropriate data sources are configured and linked in Grafana.
- Review the imported rule and dashboard configurations to verify they align with your monitoring requirements.
