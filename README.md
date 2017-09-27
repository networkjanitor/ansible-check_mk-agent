check_mk-agent
=========


Role Variables
--------------

	checkmk_agent_deb_url: '' # url pointing to the check_mk agent deb, probably on your check_mk instance
	xinetd_type: UNLISTED
	xinetd_port: 6556
	xinetd_socket_type: stream
	xinetd_protocol: tcp
	xinetd_wait: no
	xinetd_user: root
	xinetd_server: /usr/bin/check_mk_agent
	xinetd_ip_filter: false
	xinetd_only_from: 127.0.0.1 10.0.20.1 10.0.20.2
	xinetd_disable: no

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: networkjanitor.check_mk-agent }

License
-------

MIT
