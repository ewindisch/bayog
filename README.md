bayog
=====

Bayesian filter for system logs

usage
=====
pipe log into 'sa-log'. You'll want to modify this script
to do something for any positive results (the unusual logs)

learning
========

Train a bad message:
 echo "message" | sa-log-learn spam

Train a good message:
 echo "message" | sa-log-learn ham

installation
============

This requires spamassassin, although we're not actually
processing emails. We use the spamassassin bayesian filter
for log analysis.

You will want to disable all of the email-related checks
in your spamassassin installation. Eventually, this
project should include reasonable spamassassin configuration
settings.

You must run 'spamd'.
