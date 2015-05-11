Installation
============

[doc_toc]

Composer
--------

You can install this plugin into your CakePHP application using composer.

The recommended way to install composer packages is:

        composer require cakemanager/cakephp-posttypes: 1.0.0

For the stable use, use the 1.*-releases.

Configuration
-------------

You will need to add the following line to your application's `config/bootstrap.php` file:

        Plugin::load('PostTypes', ['bootstrap' => true, 'routes' => true]);

Now you are ready to add your PostTypes. Lets load the `PostTypesComponent` into your `AppController`:

        public function initialize()
        {
            // code

            $this->loadComponent('PostTypes.PostTypes');

            // code
        }
