1) Download Jmeter. Set the java home till /bin to avoid going to the path everytime running from cmd.
2) Download the pluginlibrary jar 
		https://jmeter-plugins.org/install/Install/
		add in lib/ext
		restart jmeter
3) Open PluginManager and click on available plugins and install all plugins
		Restart Jmeter
4) Download the property file reader from https://drive.google.com/file/d/1z2e7iJ_tn-T5OpflwZYcE39EngANjnJQ/view?usp=sharing
		Add in lib/ext
		Restart Jmeter



Open cmd and run the below command to execute in non-gui mode.

jmeter -n -t <<PATH OF JMX>> -l <<PATH TO CREATE RESULTS FILE>> -Jenvionment=integration/staging

Example:
jmeter -n -t C:\Users\nilesh.gupta\Desktop\poc.jmx -l C:\Users\nilesh.gupta\Desktop\results_file_poc.jtl -Jenvionment=integration