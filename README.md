Users
=====

Ce role configure la création de l'utilisateur master.

Pour générer le mot de passe: 
<pre><code>$ python -c 'import crypt; print crypt.crypt("!redhat123#", "whatever")'</code></pre>

Requirements
------------

None.

Platform
--------

Debian ou RHEL

Role Variables
--------------

<pre><code>root_password: 0689X%92
users_name: 'master'
users_comment: 'User Master'
users_group: sudo
users_createhome: yes
users_password: '' # python2.7 -c 'import crypt; print crypt.crypt("PASSWORD", "whatever")'
users_to_delete: 'config' # pirate
</code></pre>

Dependencies
------------

Ce role se télécharge automatiquement à partir du requirements.yml


Author Information
------------------

Starfly Env Team
