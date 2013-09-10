amazons3sync
============

Synchronize local directories with your remote Amason S3 buckets using the Amazon S3 SOAP API

The goal of this project is to provide a simple interface to set up the synchronization between your local server directories and your Amazon S3 Buckets.

The aim is also to use the amazon_s3 project to ease the calls to the Amazon S3 SOAP API by using a a homogeneous library containing all the features we need to communicate with it.

The project has to be be fast developped, easy to install, easy to maintain and the most compatible with any web platform.

It is not a CMS like but mostly a library that could be integrated in any CMS.

The administration web interface provided by the project is what it is to show how it works and to give a simple web interface to use.

## The administration features

The tool must provide a easy-to-use and easy-to-understand web interface to condigure the synchronization between the local directories and the Amazon S3 Buckets.

The web interface is accessible using a login and a password. On installation, only one user can connect to the web interface meaning the admin.

The admin user can create new users with 2 authorization levels represented by 2 groups of user :

  1. read/write/delete: the users that belong to this group can do anything they want

  2. read: the users that belong to this group can only read the informations without having the ability to create or delete anything

The local directories must be selected under one main directory defined once on the installation.

The remote Amazon S3 Buckets can be on the same account or on different accounts. To ease the selection of the target bucket, the web interface allows to create ad store the available buckets that can be used.

## The storage features

As previously indicated, it has to be simple enough to install and maintain but also extensible.

To do so we don't rely on databases and uniquely on configuration/data system files. The only constraint is that the directory where the files are written has to be writable by the current web server executing the  PHP files.
