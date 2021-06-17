# Docker Magento

## Setup

__1) Add 127.0.0.1 magento.local to etc/hosts file__

__2) Create new or add existing Magento project__

- Create new project
	- ```make new-project PUBLIC_KEY={{ public key }} PRIVATE_KEY={{ private key }}```
		- Keys can be found in https://marketplace.magento.com/customer/accessKeys/

- Add existing project
	- Create new "magento" folder inside project root and paste an existing Magento project to it  
    
__3) Start Docker__

```docker-compose up -d```

__4) Install Magento__

```make install```

__5) Setup Xdebug in IDE__

- PhpStorm should offer you automatic setup, which should look something like this

![PhpStorm setup](https://i.ibb.co/GVqfVs5/phpstorm.jpg "Logo Title Text 1")

