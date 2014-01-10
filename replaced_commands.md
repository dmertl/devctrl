List of Commands Replaced with devctrl
======================================

	alias xdebug_on='export XDEBUG_CONFIG="idekey="'
	alias xdebug_off='unset XDEBUG_CONFIG'

	alias start_dev='sudo port load apache2 mysql5'
	alias stop_dev='sudo port unload apache2 mysql5'
	alias restart_dev='stop_dev; start_dev'
	alias start_apache='sudo port load apache2'
	alias stop_apache='sudo port unload apache2'
	alias restart_apache='stop_apache; start_apache'
	alias start_mysql='sudo port load mysql5'
	alias stop_mysql='sudo port unload mysql5'
	alias restart_mysql='stop_mysql; start_mysql'

	alias tunnel_onzra='sudo ssh -L 25:tokyo.onzra.com:25 dmertl@tokyo.onzra.com'

	alias log_www='clear; echo -n -e "\033]0;Logging\007"; sudo tail -fn0 /opt/local/var/db/mysql5/Monaco.local.err /opt/local/apache2/logs/error_log ~/dev/ONZRA/*/*/trunk/app/tmp/logs/*.log ~/dev/ONZRA/*/*/branches/*/app/tmp/logs/*.log'
