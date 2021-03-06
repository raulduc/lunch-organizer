WEBClusive Lunch Organizer
========================

This is the Lunch Organizer, it keeps track of the lunch schedule
alerting people on HipChat about it.

1) Installing the Standard Edition
----------------------------------

When it comes to installing the Symfony Standard Edition, you have the
following options.

### Use Composer (*recommended*)

As Symfony uses [Composer][2] to manage its dependencies, the recommended way
to create a new project is to use it.

If you don't have Composer yet, download it following the instructions on
http://getcomposer.org/ or just run the following command:

    curl -s http://getcomposer.org/installer | php

Then, use the `create-project` command to generate a new Symfony application:

    php composer.phar create-project symfony/framework-standard-edition path/to/install

Composer will install Symfony and all its dependencies under the
`path/to/install` directory.

### Download an Archive File

To quickly test Symfony, you can also download an [archive][3] of the Standard
Edition and unpack it somewhere under your web server root directory.

If you downloaded an archive "without vendors", you also need to install all
the necessary dependencies. Download composer (see above) and run the
following command:

    php composer.phar install
    
2 ) Developing

### Compiling css

To compile the LESS files into CSS you need to have less installed and run a console command.

Install LESS (>= v1.3.3)
    
    npm install -g less
    
Compile CSS (will keep listening for file changes)

    app/console assetic:dump --watch
    
