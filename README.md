# Welcome to Share My Space

## Table of Contents
1. [General Info](#general-info)
2. [Technologies](#technologies)
4. [Packages](#packages)
5. [Keywords](#keywords)
6. [Useful Bash Commands](#useful-bash-commands)
### General Info
***
Welcome to [Share My Space](https://www.sharemyspace.space/), the start-up that will make space safer than zone 51 !!
You can find your access to gmail, teams, outlook, OpenVPN, teamsviewer, gitlab, your gpg key and also livebox password in a file named Documents/<your_name> on your laptop.

### Technologies
***
A list of technologies used by SMS :
* [GitLab](https://gitlab.sms.local) : Useful commands [here](https://education.github.com/git-cheat-sheet-education.pdf).
* [MySQL](https://www.mysql.com/fr/) :
  * To install MySQL :
  
    ```
    $ sudo apt-get update
    $ sudo apt-get install mysql-shell
    ```
  * To connect to MysQl :
  
    ```
    $ mysql -u <name> -p
    ```
* [Workbench](https://www.mysql.com/fr/products/workbench/)
* [OpenVPN](https://openvpn.net/community-downloads/)
* [Eclipse](https://www.eclipse.org/downloads/packages/installer)
* [Anaconda](https://docs.anaconda.com/anaconda/install/linux/)
* [Pycharm](https://itsfoss.com/install-pycharm-ubuntu/)


### Packages
***
  
A list of packages created and used by SMS :
* [sms_report](https://gitlab.sms.local/calm/sms_report)
* [sms_query](https://gitlab.sms.local/calm/sms_query)
* [pyphoton](https://gitlab.sms.local/cleopatre/pyphoton)
* [PyObs](https://gitlab.sms.local/cleopatre/pyobs)
* [Orbit_det](https://gitlab.sms.local/calm/orbit_det)
* [keepcalm](https://gitlab.sms.local/calm/keepcalm)
* [celestools](https://gitlab.sms.local/calm/celestools)

For each package :
* Follow README.md instructions
* Create and fill in [user.cfg](https://gitlab.sms.local/calm/sms_query/-/blob/master/user.cfg)

A little intro about the installation. 
```
$ conda activate <name_env>
$ export CALMDATA=user.cfg
$ git clone <link_repo>
$ conda install --file requirements.txt
$ python setup.py install

```

Install orekit : 
```
$ conda install -c conda-forge orekit==11.1
$ unzip orekit-data.zip
$ mv orekit-data orekit-data-master
$ export OREKITDATA=orekit-data-master 
```

### Keywords
***
| Physics | Sensors   | Specific to SMS | Computer sciences |
|:--------------|:-------------|:--------------|:--------------|
| **Astrometry**: Measurement of positions, motions, and magnitudes of stars | **MTOS** : Multi Telescope Observation Station | **CATUSSA** : unified catalog for SSA (Space Situational Awareness) | **Thread** : small set of instructions designed to be scheduled and executed by the CPU independently of the parent process |
**Photometry**: Measurement of light, in terms of its perceived brightness to the human eye | **STOS** : Signal Telescope Observation Station | **CALM**: Collision Avoidance for Limited Maneuvers | **SSH (Secure Shell)** : Network communication protocol that enables two computers to communicate |
**Streak** : Space object trail (waste or active satellite) | **GNSS** : Global Navigation Satellite Systems |**CLEOPATRE**: On demand Space surveillance and tracking | **VPS (Virtual Private Server)** : Virtual server that appears to the user as a dedicated server, but actually installed on a computer serving multiple websites |
**Perigee** : The point at which the satellite is closest to the Earth | **SLR** : Satellite Laser Ranging | **INDEMN**: Congestion Analysis | **OS** : Operating System |
**Apogee** : The point at which the satellite is farthest to the Earth | **Gain** : Electrons conversion to ADU (Analog Digital unit) | **MANEXT**: Maneuver Extractor| **IDE** : Integrated Development Environment |
**Photonics Chain** : Path of a photon from the bright object to the lens | **Offset** : ADU value added by default in order to be always above the Threshold of the detection of a pixel (photosites) on the camera | **SSB**: Space Sustainability Bulletin | **API (Application Programming Interface)**: Simplify software development and innovation by enabling applications to exchange data and functionality easily and safely | 
**LEO** : Low earth Orbit | **Quantum efficiency**: Conversion rate from photons to electrons as a function of the photon's wavelength | **SSR** : Space Sustainability Report
**MEO** : Medium earth Orbit | **Lambertian Sphere** : Model of diffuse light reflection on a surface | **ODL**: Orbital Data Library
**GEO** : Geostationary earth orbit | **Albedo** : Reflection rate of an object or a star |**SSL**: Space Sustainability Label |
**HEO** : High Earth Orbit | **Focal Length** : Distance to the convergence of light rays in an optical instrument
**GTO** : Geostationary Transfert Orbit from LEO to GEO | **Seeing** : Angle created by the diffraction of a light ray through the atmosphere characterizes the spread
**SSO** : Sun Synchronous orbit | **PSF** : Point Spread Function
**CAM** : Collision Avoidance Maneuver
**PTA** : Potential Threat Assessment
**CA** : Conjunction Assisment
**Delta V** : Speed variation for orbital maneuvers
**Attitude** : Rotation rate of a satellite
**OD** : Orbit Determination
**IOD** : Initial Orbit Determination
**TLE** : Towlines elements
**SP** : Special perturbation
**SGP4** : Simplify Perturbation Model
**Radec** : Angle description 
**Ephemeris** : Tables that gives the trajectory of naturally occurring astronomical objects as well as artificial satellites in the sky, i.e., the position (and possibly velocity) over time 
### Useful Bash Commands
***

* Create a new conda environment :
    ```
    $ conda create -n <env_name>
    ```
* Activate a conda environment :
    ```
    $ conda activate <env_name>
    ```
* List of conda environments :
    ```
    $ conda info --envs
    ```
* Open a gpg file :
    ```
    $ gpg --output <new_file_name> -d <file_name.gpg> 
    ```
* Update all packages :
    ```
    $ sudo apt update && sudo apt upgrade
    ```
* Find a file on your laptop : 
    ```
    $ sudo find / -name "*<file_name>*"
    ```	
* Get the path location : 
    ```
    $ pwd
    ```	
* Redirect to a folder : 
    ```
    $ cd <folder_name>
    ```	
* Go backward in the path: 
    ```
    $ cd ..
    ```	
* Get the folder content : 
    ```
    $ ls
    ```	
* To see administrator rights : 
    ```
    $ ll
    ```	
* To change administrator rights : 
    ```
    $ chmod 777 <file_name>
    ```	
* To unzip a file : 
    ```
    $ unzip <file_name.zip> -d /<path>
    ```	
* To create an environment variable : 
    ```
    $ export <VARIABLE_NAME>=<path>
    ```	
* To check if the variable has been created : 
    ```
    $ echo <VARIABLE_NAME>
    ```	

 * To connect to a server using ssh protocol : 
    ```
    $ ssh username@server
    ```			
 * Some allias  :
    ```
    $ alias sms2='ssh pouzin@192.168.1.23'
    $ alias sms9='ssh npouzin@192.168.20.9'
    $ alias calmenv='conda activate calmenv'
    $ alias python=python3
    ```

    * for keepcalm dl
    ```
    $ alias uk='pip uninstall keepcalm'
    $ alias yk='python setup.py install'
    ```


    * from git command
    ```
    $ alias gb='git branch'
    $ alias gcm='git checkout master'

    ```		


