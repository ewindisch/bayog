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
