vagrant-postgres-9.4
====================

14.04 Ubuntu 9.4 box for toying with. To use

    $vagrant up

As you probably don't want to pollute your box with postgres 9.4 beta development libs, just ssh to you vagrant box to play around:

    $vagrant ssh
    #password postgres
    vagrant-box$>psql -U postgres -W -h 127.0.0.1
    postgres=# create table person (                                                                                
      id serial,
      first_name varchar(40),
      last_name varchar(40),
      extra_details jsonb
    );
    
Meant for toying around with postgres, not an actual place to store real data.
