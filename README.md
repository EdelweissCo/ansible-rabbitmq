**Table of Contents**

- [Changelog](#Changelog)
- [Instructions](#Instructions)
- [License](#License)
- [Author](#Author)

## Changelog

- Forked [Ansible-RabbitMQ](https://github.com/mrlesmithjr/ansible-rabbitmq) by [Larry Smith Jr](https://github.com/mrlesmithjr)
- Added all vagrant hosts to *rabbitmq_cluster* ansible group
- Pinned RabbitMQ version to 3.6.16-2 (the latest version allowing all dependencies to be satisfied in the existing setup)
- Enabled port forwarding in Vagrantfile
- Removed default port forwarding rules and added forwarding for port 15672 for the master node

## Instructions

Install Ansible role on your host:

```bash
sudo ansible-galaxy install -r requirements.yml -f
```

Now spin up the environment...

```bash
cd Vagrant && vagrant up
```

Open [http://localhost:15672](http://localhost:15672) in your browser and use *rabbitmqadmin* / *rabbitmqadmin* to log in.

## License

MIT

## Author

Larry Smith Jr.

- [@mrlesmithjr](https://www.twitter.com/mrlesmithjr)
- [EverythingShouldBeVirtual](http://everythingshouldbevirtual.com)
- [mrlesmithjr@gmail.com](mailto:mrlesmithjr@gmail.com)
