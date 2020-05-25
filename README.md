# Mokuroku - Inventory Manager

Mokuroku is scalable web application managing your Ansible® hosts and inventories. 

## Features

### Hosts collection

Collection of hosts periodically or on demand with added metadata per default: such as project, stage, zone and region.

These metadata allow to make queries and filters easy:

- Get all hosts of stage `production`
- Get hosts of a region in stage `integration`
- Get hosts of a project in a zone in any stage

### Pushing Hosts

Hosts may be added or updated to the inventory on push or by an event trigger, such as a task in an Ansible® run. This is especially useful on large inventories with 1000s of hosts where a collection run is expensive.

### Staled Hosts

When hosts won't be refreshed by a collection run, they will get into a stale state before archived. This allows to run clean-up tasks such as e.g. DNS records removal.

### Inventory Vars API

Add, update and change inventory plugin configs by an API.

## License / Trademarks

Affero General Public License (AGPLv3). Ansible® is a registered trademark of Red Hat®.

