# POCO
The POCO C++ Libraries are powerful cross-platform C++ libraries for building network- and internet-based applications that run on desktop, server, mobile, IoT, and embedded systems.

<h3>Follow the steps to install the POCO library on Ubuntu Linux</h3>

#### Update and Upgrade the APT package manager.
`sudo apt update`

`sudo apt upgrade`

#### Install the required dependencies.

## Compiler
`sudo apt install build-essential cmake git`

## Option (Install as per requirement)

`sudo apt install libssl-dev unixodbc unixodbc-dev libmysqlclient-dev libiodbc2-dev`

## For POCO NetSSL (SSL/TLS support)
`sudo apt install libssl-dev`

## For POCO Data library with PostgreSQL support
`sudo apt install libpq-dev`
 
Some packages belong to repositories (Xenial and Focal) that are unknown to Ubuntu 22.04. So add the repository using <a href="https://www.google.com/search?q=Add+APT">Add APT</a>.

#### Clone the source from the official repository.
`git clone -b master https://github.com/pocoproject/poco.git`

#### Create a build directory for building the source.
`mkdir -p poco-build && cd poco-build`

#### Generate build scripts.
`cmake ../poco`

#### Build the source using cmake.
`make -j4`

#### Install the POCO package.
`sudo make install`

Installed successfully, check if it is installed as /usr/local/include/Poco

`cd /usr/local/include/ && ls`

<b>Poco</b>
