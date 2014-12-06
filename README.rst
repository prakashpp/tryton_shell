Welcome to Tryton Shell
=======================

Tryton shell is an interactive Python shell which allows you to play with the tryton ORM. To invoke the tryton shell, use this command::

  tryton_shell -c config_file -d database_name

Let's play with ORM
===================

Let's create a party::

  >>> from trytond.pool import Pool
  >>> B()  # Begin the transaction
  >>> Party = Pool().get('party.party')
  >>> party, = Party.create([{
  ...    'name': 'Joe Blow'
  >>> }])
  >>> E()  # End the transaction

Simple Right!

Suggestions!
============

Feel free to create issues or send PR.
