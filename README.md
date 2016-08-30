#Setup guidelines

##About
ITKore represents a drupal 8 platform from which new drupal 8 sites may be built. This way some of the trivial tasks are bypassed to start the project a little further ahead.
ITKore consists of three parts:
* ITKore profile (https://github.com/aakb/itkore-profile)
* ITKore theme (https://github.com/aakb/itkore-theme)
* Drupal 8 core

ITKore profile is a drupal install profile which holds custom modules and depends on some contrib modules. The profile also alters some default core configuration.

ITKore theme is a Drupal theme which holds the bare minimum for a theme to work.

## How to use?

###Buliding a new drupal core site with composer
If you are building a new drupal site locally in an ITK vagrant it is recommended to run the script file located at vagrant/base/scripts/setup-drupal8.sh.
The setup script will use composer to fetch the itkore-theme repo, itkore-profile repo and drupal core.
The script will use composer to fetch the required contrib modules and place them in the htdocs/modules folder

A local setup flow would be:

* Go to vagrant repo

* Create new local site:
```
./run.sh
```

* Run Drupal 8 setup script:
```
./base/scripts/setup-drupal8.sh
```

* Start up vagrant
* Setup site with drush or from browser

##ITKore theme
