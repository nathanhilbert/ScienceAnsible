Vagrant Box for UrbIS Base
-----------------------

**Components include**

 - jupyterhub (python 2.7 & python 3.4)
    - matplotlib
    - numpy
    - pandas
    - pyspatial (2.7 only)
    - fiona
    - gdal and ogr
    - shapely
    - pyscopg2
    - postgis (pyscopg2 styled for postgis)
 - Postgresql with pointcloud and postgis
 - various libraries
    - gdal and ogr
    - pdal

**Get Started**

Install: 

  - [Virtualbox](https://www.virtualbox.org/wiki/Downloads)
  - [Ansible](https://valdhaus.co/writings/ansible-mac-osx/)
  - [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)

Run:

```

  $ git clone https://code-int.ornl.gov/nlh/urbisvagrant
  $ cd urbisvagrant
  $ vagrant up  -- this will take a while

```

Usage:

Navigate to 192.168.99.151:8000 in your browser.  The homeshare folder is shared to the urbisvagrant/data/homeshare folder.
