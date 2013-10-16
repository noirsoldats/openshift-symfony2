Symfony on OpenShift Express
============================

This git repository helps you get up and running quickly w/ a Sympfony installation
on OpenShift Express.


Running on OpenShift
----------------------------

Create an account at http://openshift.redhat.com/

Create a php-5.3 application (you can call your application whatever you want)

    rhc create-app -a symfonyphp -t php-5.3 --from-code git@github.com:noirsoldats/openshift-symfony2.git

That's it, you can now checkout your application at:

    http://sympfonyphp-$your_domain.rhcloud.com


NOTES:

GIT_ROOT/.openshift/action_hooks/build:
  This has a few lines to ensure that the cache dir exists and is writable for the web server.

Security:
Nothing has been done to secure this installation.
