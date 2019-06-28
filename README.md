##### cloudformation-templates
`cloudformation_manage_bounces.yaml`
Deploys lambda code taken from AWS blueprint, and SNS topic with lambda endpoint subscription.
To setup working demo add SNS notification Topic in Email domain notification setting.

`cloudformation_ses_auto_stop.yaml`
Adds CloudWatch alarm which triggers SNS notification notifying by email and running Lambda to disable SES sending.

`cloudformation_state-manager_rds_stopped.yaml`
Stop RDS, SSM association. RDS cannot be stopped for more than 7 days. This ensures it stays stopped.
