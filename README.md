# Roles to deploy [counter application](https://github.com/vbatuev/counter-app) on Google Cloud Engine
Make sure that necessary packages are installed:
`pip -r requirements.txt`



Please note, that this playbooks uses [ansible dynamic inventory script](https://docs.ansible.com/ansible/2.5/scenario_guides/guide_gce.html) and you also need to configure service account in [google cloud engine](https://developers.google.com/identity/protocols/OAuth2ServiceAccount#creatinganaccount).

To deploy application use `deploy-app.yml` playbook


Then use `deploy-lb.yml` playbook to deploy load balancer.

TODO:
- Add tests
- Add CI
- Add some automation for firewalls, manage DNS zones and records

Then use `deploy-app-lb.yml` playbook to deploy load balancer.

