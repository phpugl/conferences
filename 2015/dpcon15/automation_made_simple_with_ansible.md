Erika Heidi - "Automation made simple with Ansible"
===================================================

Automation tools can save you a lot of time when dealing with server configuration and project deployments. However, 
some developers might feel slightly intimidated by the complexity present in tools like Puppet and Chef.

This talk will present you Ansible, a clean and straightforward automation tool created with focus on simplicity and 
efficiency. You will learn how to get started with Ansible and write your first playbooks to control one or hundreds 
of servers.

Sources
-------

 * Talk: <https://speakerdeck.com/erikaheidi/automation-made-simple-with-ansible-1>
 * Blog: <http://www.erikaheidi.com>
 * Twitter: <https://twitter.com/erikaheidi>
 * Github: <https://github.com/erikaheidi>

Notes
-----

Ansible macht es dem Administrator möglich Linuxsysteme fernzusteuern und zu verändern. Dafür werden keine Clients auf
dem Zielsystem benötigt. Ansible arbeite also Agentless über SSH.

* yaml configuration
* inventory file
  * Ini format
  * list of servers
  * grouping
* Playbook = Manifest = Reciepe
  * could have variables
  * loops
  * condition per task
* Template
  * System/Service configuration file
  * e.g.: Apache VHost
* Handler
  * Restart a service or daemon
  * Wird nur ausgeführt wenn der Task erfolgreich war
  * Task --notify--> Handler
* Tagging ermöglicht das nur bestimmte Teile ausgeführt werden


